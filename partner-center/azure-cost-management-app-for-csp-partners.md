---
title: Azure Cost Management di Cloudyn per i partner CSP | Centro per i partner
description: Azure Cost Management di Cloudyn richiede l'accesso tramite provisioning dell'API Centro per i partner.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 9f5439f47dbc99421e493c9f84f8ea2469ba6525
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489387"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="d53ac-103">App Azure Cost Management per i partner CSP Azure</span><span class="sxs-lookup"><span data-stu-id="d53ac-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="d53ac-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="d53ac-104">Applies to</span></span>**

-  <span data-ttu-id="d53ac-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d53ac-105">Partner Center</span></span>

[<span data-ttu-id="d53ac-106">Ottieni ulteriori informazioni su Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="d53ac-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="d53ac-107">Prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="d53ac-107">Before you begin</span></span>
<span data-ttu-id="d53ac-108">Prima di poter utilizzare Azure Cost Management, assicurati che siano soddisfatti i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="d53ac-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="d53ac-109">Essere partner del programma Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="d53ac-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="d53ac-110">Essere in grado di creare un'app Web API di Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d53ac-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="d53ac-111">Panoramica</span><span class="sxs-lookup"><span data-stu-id="d53ac-111">Overview</span></span>

<span data-ttu-id="d53ac-112">Azure Cost Management di Cloudyn è un'app Web che consente di tenere traccia e gestire l'utilizzo di Azure da parte dei clienti e i costi di tale utilizzo.</span><span class="sxs-lookup"><span data-stu-id="d53ac-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="d53ac-113">Puoi usare l'app tramite l'API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d53ac-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="d53ac-114">Registra la tua app Web nel Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="d53ac-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="d53ac-115">Registrando un'app Web di Azure Active Directory nel Centro per i partner, abiliti l'accesso all'API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d53ac-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="d53ac-116">Accedi al [Centro per i partner](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) utilizzando un [account di amministratore globale o agente amministratore](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="d53ac-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="d53ac-117">Il **Centro per i Partner**, seleziona **le impostazioni Account** &gt; **[Gestione App](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="d53ac-117">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="d53ac-118">Nella sezione **Web App** fai clic su **Add new web app**.</span><span class="sxs-lookup"><span data-stu-id="d53ac-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="d53ac-119">**Nota**: se in precedenza hai creato un'app Web, puoi ignorare il passaggio 3.</span><span class="sxs-lookup"><span data-stu-id="d53ac-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="d53ac-120">Copia e salva i GUID **Commerce ID** e **App ID** per la tua app Web.</span><span class="sxs-lookup"><span data-stu-id="d53ac-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="d53ac-121">Entrambi gli ID ti serviranno per utilizzare la versione di valutazione gratuita di 30 giorni dell'app di gestione dei costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="d53ac-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="d53ac-122">Aggiungi una chiave privata alla tua app.</span><span class="sxs-lookup"><span data-stu-id="d53ac-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="d53ac-123">Nell'elenco a discesa accanto al pulsante **Add key** seleziona una durata di 1 o 2 anni.</span><span class="sxs-lookup"><span data-stu-id="d53ac-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="d53ac-124">Fai clic su **Add key**.</span><span class="sxs-lookup"><span data-stu-id="d53ac-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="d53ac-125">Copia e salva il valore della chiave privata.</span><span class="sxs-lookup"><span data-stu-id="d53ac-125">Copy and save the secret key value.</span></span> <span data-ttu-id="d53ac-126">Questo valore ti servirà per la versione di valutazione gratuita di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="d53ac-126">You will need this for the 30-day free trial.</span></span><br>
> [!NOTE]  
> <span data-ttu-id="d53ac-127">Le chiavi private dell'applicazione sono simili alle password con più date di scadenza.</span><span class="sxs-lookup"><span data-stu-id="d53ac-127">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="d53ac-128">Salva il valore della chiave in un luogo sicuro per l'utilizzo futuro.</span><span class="sxs-lookup"><span data-stu-id="d53ac-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d53ac-129">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d53ac-129">Next steps</span></span>
<span data-ttu-id="d53ac-130">Avvia una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="d53ac-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="d53ac-131">Per avviare la versione di valutazione ti serve quanto segue:</span><span class="sxs-lookup"><span data-stu-id="d53ac-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="d53ac-132">Credenziali di accesso al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d53ac-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="d53ac-133">GUID ID commerce</span><span class="sxs-lookup"><span data-stu-id="d53ac-133">Commerce ID GUID</span></span>
- <span data-ttu-id="d53ac-134">GUID ID app</span><span class="sxs-lookup"><span data-stu-id="d53ac-134">App ID GUID</span></span>
- <span data-ttu-id="d53ac-135">Valore della chiave privata dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="d53ac-135">Application secret key value</span></span>
