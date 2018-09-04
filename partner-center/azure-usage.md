---
title: Ridimensionamento della macchina virtuale di Microsoft Azure per utilizzo della prenotazione massima | Dashboard del partner
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, prenotazioni, vm, gestire, utilizzo, ridimensionamento
ms.localizationpriority: medium
ms.openlocfilehash: bb7d022ba45462db313a9f4e16cc47e4550dbef6
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/31/2018
ms.locfileid: "2875781"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ridimensionamento della macchina virtuale Microsoft Azure per un utilizzo ottimale delle prenotazioni 

**Ambito di applicazione:**

-  Dashboard del partner
-  Portale di Azure
-  Partner di CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente 

Quando acquisti prenotazioni di Microsoft Azure per conto dei clienti, dovrai scegliere una macchina virtuale (VM) le cui dimensioni soddisfino le esigenze informatiche del cliente. Puoi trovare queste informazioni scegliendo uno dei metodi seguenti:

-   API di utilizzo Azure
-   Portale di Azure
-   Azure PowerShell
-   L'API di Azure Resource Manager (ARM)

Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito. Dopo aver acquistato una prenotazione, il relativo sconto verrà applicato automaticamente alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione. Non è necessario assegnare la prenotazione a una macchina virtuale.

>[!NOTE]
>Gli sconti relativi alla prenotazione non vengono applicati alle macchine virtuali classiche o promozionali.

>[!IMPORTANT]
>Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, dovrai utilizzare uno dei metodi descritti di seguito poiché la serie della macchina virtuale non viene visualizzata correttamente nei file di riconciliazione del Centro per i partner.


**Ottenere informazioni sul dimensionamento di una macchina virtuale mediante l'API di utilizzo di Azure**

1.  Utilizza il valore dell'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare. 

2.  Per altre informazioni, vedi [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nel [dashboard del Partner API](https://docs.microsoft.com/partner-center/develop/). 

**Ottenere informazioni sul dimensionamento di una macchina virtuale mediante il portale di Microsoft Azure**

1.  Nel dashboard del Partner, Vai alla pagina **i clienti** .

2.  Trova il cliente che desidera acquistare prenotazioni della macchina virtuale di Azure, quindi seleziona la freccia giù per espandere le informazioni del cliente. Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure. 

3.  Seleziona **Macchine virtuali** dal menu del portale, quindi seleziona la macchina virtuale per cui desideri acquistare una prenotazione. 

4.  Nella pagina dei dettagli della macchina virtuale, trova informazioni in merito a dimensioni e area geografica, come illustrato di seguito, e usa queste informazioni per acquistare la prenotazione nel Centro per i partner.  

    ![](images/usage1.png)

**Ottenere informazioni sul dimensionamento di una macchina virtuale mediante Microsoft Azure PowerShell**

Per ottenere la posizione e le dimensioni della macchina virtuale per cui desideri acquistare una prenotazione, utilizza le informazioni nell'immagine seguente. 

![](images/usage2.png)

**Ottenere informazioni sul dimensionamento di una macchina virtuale mediante l'API di Azure Resource Manager (ARM)**

1.  Tramite le API di ARMClient o ARM, chiama il client ARM per la macchina virtuale per cui desideri acquistare una prenotazione.

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  La chiamata restituisce valori per **vmSize** e **location**, come illustrato di seguito.

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificare lo sconto su prenotazione e utilizzo della macchina virtuale di Azure

Dopo l'acquisto di un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento anticipato dello spazio della macchina virtuale viene automaticamente applicato alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione del cliente. 

Puoi verificare l'utilizzo della prenotazione del cliente e vedere le macchine virtuali a cui sono applicati gli sconti relativi alla prenotazione utilizzando uno dei metodi seguenti:   

-   Portale di Azure
-   API di utilizzo di Azure

Le istruzioni per l'uso di ciascuno di questi metodi sono riportate di seguito.

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure

1.  Nel dashboard del Partner, Vai alla pagina **i clienti** .

2.  Trova il cliente di cui desideri verificare lo sconto e l'utilizzo della prenotazione, quindi seleziona la freccia giù per espandere le informazioni del cliente. Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure. 

3.  Seleziona **Prenotazioni** dal menu del portale, quindi seleziona la prenotazione di cui desideri verificare l'utilizzo. 

4.  Nella pagina **Panoramica** controlla il grafico sull'utilizzo della prenotazione, che mostra in che parte la prenotazione è stata applicata alle macchine virtuali. 

    >[!NOTE]
    >I dati di utilizzo possono essere ritardati fino a 8 ore.
    
    a.  Se l'utilizzo della prenotazione è pari al 100%, il cliente ottiene tutto il risparmio che l'acquisto della prenotazione è in grado di offrire. 
    
    b.  Se l'utilizzo della prenotazione è pari allo 0%, lo sconto non viene applicato a nessuna macchina virtuale. 
    
    c.  Se l'utilizzo della prenotazione è compreso tra 1% e 99%, esistono vantaggi inutilizzati. 

5.  Per evitare questa situazione, scegli la macchina virtuale delle dimensioni corrette per supportare le esigenze di elaborazione del cliente prima di effettuare l'acquisto.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra a quale macchina virtuale viene applicato lo sconto.  

Puoi ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente riceva lo sconto prenotazione e per vedere a quali macchine virtuali è applicato lo sconto. Confronta l'esempio A con l'esempio B per scoprire come verificare l'utilizzo della prenotazione di un cliente. 

![](images\usage5.png)

-   reservationId identifica la prenotazione di Azure utilizzata per applicare lo sconto alla macchina virtuale.
-   consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto della prenotazione.
-   ReservationMeter mostra un costo di $ 0 perché è stato applicato lo sconto prenotazione. 

Per ulteriori informazioni, vedi [Ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell'[API del Centro per i partner](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>I costi relativi al software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura. Tuttavia, se un cliente ha il vantaggio Azure Hybrid Use, i costi del software non verranno applicati. Per ulteriori informazioni, vedi [I costi del software Windows non sono inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure
|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere istanze di macchina virtuale riservate di Microsoft Azure](azure-reservations.md)
|Acquisto di prenotazioni di Azure per i clienti nel dashboard del Partner   |[Acquistare prenotazioni di Azure](azure-reservations-buying.md)
| La gestione di prenotazioni di Azure nel dashboard del Partner | [La gestione di prenotazioni di Azure nel dashboard del Partner](azure-reservations-manage.md)
|Acquisto di prenotazioni di Azure nel portale di Azure | [Pagare in anticipo per macchine virtuali con istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure |
|Gestione di prenotazioni di Azure nel portale di Azure   |[Gestire le istanze di macchina virtuale riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure  |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner



