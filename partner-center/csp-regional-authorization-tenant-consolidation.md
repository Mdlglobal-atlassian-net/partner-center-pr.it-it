---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
keywords: migrazione dei clienti, provisioning, account tenant, consolidamento dei tenant
ms.openlocfilehash: e895fd049211a3dfcb4db930b75d94906563b700
ms.sourcegitcommit: 09f6988db95a3d7c62f2cf16f02cabc2c4418646
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/17/2018
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="036a9-104">Consolidamento dei tenant per l'autorizzazione regionale per CSP</span><span class="sxs-lookup"><span data-stu-id="036a9-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="036a9-105">Si applica a</span><span class="sxs-lookup"><span data-stu-id="036a9-105">Applies to</span></span>**

-  <span data-ttu-id="036a9-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="036a9-106">Partner Center</span></span>
-  <span data-ttu-id="036a9-107">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="036a9-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="036a9-108">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="036a9-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="036a9-109">\[Alcune informazioni sono relative a un prodotto non definitivo che potrebbe subire modifiche sostanziali prima del rilascio sul mercato.</span><span class="sxs-lookup"><span data-stu-id="036a9-109">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="036a9-110">Microsoft non riconosce alcuna garanzia, espressa o implicita, in merito alle informazioni qui fornite.\]</span><span class="sxs-lookup"><span data-stu-id="036a9-110">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="036a9-111">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="036a9-111">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="036a9-112">**Nota** Devi conoscere tutte le sottoscrizioni e il numero di postazioni per i tuoi clienti di cui è stato eseguito il provisioning dagli account per la transizione.</span><span class="sxs-lookup"><span data-stu-id="036a9-112">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="036a9-113">Nell'ambito del processo di migrazione, dovrai eseguire nuovamente il provisioning degli stessi esatti abbonamenti con lo stesso numero di postazioni nel nuovo account CSP centralizzato.</span><span class="sxs-lookup"><span data-stu-id="036a9-113">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="036a9-114">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="036a9-114">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="036a9-115">Il consolidamento dei tenant è una scelta del partner.</span><span class="sxs-lookup"><span data-stu-id="036a9-115">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="036a9-116">Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente.</span><span class="sxs-lookup"><span data-stu-id="036a9-116">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="036a9-117">Tieni presente che potrebbe essere richiesto anche l'intervento dei clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-117">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="036a9-118">Prepararsi per la migrazione</span><span class="sxs-lookup"><span data-stu-id="036a9-118">Prepare for migration</span></span>


-   <span data-ttu-id="036a9-119">Accedi a <https://partnercenter.microsoft.com> con l'account per la transizione (esistente) e prendi nota di tutti i clienti e di tutti i servizi di cui è stato eseguito il provisioning per tali clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-119">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![elenco dei clienti regionali](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="036a9-121">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="036a9-121">Migrate customer accounts</span></span>


1.  <span data-ttu-id="036a9-122">Accedi a <https://partnercenter.microsoft.com> con l'account per la transizione (nuovo) e passa all'elenco Clienti dal dashboard del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="036a9-122">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="036a9-123">Seleziona Clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-123">Select Customers.</span></span>

3.  <span data-ttu-id="036a9-124">Fai cli su **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="036a9-124">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="036a9-125">Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-125">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="036a9-126">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="036a9-126">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="036a9-127">**Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL.</span><span class="sxs-lookup"><span data-stu-id="036a9-127">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="036a9-128">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="036a9-128">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="036a9-129">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="036a9-129">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="036a9-130">Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="036a9-130">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="036a9-131">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-131">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="036a9-132">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo l'invio del contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="036a9-132">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="036a9-133">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="036a9-133">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="036a9-134">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="036a9-134">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="036a9-135">Nel dashboard del Centro per i partner fai clic su **Clienti** nel menu di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="036a9-135">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="036a9-136">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-136">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="036a9-137">Fai clic su **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-137">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="036a9-138">Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo.</span><span class="sxs-lookup"><span data-stu-id="036a9-138">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="036a9-139">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-139">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![screenshot dell'elenco clienti](images/regionalcustomer2.png)

6.  <span data-ttu-id="036a9-141">Fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="036a9-141">Click **Submit.**</span></span>

<span data-ttu-id="036a9-142">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-142">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="036a9-143">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-143">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="036a9-144">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-144">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="036a9-145">**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni.</span><span class="sxs-lookup"><span data-stu-id="036a9-145">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="036a9-146">Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-146">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="036a9-147">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="036a9-147">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="036a9-148">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="036a9-148">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="036a9-149">Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-149">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="036a9-150">Accedi a <https://partnercenter.microsoft.com> con l'account CSP di **origine della transizione** e passa all'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-150">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="036a9-151">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="036a9-151">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="036a9-152">Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="036a9-152">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="036a9-153">**Nota** La sospensione della sottoscrizione consente di evitare doppie fatturazioni.</span><span class="sxs-lookup"><span data-stu-id="036a9-153">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="036a9-154">La sottoscrizione è indicata con lo stato **Sospeso** nell'elenco delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="036a9-154">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="036a9-155">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="036a9-155">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="036a9-156">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="036a9-156">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="036a9-157">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="036a9-157">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="036a9-158">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="036a9-158">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="036a9-159">Nota che non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP in base all'uso di Azure come nel caso delle sottoscrizioni CSP di Office 365.</span><span class="sxs-lookup"><span data-stu-id="036a9-159">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="036a9-160">Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-160">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="036a9-161">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="036a9-161">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="036a9-162">Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-162">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="036a9-163">I partner comunicano a Microsoft gli account dei clienti con sottoscrizioni di Azure pronti per la migrazione e forniscono i nomi dell'azienda dei clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-163">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="036a9-164">Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-164">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="036a9-165">Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="036a9-165">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="036a9-166">Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="036a9-166">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="036a9-167">**Nota** La disabilitazione delle sottoscrizioni per il cliente non cambia l'aspetto del cliente nell'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-167">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="036a9-168">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="036a9-168">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="036a9-169">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="036a9-169">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="036a9-170">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-170">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="036a9-171">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-171">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="036a9-172">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="036a9-172">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="036a9-173">Note</span><span class="sxs-lookup"><span data-stu-id="036a9-173">Notes</span></span>

-   <span data-ttu-id="036a9-174">Disabilitare la sottoscrizione dall'account CSP di **origine della transizione** non influisce sul servizio del cliente finale, a condizione che il provisioning del servizio sia stato eseguito dall'account CSP di **destinazione della transizione** prima della disabilitazione.</span><span class="sxs-lookup"><span data-stu-id="036a9-174">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="036a9-175">Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.</span><span class="sxs-lookup"><span data-stu-id="036a9-175">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="036a9-176">Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-176">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="036a9-177">**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni.</span><span class="sxs-lookup"><span data-stu-id="036a9-177">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="036a9-178">Microsoft non supporterà le richieste di accrediti causate da eventuali sovrapposizioni nella fatturazione dovute alla mancata sospensione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="036a9-178">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="036a9-179">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="036a9-179">Simplify migration using Export</span></span>

<span data-ttu-id="036a9-180">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="036a9-180">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="036a9-181">Fai clic su **Clienti** nel tuo dashboard per visualizzare l'elenco dei clienti nella struttura esistente.</span><span class="sxs-lookup"><span data-stu-id="036a9-181">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="036a9-182">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="036a9-182">Open the desired customer name.</span></span>

3.  <span data-ttu-id="036a9-183">Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="036a9-183">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="036a9-184">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="036a9-184">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="036a9-185">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="036a9-185">API registration</span></span>

<span data-ttu-id="036a9-186">Per altre informazioni sulla registrazione dell'API, [vedi questa pagina](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="036a9-186">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="036a9-187">Log attività del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="036a9-187">Partner Center Activity log</span></span>


<span data-ttu-id="036a9-188">Con il log attività i partner possono visualizzare un record di tutte le modifiche effettuate nel loro tenant con effetti sui clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-188">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="036a9-189">Queste informazioni sono utili per tenere traccia delle modifiche apportate nel tenant di un cliente.</span><span class="sxs-lookup"><span data-stu-id="036a9-189">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="036a9-190">Visualizzare il log attività</span><span class="sxs-lookup"><span data-stu-id="036a9-190">View the Activity log</span></span>**

1.  <span data-ttu-id="036a9-191">Dal dashboard del Centro per i partner fai clic su link **Log attività**.</span><span class="sxs-lookup"><span data-stu-id="036a9-191">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="036a9-192">Nella pagina **Log attività** visualizza le modifiche apportate agli account dei clienti.</span><span class="sxs-lookup"><span data-stu-id="036a9-192">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="036a9-193">Per filtrare il log attività in base alla data, seleziona l'intervallo desiderato in **da** e **a** per limitare i record selezionati nel log.</span><span class="sxs-lookup"><span data-stu-id="036a9-193">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="036a9-194">Per filtrare in base al cliente, usa la casella di ricerca nella pagina **Log attività**.</span><span class="sxs-lookup"><span data-stu-id="036a9-194">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="036a9-195">Esportare il log attività</span><span class="sxs-lookup"><span data-stu-id="036a9-195">Export the Activity log</span></span>**

-   <span data-ttu-id="036a9-196">Fai clic su **Esporta log** per esportare i dati del log attività in un file CSV.</span><span class="sxs-lookup"><span data-stu-id="036a9-196">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="036a9-197">Puoi anche esportare l'elenco dei clienti e l'elenco delle sottoscrizioni di un singolo cliente (dalla pagina delle sottoscrizioni del cliente).</span><span class="sxs-lookup"><span data-stu-id="036a9-197">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



