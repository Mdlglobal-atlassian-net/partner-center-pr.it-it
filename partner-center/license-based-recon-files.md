---
title: License-based reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand license-based reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 617b49556851a4d9999e6294d61d79c4fe1befa1
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389819"
---
# <a name="license-based-reconciliation-files"></a>File di riconciliazione in base alle licenze

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

To reconcile your changes against a customer's orders, compare the **Syndication_Partner_Subscription_Number** from the reconciliation file against the **Subscription ID** from Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Fields in license-based reconciliation files

| Column | Descrizione | Valore di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Unique identifier in GUID format for a specific billing entity. Not required for reconciliation. È lo stesso per tutte le righe. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerID | Unique Microsoft identifier for the customer in GUID format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. May be useful to identify the order when contacting support. Not used for reconciliation. | *566890604832738111* |
| SubscriptionID | Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. May be useful to identify the subscription when contacting support. Not used for reconciliation. *This value is not the same as the **Subscription ID** on the Partner Admin Console. Please see **SyndicationPartnerSubscriptionNumber** instead.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificatore univoco per le sottoscrizioni. A customer can have multiple subscriptions for the same plan. This column is important for reconciliation file analysis. This field maps to the **Subscription ID** in the Partner Admin Console. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferID | Unique offer identifier. Standard offer identifier, as defined in the price list. *This value does not match **Offer ID** from the price list. See **DurableOfferID** instead.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Unique durable offer identifier, as defined in the price list. *This value matches the **Offer ID** from the price list.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | The subscription start date. L'ora indicata è sempre l'inizio della giornata, le 0:00. This field is set to the day after the order was submitted. Used in conjunction with the **SubscriptionEndDate** to determine: if the customer is still within the first year of the subscription, or if the subscription has been renewed for the following year. | *2/1/2019 0:00* |
| SubscriptionEndDate | The subscription end date. L'ora indicata è sempre l'inizio della giornata, le 0:00. Either *12 months plus **x** days after the start date* to align with the partner's billing date or *12 months from the renewal date*. In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente. È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico. | *2/1/2019 0:00* |
| ChargeStartDate | Giorno di inizio degli addebiti. L'ora indicata è sempre l'inizio della giornata, le 0:00. Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/1/2019 0:00* |
| ChargeEndDate | Giorno di fine degli addebiti. L'ora indicata è sempre la fine della giornata, le 23:59. Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/28/2019 23:59* |
| ChargeType | The [type of charge](recon-file-charge-types.md) or adjustment. | See [charge types](recon-file-charge-types.md). |
| UnitPrice | Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto. Be sure this matches the information stored in your billing system during reconciliation. | *6.82* |
| Quantità | Numero di postazioni. Be sure this matches the information stored in your billing system during reconciliation. | *2* |
| Importo | Prezzo totale per la quantità. Used to check if the amount calculation matches how you calculate this value for your customers. | *13.32* |
| TotalOtherDiscount | Importo dello sconto applicato a questi addebiti. Product licenses included with a competency or MAPS, or new subscriptions eligible for an incentive, will also contain a discount amount in this column. | *2.32* |
| Subtotal | Totale al lordo delle imposte. Checks if your subtotal matches your expected total, in case of a discount. | *11* |
| Imposta | Tax amount charge. Based on your market's tax rules and specific circumstances. | *0* |
| TotalForCustomer | Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte. | *11* |
| Currency | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Check if it matches your first invoice. Check again after any major billing platform updates. | *EUR* |
| CustomerName | Customer's organization name, as reported in Partner Center. *Very important field for reconciling the invoice with your system information.* | *Test Customer A* |
| MPNID | MPN identifier of the CSP partner. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | MPN identifier of the reseller of record for the subscription. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Customer's domain name. Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* | *example.onmicrosoft.com* |
| SubscriptionName | Nome alternativo della sottoscrizione. If no nickname is specified, Partner Center uses the **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. (This is an identical field to **OfferName**.) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
