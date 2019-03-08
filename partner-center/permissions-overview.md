---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Tutti i dipendenti che hanno necessità di lavorare in Partner Center devono essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587744"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="c6d66-104">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="c6d66-104">Assign users roles and permissions</span></span>


<span data-ttu-id="c6d66-105">È stata configurare il profilo di partner inclusi ragione sociale e indirizzi, i dettagli sul supporto, esenzione di file, informazioni bancarie e il contatto principale per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="c6d66-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c6d66-106">Passaggio successivo: gli utenti configurati con le password e i ruoli in modo che possano iniziare a lavorare nel centro per i Partner con l'utente.</span><span class="sxs-lookup"><span data-stu-id="c6d66-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c6d66-107">Configurare i dipendenti di lavorare in Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c6d66-108">Determinare i tipi di accesso che al centro per i Partner gli utenti dispongono per i ruoli e autorizzazioni che finti.</span><span class="sxs-lookup"><span data-stu-id="c6d66-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c6d66-109">I ruoli sono correlati per le applicazioni che è interessata dalla propria azienda.</span><span class="sxs-lookup"><span data-stu-id="c6d66-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c6d66-110">Ad esempio, se l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo è il standard di Azure AD i ruoli di gestione, ad esempio amministratore globale del tenant, ma sarà necessario ruoli specifici per il programma CSP.</span><span class="sxs-lookup"><span data-stu-id="c6d66-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c6d66-111">Ogni programma svolge ruoli specifici a esso.</span><span class="sxs-lookup"><span data-stu-id="c6d66-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c6d66-112">I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="c6d66-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c6d66-113">Ruoli AAD-non includono MPN amministratore, amministratore profilo business, amministrazione di referral, admin incentivi e incentivi utente.</span><span class="sxs-lookup"><span data-stu-id="c6d66-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c6d66-114">Gestire le transazioni commerciali nel centro per i Partner (Azure AD e i ruoli CSP)</span><span class="sxs-lookup"><span data-stu-id="c6d66-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c6d66-115">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="c6d66-115">**Role**</span></span>|<span data-ttu-id="c6d66-116">**Le operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="c6d66-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c6d66-117">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c6d66-117">Global admin</span></span>|<span data-ttu-id="c6d66-118">• Possono accedere a tutti i Microsoft account/servizi con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="c6d66-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c6d66-119">• Creare ticket di supporto per il centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c6d66-120">• Visualizzare gli accordi sui listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="c6d66-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c6d66-121">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="c6d66-122">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="c6d66-122">User Admin</span></span>   | <span data-ttu-id="c6d66-123">• Visualizzare, creare e gestire gli utenti</span><span class="sxs-lookup"><span data-stu-id="c6d66-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="c6d66-124">• Visualizzare tutti i profili partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-124">• View all partner profiles</span></span>
||<span data-ttu-id="c6d66-125">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="c6d66-126">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="c6d66-126">Default user</span></span>|  <span data-ttu-id="c6d66-127">Visualizza profilo personale</span><span class="sxs-lookup"><span data-stu-id="c6d66-127">View My profile</span></span>   |
|<span data-ttu-id="c6d66-128">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="c6d66-128">Admin agent</span></span> | <span data-ttu-id="c6d66-129">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="c6d66-129">•    Customer management</span></span>
||<span data-ttu-id="c6d66-130">• Aggiungere l'elenco dei dispositivi al centro per i Partner <</span><span class="sxs-lookup"><span data-stu-id="c6d66-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="c6d66-131">• Creare e applicare i profili nei dispositivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="c6d66-132">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="c6d66-132">• Subscription management</span></span>
||<span data-ttu-id="c6d66-133">• Servizio integrità e soddisfare richieste per i clienti</span><span class="sxs-lookup"><span data-stu-id="c6d66-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="c6d66-134">• Richiesta delegati i privilegi di amministratore</span><span class="sxs-lookup"><span data-stu-id="c6d66-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="c6d66-135">• Visualizza i prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="c6d66-135">• View pricing and offers</span></span>
||<span data-ttu-id="c6d66-136">• La fatturazione</span><span class="sxs-lookup"><span data-stu-id="c6d66-136">• Billing</span></span>
||<span data-ttu-id="c6d66-137">• Amministra per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="c6d66-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="c6d66-138">• Registra un valore aggiunto rivenditore</span><span class="sxs-lookup"><span data-stu-id="c6d66-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="c6d66-139">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c6d66-139">Sales agent</span></span> | <span data-ttu-id="c6d66-140">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="c6d66-140">•    Customer management</span></span>
||<span data-ttu-id="c6d66-141">• Aggiungere l'elenco dei dispositivi al centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="c6d66-142">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="c6d66-142">• Subscription management</span></span>
||<span data-ttu-id="c6d66-143">Ticket di supporto di visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="c6d66-143">• View support tickets</span></span>
||<span data-ttu-id="c6d66-144">• Richiesta una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="c6d66-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="c6d66-145">• Gestire i lead dei clienti</span><span class="sxs-lookup"><span data-stu-id="c6d66-145">• Manage customer leads</span></span>
||<span data-ttu-id="c6d66-146">• Visualizzare il contratto del cliente</span><span class="sxs-lookup"><span data-stu-id="c6d66-146">• View the customer agreement</span></span>
||<span data-ttu-id="c6d66-147">• Registro un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="c6d66-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="c6d66-148">Agente help desk</span><span class="sxs-lookup"><span data-stu-id="c6d66-148">Helpdesk agent</span></span>| <span data-ttu-id="c6d66-149">• Cercare e visualizzare un cliente</span><span class="sxs-lookup"><span data-stu-id="c6d66-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="c6d66-150">• Modificare i dettagli cliente</span><span class="sxs-lookup"><span data-stu-id="c6d66-150">• Edit customer details</span></span>
||<span data-ttu-id="c6d66-151">• Guida risolvere cliente i problemi con la gestione di fatturazione o alla sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c6d66-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c6d66-152">• Richiedere il supporto per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="c6d66-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="c6d66-153">• Gestire le sottoscrizioni e fatturazione problemi per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="c6d66-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c6d66-154">Fornitore del Pannello di controllo (CPV).</span><span class="sxs-lookup"><span data-stu-id="c6d66-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c6d66-155">(Non-AAD ruolo e ruolo CSP)</span><span class="sxs-lookup"><span data-stu-id="c6d66-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c6d66-156">CPVs lo sviluppo di App per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="c6d66-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c6d66-157">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="c6d66-157">**Role**</span></span>   |<span data-ttu-id="c6d66-158">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="c6d66-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c6d66-159">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c6d66-159">Global admin</span></span>| <span data-ttu-id="c6d66-160">Visualizzare e gestire il profilo CPV</span><span class="sxs-lookup"><span data-stu-id="c6d66-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c6d66-161">Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV</span><span class="sxs-lookup"><span data-stu-id="c6d66-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="c6d66-162">Gestire l'appartenenza MPN e la propria azienda (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="c6d66-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="c6d66-163">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="c6d66-163">**Role**</span></span> | <span data-ttu-id="c6d66-164">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="c6d66-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c6d66-165">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="c6d66-165">MPN partner admin</span></span>|<span data-ttu-id="c6d66-166">•CAN aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="c6d66-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="c6d66-167">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="c6d66-168">• Vista legale, l'organizzazione, business e i profili MPN</span><span class="sxs-lookup"><span data-stu-id="c6d66-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="c6d66-169">• Visualizzare i dettagli di utente e i relativi dati di competenze</span><span class="sxs-lookup"><span data-stu-id="c6d66-169">• View user details and their skills data</span></span>
||<span data-ttu-id="c6d66-170">• Visualizza competenze</span><span class="sxs-lookup"><span data-stu-id="c6d66-170">• View competencies</span></span>
||<span data-ttu-id="c6d66-171">• Visualizzare e gestire i vantaggi</span><span class="sxs-lookup"><span data-stu-id="c6d66-171">• View and manage benefits</span></span>
||<span data-ttu-id="c6d66-172">Acquisto e la visualizzazione • ottenuta MPN</span><span class="sxs-lookup"><span data-stu-id="c6d66-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="c6d66-173">• Visualizzare MPN offre le fatture e cronologia degli ordini</span><span class="sxs-lookup"><span data-stu-id="c6d66-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c6d66-174">• Visualizza dati contributi di partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-174">• View partner contribution data</span></span>
||<span data-ttu-id="c6d66-175">• Possono utilizzare lo strumento di convalida Voucher</span><span class="sxs-lookup"><span data-stu-id="c6d66-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c6d66-176">-Visualizzare analitica dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="c6d66-176">- View customer data analytics</span></span>
|<span data-ttu-id="c6d66-177">Amministratore account</span><span class="sxs-lookup"><span data-stu-id="c6d66-177">Account admin</span></span>| <span data-ttu-id="c6d66-178">• È possibile aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="c6d66-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="c6d66-179">• Aggiunta o eliminazione di percorsi</span><span class="sxs-lookup"><span data-stu-id="c6d66-179">• Add or delete locations</span></span>
||<span data-ttu-id="c6d66-180">-Gestire i profili relativi agli account di per che amministratore</span><span class="sxs-lookup"><span data-stu-id="c6d66-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c6d66-181">• Assegnare ruoli per gli utenti nel tenant per i ruoli AAD non</span><span class="sxs-lookup"><span data-stu-id="c6d66-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c6d66-182">• Percorsi nei programmi di registrazione</span><span class="sxs-lookup"><span data-stu-id="c6d66-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="c6d66-183">Gestire i riferimenti (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="c6d66-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="c6d66-184">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="c6d66-184">**Role**</span></span>|<span data-ttu-id="c6d66-185">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="c6d66-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c6d66-186">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="c6d66-186">Referrals admin</span></span>       |<span data-ttu-id="c6d66-187">• Visualizzare, creare e gestire i profili di business</span><span class="sxs-lookup"><span data-stu-id="c6d66-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="c6d66-188">• Ricevere e gestire i riferimenti</span><span class="sxs-lookup"><span data-stu-id="c6d66-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="c6d66-189">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="c6d66-190">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="c6d66-190">Business profile admin</span></span>   |<span data-ttu-id="c6d66-191">• Visualizzare, creare e gestire il profilo di business</span><span class="sxs-lookup"><span data-stu-id="c6d66-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="c6d66-192">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="c6d66-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="c6d66-193">Gestire gli incentivi (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="c6d66-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="c6d66-194">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="c6d66-194">**Role**</span></span> | <span data-ttu-id="c6d66-195">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="c6d66-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c6d66-196">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-196">Incentives admin</span></span>|<span data-ttu-id="c6d66-197">• Avvia e gestisce gli incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="c6d66-198">• È possibile visualizzare e modificare tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c6d66-199">• È possibile visualizzare e modificare i dettagli fiscali e bancarie</span><span class="sxs-lookup"><span data-stu-id="c6d66-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c6d66-200">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="c6d66-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c6d66-201">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="c6d66-201">• Access support</span></span>
||<span data-ttu-id="c6d66-202">Pagamenti di incentivi controversia •</span><span class="sxs-lookup"><span data-stu-id="c6d66-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="c6d66-203">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-203">Incentives user</span></span>|<span data-ttu-id="c6d66-204">• Consente di visualizzare i programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="c6d66-205">• È possibile visualizzare e avviare le attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="c6d66-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c6d66-206">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="c6d66-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c6d66-207">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="c6d66-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c6d66-208">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="c6d66-208">• Access support</span></span>












