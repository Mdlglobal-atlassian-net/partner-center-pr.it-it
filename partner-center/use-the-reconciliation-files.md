---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
description: Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343464"
---
# <a name="use-the-reconciliation-files"></a>Usare i file di riconciliazione

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government


Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner. I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.

## <a name="formatting-issues"></a>Problemi di formattazione

In alcuni casi il file di riconoscimento potrà avere problemi di formattazione. (Questa situazione può verificarsi, ad esempio, se non viene utilizzata le impostazioni locali EN-US.) Attenersi alla procedura seguente per risolvere questi problemi. 

<ol>
<li>Aprire il file con estensione csv in Excel e selezionare la prima colonna. Sulla barra multifunzione, selezionare <strong>dati</strong>, quindi selezionare <strong>testo alle colonne</strong>.</li>

<li>La conversione guidata testo in colonne, selezionare <strong>tipo di file delimitati</strong>e quindi selezionare <strong>successivo</strong>.</li> 

<li>Nel campo Delimeters, selezionare <strong>virgole</strong>. Se <strong>scheda</strong> è già selezionata, è possibile lasciarla. Selezionare <strong>Avanti</strong>.</li>

<li>Nel campo formato dei dati di colonna, selezionare <strong>data: MDY</strong>, quindi selezionare <strong>successivo</strong>.</li> 

<li>Nel campo formato dei dati di colonna, selezionare <strong>testo</strong> per tutte le colonne e quindi selezionare l'importo <strong>fine</strong>.</li>
</ol>

## <a name="downloading-a-large-recon-file"></a>Download di un file di riconoscimento di grandi dimensioni

File di riconoscimento possono raggiungere dimensioni molto grandi e sono talvolta difficili da scaricare. Per uno script di PowerShell scaricare i file di grandi dimensioni riconoscimento, vedere [voci della fattura Get](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).

## <a href="" id="itemizebypartner"></a>Specificare i dettagli da partner


I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>ID MPN</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>ID MPN</td>
<td><p>ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</p></td>
</tr>
<tr class="even">
<td>ID MPN rivenditore</td>
<td><p>Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</p>
<p>ID MPN del rivenditore nel record per la sottoscrizione. Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</p>
<p>eTo visualizzare o aggiornare il rivenditore, dal menu Centro per i Partner, selezionare <strong>clienti</strong>, quindi scegliere il cliente dall'elenco. Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco. Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</p>
<p>Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</p>
<p>Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</p>
<p>Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> Campi del file basati su licenza


Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonna</strong></td>
<td><strong>Descrizione</strong></td>
<td><strong>Valore di esempio</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>Identificatore univoco per un'entità di fatturazione specifica, in formato GUID. Non è necessario per la riconciliazione, ma può risultare utile. È lo stesso per tutte le righe.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p>
<p>Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner. Vedi Syndication_Partner_Subscription_Number.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>Identificatore univoco per le sottoscrizioni. Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</p>
<p>Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>ID univoco dell'offerta. ID dell'offerta standard in base al listino prezzi.</p>
<p><b>Nota</b>: Questo valore non corrisponde ID offerta dall'elenco prezzi. Vedi DurableOfferID di seguito.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID dell'offerta durevole univoco, come definito nel listino prezzi.</p>
<p><b>Nota</b>: Questo valore corrisponde all'ID dell'offerta dall'elenco prezzi.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</p></td>
<td>Microsoft Office 365 (Piano E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine. Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>La data di fine sottoscrizione: 12 mesi + x giorni dopo la data di inizio (in modo da allinearsi partner data di fatturazione) o 12 mesi dalla data di rinnovo.</p>
<p>In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente. È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Giorno di inizio degli addebiti.</p>
<p>Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Giorno di fine degli addebiti.</p>
<p>Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</p>
<p>L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Tipo di addebito o rettifica. Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
<td><p>Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantità</td>
<td><p>Numero di postazioni. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Importo</td>
<td><p>Prezzo totale per la quantità. Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Importo dello sconto applicato a questi addebiti. IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>Totale al lordo delle imposte. Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Imposta</td>
<td><p>Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Cliente&#39;nome organizzazione s come riportato nel centro per i Partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema.</p></td>
<td>Cliente di prova A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID MPN del partner CSP</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione. Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Cliente&#39;nome di dominio s, usato per identificare il cliente. Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365. Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Nome alternativo della sottoscrizione. Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</p></td>
<td>PROGETTO ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questo è un campo identico a Nome offerta.</p></td>
<td>PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Campi del file basato sull'utilizzo


Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.

I campi seguenti illustrano quali servizi sono stati usati e la tariffa.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonna</strong></td>
<td><strong>Descrizione</strong></td>
<td><strong>Valore di esempio</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>ID del partner, in formato GUID.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Nome partner.</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>ID account partner.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Cliente&#39;nome organizzazione s come riportato nel centro per i Partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema.</p></td>
<td>Cliente di prova A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID MPN del partner CSP.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione. Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Numero di fattura in cui viene visualizzata la transazione specificata.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</p>
<p>L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p>
<p>Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Nome alternativo dell'offerta di servizio.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Line-of-business dell'offerta di servizio</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>Nome del servizio di Azure in questione.</p></td>
<td>MACCHINE VIRTUALI</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Tipo specifico di servizio di Microsoft Azure.</p></td>
<td><ul>
<li>Service Bus – Individual o Pack</li>
<li>SQL Azure database – Business o Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Resource Name</td>
<td><p>Nome della risorsa Azure.</p></td>
<td><ul>
<li>Data Transfer In (GB)</li>
<li>Data Transfer Out (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>Area geografica a cui si applica l'uso. Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</p></td>
<td>Asia Pacifico, Europa, America Latina, America del Nord</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>Identificatore univoco MSFT per l'offerta</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione. Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</p>
<p>Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Unità incluse nell'ambito dell'offerta. In genere non presente in CSP.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</p>
<p>Uguale a ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Totale al netto delle imposte, se le imposte sono applicabili.</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Prezzo unitario prima dell'applicazione delle imposte. Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Prezzo unitario dopo l'applicazione delle imposte. Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Tipo di addebito o rettifica. Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
<td><p>Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>ID account univoco nella piattaforma di fatturazione MSFT.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Data di distribuzione del servizio.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</p></td>
<td>East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name. I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name. La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</p></td>
<td>AccessControl, CDN, Compute, Database, ServiceBus, Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</p></td>
<td>EXTERNAL</td>
</tr>
<tr class="even">
<td>Project</td>
<td><p>Nome definito dal cliente per l'istanza del servizio</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</p></td>
<td>Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days". Se disponi di un pacchetto 25 di connessioni del bus di servizio eseguito il provisioning e si fosse utilizzato 1 durante il giorno, l'istruzione di utilizzo giornaliero per quel giorno indicherebbe "25 connessioni / 30 giorni: utilizzato: 1.000000”.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Cliente&#39;nome di dominio s, usato per identificare il cliente. Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>Unità</td>
<td><p>Nome dell'unità della risorsa</p></td>
<td>GB o ORE</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>Campi del file sia monouso che ricorrenti

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerId</td>
<td><p>Identificatore univoco tenant di Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID. Non è necessario per la riconciliazione, ma può risultare utile. È lo stesso per tutte le righe.</p></td>
</tr>

<tr class="even">
<td>Id cliente</td>
<td><p>Microsoft Azure Active Directory tenant ID univoco, in formato GUID, usato per identificare il cliente.</p></td>
</tr>

<tr class="odd">
<td>Nome cliente</td>
<td><p>Nome dell'organizzazione del cliente registrato nel Centro per i partner.</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>Nome di dominio del cliente, usato per identificare il cliente. Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365. Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</p></td>
</tr>

<tr class="odd">
<td>Paese del cliente</td>
<td><p>Paese in cui si trova il cliente.</p></td>
</tr>

<tr class="even">
<td>Numero fattura</td>
<td><p>Numero di fattura in cui viene visualizzata la transazione specificata.</p></td>
</tr>

<tr class="odd">
<td>MpnId</td>
<td><p>ID MPN del partner CSP.</p></td>
</tr>

<tr class="even">
<td>MpnId rivenditore</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione.</p></td>
</tr>

<tr class="odd">
<td>ID ordine</td>
<td><p>Identificatore univoco per un ordine in cui la piattaforma di e-commerce di Microsoft. Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p></td>
</tr>

<tr class="even">
<td>Data ordine</td>
<td><p>Data di effettuazione dell'ordine.</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>ID del prodotto.</p></td>
</tr>

<tr class="even">
<td>SkuId</td>
<td><p>ID di una SKU particolare.</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>ID di una disponibilità particolare. "Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</p></td>
</tr>

<tr class="even">
<td>Nome SKU</td>
<td><p>Titolo di una particolare SKU.</p></td>
</tr>

<tr class="odd">
<td>Nome prodotto</td>
<td><p>Nome del prodotto.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Il nome del server di pubblicazione del prodotto.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>ID univoco per questo server di pubblicazione.</p></td>
</tr>

<tr class="even">
<td>Descrizione della sottoscrizione</td>
<td><p>Nome descrittivo di una sottoscrizione.</p></td>
</tr>

<tr class="odd">
<td>ID sottoscrizione</td>
<td><p>Identificatore univoco per una sottoscrizione nella piattaforma Microsoft e-commerce. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione. Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Giorno di inizio degli addebiti. L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Giorno di fine degli addebiti. L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
</tr>

<tr class="even">
<td>Periodo di validità e Billingcycle</td>
<td><p>La durata del periodo e ciclo di fatturazione per l'acquisto. Ad esempio, "1 anno, mese."</p></td>
</tr>

<tr class="odd">
<td>Tipo di addebito</td>
<td><p>Tipo di addebito o rettifica.</p></td>
</tr>

<tr class="even">
<td>Prezzo unitario</td>
<td><p>Il prezzo come pubblicato nel listino prezzi dei contratti al momento dell'acquisto. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
</tr>

<tr class="odd">
<td>Prezzo unitario efficace</td>
<td><p>Il prezzo unitario dopo che sono state apportate modifiche.</p></td>
</tr>

<tr class="even">
<td>Quantità</td>
<td><p>Numero di unità. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
</tr>

<tr class="odd">
<td>Tipo di unità</td>
<td><p>Il tipo di unità acquistate.</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>Spiegazione di eventuali sconti.</p></td>
</tr>

<tr class="odd">
<td>Subtotale</td>
<td><p>Totale al lordo delle imposte. Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</p></td>
</tr>

<tr class="even">
<td>Totale imposte</td>
<td><p>Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</p></td>
</tr>

<tr class="odd">
<td>Totale</td>
<td><p>Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte.</p></td>
</tr>

<tr class="even">
<td>Currency</td>
<td><p>Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</p></td>
</tr>

<tr class="odd">
<td>AlternateID</td>
<td><p>Un identificatore alternativo per un ID dell'ordine.</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>Campi del file classificati giornaliera dell'utilizzo


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Column</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerId</td>
<td><p>ID del partner, in formato GUID.</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>Nome partner.</p></td>
</tr>

<tr class="odd">
<td>CustomerId</td>
<td><p>ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>Nome dell'organizzazione del cliente registrato nel Centro per i partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema.</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>Nome di dominio del cliente. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class="even">
<td>Paese del cliente</td>
<td><p>Paese in cui si trova il cliente.</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>ID MPN del partner CSP.</p></td>
</tr>

<tr class="even">
<td>Rivenditore MPNID</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>Numero di fattura in cui viene visualizzata la transazione specificata. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>ID del prodotto.</p></td>
</tr>

<tr class="odd">
<td>SkuId</td>
<td><p>ID di una SKU particolare.</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>ID di una disponibilità particolare. "Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</p></td>
</tr>

<tr class="odd">
<td>Nome SKU</td>
<td><p>Titolo di una particolare SKU.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Il nome del server di pubblicazione.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>L'ID del server di pubblicazione, in formato GUID. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class=”even">
<td>Descrizione della sottoscrizione</td>
<td><p>Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questo è un campo identico a Nome offerta.</p></td>
</tr>

<tr class="odd">
<td>ID sottoscrizione</td>
<td><p>Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione. Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
</tr>

<tr class="even">
<td>Data di utilizzo</td>
<td><p>Data di utilizzo del servizio.</p></td>
</tr>

<tr class="odd">
<td>Tipo di misuratore</td>
<td><p>Tipo di misuratore.</p></td>
</tr>

<tr class="even">
<td>Categoria misuratore</td>
<td><p>Il servizio di primo livello per l'utilizzo.</p></td>
</tr>

<tr class="odd">
<td>Id contatore</td>
<td><p>L'ID del contatore in uso.</p></td>
</tr>

<tr class="even">
<td>Sottocategoria contatore</td>
<td><p>Tipo di servizio di Azure che possa influire sulla tariffa.</p></td>
</tr>

<tr class="odd">
<td>Nome contatore</td>
<td><p>L'unità di misura per il contatore utilizzato.</p></td>
</tr>

<tr class="even">
<td>Area contatore</td>
<td><p>Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</p></td>
</tr>

<tr class="odd">
<td>Unità</td>
<td><p>Unità di risorsa del nome.</p></td>
</tr>

<tr class="even">
<td>Quantità utilizzata</td>
<td><p>La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting. Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</p></td>
</tr>

<tr class="odd">
<td>Percorso della risorsa</td>
<td><p>Il Data Center in cui il contatore è in esecuzione.</p></td>
</tr>

<tr class="even">
<td>Servizio utilizzato</td>
<td><p>Il servizio della piattaforma Azure che è stato usato.</p></td>
</tr>

<tr class="odd">
<td>Gruppo di risorse</td>
<td><p>Il gruppo di risorse in cui è in esecuzione il contatore distribuito.</p></td>
</tr>

<tr class="even">
<td>URI della risorsa</td>
<td><p>L'URI della risorsa in uso.</p></td>
</tr>

<tr class="odd">
<td>Tipo di addebito</td>
<td><p>Tipo di addebito o rettifica. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class="even">
<td>Prezzo unitario</td>
<td><p>Prezzo per ciascuna licenza, come pubblicato nel listino prezzi dei contratti al momento dell'acquisto. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
</tr>

<tr class="odd">
<td>Quantità</td>
<td><p>Numero di licenze. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
</tr>

<tr class="even">
<td>Tipo di unità</td>
<td><p>Il tipo di unità che in cui viene addebitato il contatore. Non è disponibile per l'attività corrente.</p></td>
</tr>

<tr class="odd">
<td>La fatturazione pre fiscali</td>
<td><p>Quantità totale prima delle imposte.</p></td>
</tr>

<tr class="even">
<td>Valuta di fatturazione</td>
<td><p>La valuta nell'area geografica del cliente</p></td>
</tr>

<tr class="odd">
<td>Prezzo totale al lordo di imposte</td>
<td><p>Il piano tariffario prima dell'aggiunta delle imposte.</p></td>
</tr>

<tr class="even">
<td>Prezzi di valuta</td>
<td><p>La valuta nel prezzo di listino.</p></td>
</tr>

<tr class="odd">
<td>Informazioni servizio 1</td>
<td><p>Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</p></td>
</tr>

<tr class="even">
<td>Informazioni servizio 2</td>
<td><p>Campo legacy che acquisisce i metadati specifici del servizio facoltativo.</p></td>
</tr>

<tr class="odd">
<td>`Tags`</td>
<td><p>Tag che è assegnare a misuratore in ordine per raggruppare i record di fatturazione. Ad esempio, è possibile usare tag per distribuire i costi in base al reparto che utilizza il contatore.</p></td>
</tr>

<tr class="even">
<td>Informazioni aggiuntive</td>
<td><p>Eventuali informazioni aggiuntive non incluse in altre colonne.</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>Addebiti di mapping tra una fattura e i file di riconciliazione

La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.

Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.

I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati). Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.

Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione. 

<table>
<tbody>
<tr>
<td>
<p><strong>Descrizione di addebito della fattura</strong></p>
</td>
<td>
<p><strong>Descrizione di addebito file di riconciliazione (ChargeType colonna)</strong></p>
</td>
<td>
<p><strong>Che cos'è l'addebito?</strong></p>
</td>
<td>
<p><strong>Come è possibile associare queste ChargeTypes nella fattura?</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>Addebiti basati su licenza</strong></p>
</td>
<td>
<p>Commissione di attivazione</p>
</td>
<td>
<p>L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</p>
</td>
<td rowspan="10">
<p>Dal file in base alle licenze, somma la colonna <strong>Amount</strong></p>
</td>
</tr>
<tr>
<td>
<p>Commissione di annullamento</p>
</td>
<td>
<p>Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</p>
</td>
</tr>
<tr>
<td>
<p>Tariffa periodica</p>
</td>
<td>
<p>Addebiti periodici per una sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Istanza del ciclo rateizzata</p>
</td>
<td>
<p>Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza le tariffe in caso di annullamento</p>
</td>
<td>
<p>Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza le tariffe all'acquisto</p>
</td>
<td>
<p>Il tipo di addebito per una sottoscrizione quando si usa la fatturazione annua</p>
</td>
</tr>
<tr>
<td>
<p>Tariffa di acquisto</p>
</td>
<td>
<p>Il tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza la tariffa al rinnovo</p>
</td>
<td>
<p>Tariffe rateizzate al rinnovo della sottoscrizione</p>
</td>
</tr>
<tr>

<td>
<p>Tariffa di rinnovo</p>
</td>
<td>
<p>Addebito per il rinnovo di una sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza le tariffe all'attivazione</p>
</td>
<td>
<p>Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><strong>Spese una tantum</strong></p>

</td>
<td>
<p>Nuova</p>
</td>
<td>
<p>Utilizzato quando viene creato un nuovo acquisto</p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p>addQuantity</p>
</td>
<td>
<p>Usato in entrambi il rimborso dell'acquisto originale e la nuova quantità dopo l'aumento</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>removeQuantity</p>
</td>
<td>
<p>Usato in entrambi il rimborso dell'acquisto originale e la nuova quantità dopo la diminuzione</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Cancel</p>
</td>
<td>
<p>Utilizzato quando viene annullata una sottoscrizione</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Convertire</p>
</td>
<td>
<p>Utilizzato quando viene aggiornata una licenza, ma rimane invariato il numero di postazioni</p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><strong>Costi di utilizzo</strong></p>
</td>
<td>
<p>Valuta la tariffa di utilizzo all'annullamento</p>
</td>
<td>
<p>Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</p>
</td>
<td rowspan="2">
<p>Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Valuta la tariffa di utilizzo per il ciclo corrente</p>
</td>
<td>
<p>Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</p>
</td>
</tr>

<tr>
<td>
<p><strong>Crediti</strong></p>
</td>
<td>
<p>Compensa una voce</p>
</td>
<td>
<p>Rimborso parziale o totale per una voce, comprese le imposte</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></p>
<p>Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>Sconti basati sull'utilizzo</strong></p>
</td>
<td>
<p>Sconto attivazione</p>
</td>
<td>
<p>Sconto applicato all'attivazione della sottoscrizione</p>
</td>

<td rowspan="4">
<p>Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Sconto ciclo</p>
</td>
<td>
<p>Sconto applicato su addebiti periodici</p>
</td>
</tr>
<tr>
<td>
<p>Sconto rinnovo</p>
</td>
<td>
<p>Sconto applicato al rinnovo della sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Annulla sconto</p>
</td>
<td>
<p>Addebiti applicati all'annullamento degli sconti</p>
</td>
</tr>


<tr>
<td>
<p><strong>Sconti basati su licenza</strong></p>
</td>
<td>
<p><em>Può essere applicato a più tipi di costo</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></p>
</td>
<td>
<p><em>Può essere applicato a più tipi di costo</em></p>
<p><em>Eccezione: &quot;Offset di una voce&quot; include già le imposte. Vedere i crediti, sopra.</em></p>
</td>
<td>
<p>Imposte o imposte sul valore aggiunto (IVA)</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>Tax</strong></p>
<p>Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
