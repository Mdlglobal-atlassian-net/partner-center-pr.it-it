---
title: Azure Cost Management di Cloudyn per i partner CSP | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management di Cloudyn richiede l'accesso tramite provisioning dell'API Centro per i partner.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995795"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>App Azure Cost Management per i partner CSP Azure  

**Si applica a**

-  Centro per i partner

[Ottieni ulteriori informazioni su Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Prima di iniziare
Prima di poter utilizzare Azure Cost Management, assicurati che siano soddisfatti i requisiti seguenti:

- Essere partner del programma Cloud Solution Provider.
- Essere in grado di creare un'app Web API di Centro per i partner.

## <a name="overview"></a>Panoramica

Azure Cost Management di Cloudyn è un'app Web che consente di tenere traccia e gestire l'utilizzo di Azure da parte dei clienti e i costi di tale utilizzo. Puoi usare l'app tramite l'API del Centro per i partner.

## <a name="register-your-web-app-in-the-partner-center"></a>Registra la tua app Web nel Centro per i Partner
Registrando un'app Web di Azure Active Directory nel Centro per i partner, abiliti l'accesso all'API del Centro per i partner. 
1.  Accedi al [Centro per i partner](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) utilizzando un [account di amministratore globale o agente amministratore](create-user-accounts-and-set-permissions.md).
2.  Il **Centro per i Partner**, seleziona **le impostazioni Account** &gt; **[Gestione App](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Nella sezione **Web App** fai clic su **Add new web app**.
<br> **Nota**: se in precedenza hai creato un'app Web, puoi ignorare il passaggio 3.
4.  Copia e salva i GUID **Commerce ID** e **App ID** per la tua app Web. Entrambi gli ID ti serviranno per utilizzare la versione di valutazione gratuita di 30 giorni dell'app di gestione dei costi di Azure.

## <a name="add-a-secret-key-to-your-app"></a>Aggiungi una chiave privata alla tua app.
1. Nell'elenco a discesa accanto al pulsante **Add key** seleziona una durata di 1 o 2 anni.
2. Fai clic su **Add key**. 
3. Copia e salva il valore della chiave privata. Questo valore ti servirà per la versione di valutazione gratuita di 30 giorni.<br>
   > [!NOTE]  
   > Le chiavi private dell'applicazione sono simili alle password con più date di scadenza. Salva il valore della chiave in un luogo sicuro per l'utilizzo futuro.

## <a name="next-steps"></a>Passaggi successivi
Avvia una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).
Per avviare la versione di valutazione ti serve quanto segue:
- Credenziali di accesso al Centro per i partner
- GUID ID commerce
- GUID ID app
- Valore della chiave privata dell'applicazione
