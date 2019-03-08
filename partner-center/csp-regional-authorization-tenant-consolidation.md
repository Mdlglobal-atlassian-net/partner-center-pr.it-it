---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: article
ms.date: 10/29/2018
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: migrazione dei clienti, provisioning, account tenant, consolidamento dei tenant
ms.localizationpriority: medium
ms.openlocfilehash: 183b5f518a57fdaf27badce5927a2ea09a5ec89c
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587554"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>Consolidamento dei tenant per l'autorizzazione regionale per CSP

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government


\[Alcune informazioni si riferiscono al prodotto non definitivo che può essere modificato sostanzialmente prima del rilascio in commercio. Microsoft non rilascia alcuna garanzia, espressa o implicita, relativamente alle informazioni fornite di seguito.\]

Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

**Nota** Devi conoscere tutte le sottoscrizioni e il numero di postazioni per i tuoi clienti di cui è stato eseguito il provisioning dagli account per la transizione. Nell'ambito del processo di migrazione, dovrai eseguire nuovamente il provisioning degli stessi esatti abbonamenti con lo stesso numero di postazioni nel nuovo account CSP centralizzato. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato. Il consolidamento dei tenant è una scelta del partner. Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente. Tieni presente che potrebbe essere richiesto anche l'intervento dei clienti.



## <a name="prepare-for-migration"></a>Prepararsi per la migrazione


-   Accedi per i **Centro per i Partner** con il **dedicata alla transizione** account (esistente) (quello passerà) e prendere nota di tutti i clienti e tutti i servizi di provisioning per i clienti.

![elenco dei clienti regionali](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti


1.  Accedi per i **Centro per i Partner** con il **dedicata alla transizione** (nuovo) dell'account (quello che stanno passando a) e passare all'elenco di clienti dal **clienti**.

2.  Seleziona Clienti.

3.  Fai cli su **Richiedi una relazione come rivenditore**. Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4.  **Azione del cliente:** Assicurarsi che ogni cliente active che si vuole eseguire la migrazione visita questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5.  Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

I clienti verranno visualizzati nell'elenco dei clienti del partner dopo l'invio del contratto, uno alla volta.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure


1.  Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.

2.  Dal **Centro per i Partner** selezionate **clienti**.

3.  Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.

4.  Fai clic su **Aggiungi sottoscrizione**.

5.  Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo. Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.

![elenco di clienti](images/regionalcustomer2.png)

6.  Fai clic su **Invia**.

I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.

Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.

Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.

**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni. Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione


La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1.  Accedi per il **Centro per i Partner** con il **in fase di transizione da** CSP di account e passare all'elenco di clienti.

2.  Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.
3.  Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.

 >[! **Nota**] sospensione della sottoscrizione assicura provochi una fatturazione non si verifica.



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5.  Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure


Nota che non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP in base all'uso di Azure come nel caso delle sottoscrizioni CSP di Office 365. Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1.  Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.
2.  I partner comunicano a Microsoft gli account dei clienti con sottoscrizioni di Azure pronti per la migrazione e forniscono i nomi dell'azienda dei clienti.
3.  Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.
4.  Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.
5.  Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.

>[! **Nota**] la disabilitazione di sottoscrizioni per il cliente non modifica l'aspetto del cliente nell'elenco di clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.



6.  Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="notes"></a>Note

-   Disabilitare la sottoscrizione dall'account CSP di **origine della transizione** non influisce sul servizio del cliente finale, a condizione che il provisioning del servizio sia stato eseguito dall'account CSP di **destinazione della transizione** prima della disabilitazione.

-   Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.

-   Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.

-   **Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni. Microsoft non supporterà le richieste di accrediti causate da eventuali sovrapposizioni nella fatturazione dovute alla mancata sospensione delle sottoscrizioni nell'**origine della transizione**.



### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1.  Fare clic su **clienti** nel centro per i Partner per visualizzare l'elenco di clienti in una struttura esistente.

2.  Apri il nome del cliente desiderato.

3.  Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.

4.  Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, [vedi questa pagina](https://go.microsoft.com/fwlink/?linkid=847990).








