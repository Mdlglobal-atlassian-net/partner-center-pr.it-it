---
title: Leggere la fattura | Centro per i partner
description: "La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel dashboard del Centro per i partner."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: "fatturazione abbonamenti, fatturazione, fatturazione nel centro per i partner, centri per i partner fatturazione, leggere la fattura, fattura, fattura del centro per i partner, fattura CSP, dove è la fattura?"
ms.openlocfilehash: d24c9ad9ac90597c8e56843a25a69b9108c020d2
ms.sourcegitcommit: 2c99458586d7d536f5502317653eb4a43e2fdafc
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/10/2017
---
# <a name="read-your-bill"></a>Leggere la fattura

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Per la fatturazione, accedi al menu **Dashboard** e seleziona **Fatturazione** per visualizzare la cronologia e le tendenze della fatturazione, link al file di fatturazione e di riconciliazione e informazioni sull'ultimo pagamento.

I partner del programma Cloud Solution Provider che hanno scelto la fatturazione mensile pagheranno Microsoft per gli abbonamenti dei clienti (sia in base a licenza che in base all'uso) in via posticipata, dopo 60 giorni.

>**Nota**<br>
La fattura è un riepilogo di tutti gli addebiti relativi a programma, prodotti e clienti per il periodo di fatturazione corrente ed è disponibile entro quattro (4) giorni dalla data di fatturazione selezionata.


Per i dettagli sugli addebiti, consulta i file di riconciliazione associati. I file di riconciliazione includono gli ID dei clienti e gli ID delle sottoscrizioni che userai per creare le fatture per i clienti. Per altre informazioni, vedi [Come usare i file di riconciliazione](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definizioni del file di fatturazione


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Campo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>ID fiscale federale.</td>
</tr>
<tr class="odd">
<td>Numero cliente</td>
<td>Codice del cliente.</td>
</tr>
<tr class="even">
<td>Indirizzo fatturazione</td>
<td>Indirizzo a cui inviare la fattura. Per modificare questo indirizzo, vai a Impostazioni account > Profilo di fatturazione partner. </td>
</tr>
<tr class="odd">
<td>Addebiti periodici</td>
<td>Gli addebiti fissi mensili o annuali per le licenze in base all'uso acquistate, fatturati prima del servizio. Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</td>
</tr>
<tr class="even">
<td>Costi di utilizzo</td>
<td>Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il periodo di fatturazione. Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</td>
</tr>
<tr class="odd">
<td>Crediti e rettifiche</td>
<td>Crediti o rettifiche per modifiche apportate alle sottoscrizioni, ad esempio aumento o riduzione delle postazioni.</td>
</tr>
<tr class="even">
<td>Altri sconti</td>
<td>Ad esempio lo sconto che il cliente riceve sul prezzo normale della sottoscrizione. Lo sconto viene indicato come importo unico, non come prezzo per unità o licenza.</td>
</tr>
<tr class="odd">
<td>Imposte</td>
<td>Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti che fanno riferimento a:
<ul>
<li>la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</li>
<li>la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</li>
</ul></td>
</tr>
<tr class="even">
<td>Costi attuali totali</td>
<td>L'importo dovuto nella valuta della fattura per il periodo fatturato, da pagare entro la data di scadenza.</td>
</tr>
<tr class="odd">
<td>Istruzioni per il pagamento</td>
<td>Descrive come pagare la fattura, in base all'area geografica. Includi sempre il numero di fattura quando effettui un pagamento.</td>
</tr>
<tr class="even">
<td>N. fattura</td>
<td>Numero della fattura.</td>
</tr>
<tr class="odd">
<td>Periodo di fatturazione</td>
<td>I partner CSP ricevono una fattura mensile o annuale.</td>
</tr>
<tr class="even">
<td>Data fattura</td>
<td>Data in cui ricevi la fattura.</td>
</tr>
<tr class="odd">
<td>Data scadenza pagamento</td>
<td>Data entro cui effettuare il pagamento.</td>
</tr>
<tr class="even">
<td>Ordine d'acquisto del cliente</td>
<td>Il numero del tuo ordine di acquisto.</td>
</tr>
<tr class="odd">
<td>Servizio clienti</td>
<td>Indirizzo del sito Web per accedere al servizio clienti.</td>
</tr>
<tr class="even">
<td>Destinatario del servizio</td>
<td>Indirizzo in cui viene usato il servizio. (Questo è l'indirizzo legale della società associato alla verifica della società e non può essere modificato.)</td>
</tr>
</tbody>
</table>

 

 

 



