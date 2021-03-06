---
title: Tipi di addebito file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 01/06/2020
description: Tipi di addebiti (basati su licenza, utilizzo e una volta), crediti e sconti sui file di riconciliazione del centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716872"
---
# <a name="understand-charge-types"></a>Informazioni sui tipi di addebito

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale

In questo argomento vengono descritti i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere presenti nel file di riconciliazione. La fattura fornisce un riepilogo degli addebiti. Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di elementi riga, inclusi i tipi di addebito. Per ulteriori informazioni sui file di riconciliazione, vedere [come utilizzare i file di riconciliazione](use-the-reconciliation-files.md).

Sia [i file di riconciliazione basati sull'utilizzo](usage-based-recon-files.md) che [i file di riconciliazione basati sulle licenze](license-based-recon-files.md) mostrano solo le transazioni e gli addebiti relativi all'utilizzo (unità utilizzate e addebiti correlati).

> [!NOTE]
> I crediti, gli sconti o i rimborsi unidirezionali visualizzati nella fattura come **modifiche** non vengono visualizzati nel file di riconciliazione.

## <a name="map-charge-types-to-invoice-charges"></a>Mappare i tipi di addebito ai costi fattura

Per fare riferimento incrociato agli importi tra la fattura e il file di riconciliazione, utilizzare le opzioni di filtro in Microsoft Excel. Filtrare in base ai tipi di addebito sul file di riconciliazione per eseguire il mapping degli addebiti per la fattura a un set di suddivisione dei costi nel file di riconciliazione

## <a name="license-based-charges"></a>Addebiti in base alle licenze

Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la colonna **Amount** del file basato su licenze.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Commissione di attivazione | Importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto. |
| Commissione di annullamento | Addebiti rivalutati per il cliente quando vengono modificate le postazioni associate. |
| Istanza di annullamento ripartita proporzionalmente | Addebiti rivalutati annullati quando al cliente con sottoscrizione mensile è stata sospesa la sottoscrizione e le postazioni associate sono state modificate nello stesso mese |
| Tariffa periodica | Addebiti periodici per una sottoscrizione. |
| Ripartizione dell'istanza del ciclo | Addebiti rivalutati dal cliente quando vengono modificate le postazioni associate. |
| Rateizza le tariffe in caso di annullamento | Rimborso proporzionale per la parte di servizio inutilizzata al momento dell'annullamento. |
| Tariffe propagate quando si esegue la conversione a partire dall'offerta corrente | Addebiti rivalutati dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale. |
| Tariffe della propagazione durante la conversione in una nuova offerta | Addebiti rivalutati dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale. |
| Ripartizione delle tariffe all'acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale. |
| Tariffa di acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile. |
| Rateizza la tariffa al rinnovo | Tariffe riordinate al rinnovo della sottoscrizione. |
| Tariffa di rinnovo | Addebito per il rinnovo di una sottoscrizione |
| Rateizza le tariffe all'attivazione | > tariffe rivalutate dall'attivazione fino alla fine del periodo di fatturazione. |

## <a name="one-time-charges"></a>Addebiti monouso

Per eseguire il mapping di questi addebiti monouso alla fattura, sommare la colonna **Amount** del file basato su licenze.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Nuova | Utilizzato quando viene creato un nuovo acquisto. |
| addQuantity | Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo un aumento. |
| removeQuantity | Utilizzato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo una riduzione. |
| Annulla | Utilizzato quando viene annullata una sottoscrizione. |
| Convert | Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato. |

## <a name="usage-charges"></a>Costi di utilizzo

Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Valuta la tariffa di utilizzo all'annullamento | Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente. |
| Valuta la tariffa di utilizzo per il ciclo corrente | Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente. |

### <a name="credits"></a>Crediti

Per eseguire il mapping di questi crediti alla fattura:

- Sommare il **TotalForCustomer** dal file basato sulle licenze.
- Sommare la colonna **PostTaxTotal** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Compensa una voce | Rimborso parziale o totale per una voce, incluse le imposte. |

### <a name="usage-based-discounts"></a>Sconti in base all'uso

Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Sconto attivazione | Sconto applicato quando la sottoscrizione è stata attivata. |
| Sconto ciclo | Sconto applicato agli addebiti periodici. |
| Sconto rinnovo | Sconto applicato quando la sottoscrizione è stata rinnovata. |
| Annulla sconto | Addebiti applicati quando gli sconti vengono annullati. |

### <a name="license-based-discounts"></a>Sconti in base alle licenze

Per eseguire il mapping degli sconti basati sulle licenze alla fattura, sommare la colonna **TotalOtherDiscount** del file basato su licenza.

*Gli sconti basati sulle licenze possono essere applicati a più tipi di addebito.*
