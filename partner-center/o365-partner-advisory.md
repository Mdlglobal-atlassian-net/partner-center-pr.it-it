---
title: Consulenza partner Office 365-Microsoft 365 Voice in CSP | Centro per i partner
description: I servizi PSTN in alcuni paesi possono essere soggetti a requisiti fiscali e normativi speciali che possono influenzare l'ordine e la fatturazione dei partner.
ms.topic: article
ms.date: 11/04/2019
author: maggiepuccievans
ms.author: evansma
keywords: Office, O365, servizi PSTN, imposte, requisiti, fattura, fatturazione
ms.localizationpriority: medium
ms.openlocfilehash: 2edf62c8a2157bc2b75855833ddbc7a63e7c6bb0
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005060"
---
# <a name="office-365-partner-advisory-microsoft-365-voice-in-csp"></a>Advisory per i partner di Office 365: Microsoft 365 Voice in CSP

**Si applica a**

- Centro per i partner  

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente amministratore

I servizi PSTN (Public Switched Telephone Network) in alcuni paesi potrebbero essere soggetti a requisiti fiscali e normativi speciali che possono influenzare l'ordine e la fatturazione dei partner.  In Stati Uniti, Puerto Rico e Canada, i servizi PSTN e Microsoft 365 Voice di Skype for business sono soggetti a requisiti fiscali e normativi specifici. Nei Stati Uniti e in Puerto Rico i servizi PSTN dei prezzi Microsoft sono inclusi nell'IVA.  Le tasse e le normative PSTN univoche influiranno sui partner di Office 365 che trasformano Microsoft 365 prodotti vocali.  Se un partner applica ricarichi al prezzo di un servizio PSTN Microsoft, potrebbe avere la responsabilità di calcolare e versare imposte e tariffe specifiche per i servizi PSTN.

## <a name="partner-recommendations"></a>Raccomandazioni per i partner

Rivolgersi ai consulenti fiscali e legali per informazioni sulle responsabilità dell'organizzazione in merito a normative, imposte e costi per i servizi PSTN e altre potenziali responsabilità.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Presentazione della fattura e file di riconciliazione partner

Le fatture CSP e i file di riconciliazione CSP nel Stati Uniti, Puerto Rico e Canada che includono Skype for business PSTN e Microsoft 365 Voice Services forniranno voci separate per i componenti PSTN e non PSTN.

Inoltre, le fatture CSP visualizzeranno la nota seguente:

* Il prezzo visualizzato è un addebito per i servizi di conferenza audio e del piano chiamante.  Tutte le imposte transazionali applicabili vengono addebitate esclusivamente sulla quantità indicata ad eccezione delle vendite effettuate all'interno del Stati Uniti.  Negli Stati Uniti il prezzo visualizzato è Tax inclusive, perché include un addebito per il piano di chiamata e i servizi di audioconferenza e un addebito per le imposte e i costi richiesti.  I servizi di conferenza audio e del piano di chiamata sono serviti dall'affiliato Microsoft autorizzato a fornirli.  Per informazioni dettagliate, vedere [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) .

## <a name="reconciliation-file-example"></a>Esempio di file di riconciliazione

Office 365 Enterprise E5 presenta il file di riconciliazione come due voci con nomi identici e ID identici, ma ogni elemento riga ha un prezzo unitario univoco (ad esempio: $28,40 e $2,00). Questo separa il componente Servizi di conferenza PST Skype for Business dell'offerta Office 365, in modo da poter applicare correttamente le imposte.

**Esempio di riconciliazione partner #1 (selezione colonne):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Tariffa periodica   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Tariffa periodica   |2,00   |

**Esempio di riconciliazione partner #2**

Microsoft 365 Business voce disponibile in Canada dispone di componenti impostabili PSTN aggiuntivi consolidati sulla fattura CSP (analogamente a Office 365 E5, vengono presentate due voci, una per i componenti PSTN e l'altra per i componenti non PSTN).  Il file di riconciliazione CSP per Microsoft 365 Business Voice visualizzerà tutti i componenti tassabili PSTN singolarmente (i singoli componenti PSTN non verranno consolidati in. CSV o strumento API).  La somma dei dettagli degli ordini e degli importi fatturati per i clienti trovati nel file di riconciliazione corrisponderà alla fattura CSP.

## <a name="additional-resources"></a>Risorse aggiuntive
Per ulteriori informazioni, visitare il sito [Microsoft 365 per partner](https://drumbeat.office.com/Pages/home2016.aspx) .

