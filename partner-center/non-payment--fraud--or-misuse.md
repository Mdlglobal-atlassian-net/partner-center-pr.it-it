---
title: Gestire insoluti, frodi o uso improprio
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: È importante conoscere i diversi rischi correlati alle transazioni online e le procedure consigliate per gestire e mitigare tali rischi.
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: frode, uso improprio, utilizzo accettabile, criteri di utilizzo accettabili, mancato pagamento, il cliente non pagherà fattura, rischi online, furto del servizio, abusi del servizio, Sospendi una sottoscrizione,
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 24a6d636ec4b0fb8aecc158f4750e471f1ca1a3a
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998447"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gestione di mancato pagamento, frode o uso improprio nel Centro per i partner

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**
- Amministratore globale
- Amministratore utenti
- Agente amministratore
- Amministratore fatturazione

L'utente è responsabile finanziario per gli acquisti fraudolenti da clienti e/o clienti che non hanno effettuato il pagamento dei servizi acquistati. Pertanto, si *consiglia di adottare i controlli di mitigazione dei rischi di rilevamento e prevenzione delle frodi*.

Per evitare e/o risolvere le attività fraudolente o l'utilizzo improprio, è importante comprendere i potenziali rischi e sviluppare criteri e procedure che possono ridurre l'esposizione.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Imposizione dei criteri di utilizzo accettabili di Microsoft

Se Microsoft rileva l'attività del partner o del cliente confermata o sospetta viola i criteri di utilizzo accettabili, verranno eseguiti i passaggi per l'applicazione. Il cliente potrebbe essere immediatamente sospeso. Si riceverà una notifica sulle azioni di imposizione o sull'aggiornamento delle richieste da Microsoft.

## <a name="abuse-of-service-risks"></a>Abuso dei rischi di servizio

L' **abuso dei** rischi per i servizi indica che i clienti che usano servizi cloud violano i criteri di utilizzo accettabili di Microsoft.

### <a name="examples-of-abuse-of-service"></a>Esempi di abusi del servizio

Esempi di queste violazioni dei criteri di utilizzo accettabili di Microsoft possono includere:

- Spamming
- Hacking
- Attacchi Denial of Service (DDoS) distribuiti
- Data mining Bitcoin
- Distribuzione malware
- Rivendita di sottoscrizioni Pirate

## <a name="theft-of-service-risks"></a>Furto dei rischi di servizio

Il **furto di** rischi per i servizi indica ai clienti che non hanno intenzione di pagare per i servizi usati. Questo furto può comportare l'utilizzo di strumenti di pagamento rubati, l'invio di informazioni di fatturazione false e/o l'impostazione predefinita di saldi in attesa.

### <a name="examples-of-service-theft"></a>Esempi di furto del servizio

Esempi di questi rischi per le transazioni online possono includere:

- Transazioni che non si verificano in persona (transazioni con carta di credito non presenti)
- Identità non rappresentate
- Servizi sottoposti a provisioning e utilizzati prima della ricezione del pagamento iniziale
- Mercati emergenti e/o aree ad alto rischio per frode online
- Automatizzare la creazione e l'acquisto di account da attori malintenzionati

## <a name="managing-online-risk"></a>Gestione dei rischi online

È possibile utilizzare i seguenti suggerimenti per sviluppare criteri e procedure per ridurre l'esposizione ai rischi per le transazioni online nel ciclo di vita delle relazioni dei clienti.

### <a name="onboarding-new-customers"></a>Onboarding di nuovi clienti

Suggerimenti per ridurre i rischi online quando il caricamento di nuovi clienti include:

- Stabilire relazioni personali con i clienti, se possibile, ad esempio contattando i clienti per telefono.
- Verificare le credenziali e i retroscena dei clienti tramite metodi migliori, ad esempio l'uso di uffici di credito o agenzie di report commerciali commerciali.
- Usare l'autenticazione a più fattori, ad esempio la verifica tramite SMS, durante l'iscrizione per ridurre al minimo l'esposizione alla creazione e all'acquisto di account robotizzati.
- Gestire e tenere traccia delle identità usando i servizi, ad esempio i servizi di identità digitali.
- Valutare la forza finanziaria dei clienti tramite sistemi di rilevamento illeciti di carte di credito rigorosi.
- Definire un criterio Clear Collections. Consente di illustrare in dettaglio il processo di raccolta e quando l'accesso alle sottoscrizioni sarà influenzato da un mancato pagamento. È possibile disabilitare l'accesso o [sospendere le sottoscrizioni di un cliente per il](suspend-a-subscription.md) mancato pagamento.

### <a name="managing-customer-accounts"></a>Gestione degli account cliente

I suggerimenti per la gestione degli account cliente dopo l'acquisto includono:

- Implementare un processo per ricevere, rivedere, agire in modo rapido e rispondere alle notifiche Microsoft.
- Collaborare con i clienti per comprendere le esigenze aziendali di utilizzo del cloud e le impostazioni appropriate per le soglie di monitoraggio. Ad esempio, è possibile [impostare un budget mensile per la spesa di Azure](set-an-azure-spending-budget-for-your-customers.md) nel centro per i partner. In questo modo è possibile monitorare l'utilizzo dei clienti durante il mese e ricevere una notifica quando i clienti si avvicinano al budget.
- Monitora regolarmente i [log attività del cliente](activity-logs.md) per aiutare a rilevare tempestivamente le frodi.
- Eseguire un'azione rapida quando vengono rilevate attività sospette.
- Evitare di concedere ai clienti l'accesso amministrativo completo alle sottoscrizioni senza prima implementare i controlli di mitigazione dei rischi.

### <a name="managing-customer-billing"></a>Gestione della fatturazione dei clienti

I suggerimenti per la gestione della fatturazione del cliente dopo l'acquisto includono:

- Richiedere i prepagamenti prima delle transazioni e della fatturazione iniziali.
- Non accettare strumenti di pagamento ad alto rischio (ad esempio carte prepagate o schede con valori archiviati).
- Monitorare i pagamenti dei clienti e l'invecchiamento degli account. Applicare in modo aggressivo i processi di Dunning standardizzati per i pagamenti tardivi o il mancato pagamento.

Per strategie più dettagliate per attenuare i rischi online, vedere la guida alla gestione dei rischi per le [transazioni online.](https://assets.windowsphone.com/7d885238-e13b-4f10-a682-3d5adacd2859/CSP-PartnerRiskGuide-APSFinal_InvariantCulture_Default.zip)
