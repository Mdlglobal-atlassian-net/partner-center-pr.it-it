---
title: Creare account utente e impostare le autorizzazioni | Centro partner
description: L'amministratore crea un account utente per ogni dipendente del partner che deve accedere al Centro per i partner.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
Keywords: roles, permissions,add user, assign role, admin, agent,
ms.openlocfilehash: 8c29fecf1d630021a58973e0e8e0e9844dac04e0
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/08/2018
---
# <a name="create-user-accounts-and-assign-permissions"></a>Creare account utente e assegnare le autorizzazioni

**Si applica a**

-  Centro per i partner

Creare gli account utente per i dipendenti che richiedono l'accesso al dashboard del partner. Queste attività devono essere eseguite da un amministratore con autorizzazioni di amministratore per la gestione degli utenti. 

>**Nota**<br> Ora hai la possibilità di assegnare gli utenti a tre nuovi ruoli nel dashboard del partner che consentono di gestire l'azienda: amministratore MPN, amministratore del profilo di lavoro e amministratore delle segnalazioni. Vedi di seguito Assegnare le autorizzazioni utente per i dettagli su ogni ruolo.


## <a name="add-a-new-user"></a>Aggiungere un nuovo utente

1. Seleziona **Gestione utenti** dal menu **Impostazioni**.

2.  Seleziona **Aggiungi utente**.

3.  Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.

4.  Seleziona il tipo di agente e/o il tipo di amministratore da assegnare all'utente. L'accesso al dashboard del partner è basato sui ruoli, pertanto puoi assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche. Per altre informazioni sulle operazioni possibili con ciascun ruolo, vedi di seguito Assegnare le autorizzazioni utente.

5.  Seleziona **Aggiungi** per creare l'account utente. Verifica i dettagli dell'utente nella pagina successiva.

>**Importante**<br>
Prendi nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina. Copiale e inviale al nuovo utente perché dopo non potrai più accedervi. 

L'utente dovrà accedere al dashboard del partner con il nome utente e la password temporanea. Quando l'utente accede al dashboard del partner per la prima volta, gli viene chiesto di modificare la password. 

>**Nota**<br> Se l'amministratore globale ha lasciato l'organizzazione o ha un altro ruolo ed è necessario aggiungere un nuovo amministratore globale, devi registrare una richiesta di assistenza nel [portale MPN](https://partner.microsoft.com/support). Se il richiedente è in grado di fornire le informazioni di identità personale richieste e altre informazioni sull'organizzazione, l'agente del supporto può richiedere l'elevazione dei privilegi di un utente ad amministratore globale.

## <a name="assign-user-permissions"></a>Assegnare le autorizzazioni utente

L'accesso al dashboard del partner è basato sui ruoli. Pertanto le autorizzazioni che assegni a un utente personalizzano la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le sue attività specifiche. 

Per ogni utente, devi assegnare almeno un livello di autorizzazione. Uno di questi livelli può essere il livello predefinito, ossia **Gestisce l'account della tua organizzazione come**. Se non assegni un ruolo, l'utente non sarà in grado di utilizzare il dashboard del partner.

-   Le autorizzazioni dell'agente controllano il tipo di dati dei clienti e le informazioni sull'account che l'utente può visualizzare e modificare.

-   Le autorizzazioni di amministratore controllano il livello di accesso che l'utente ha alle funzionalità del dashboard del partner. Questa impostazione ha un impatto al di fuori del dashboard del partner. Ad esempio, un amministratore della fatturazione può accedere alle fatture per tutti i servizi Microsoft, inclusi quelli che non riguardano CSP. Allo stesso modo, un amministratore globale può accedere agli account utente e dei clienti, inclusi quelli relativi a servizi diversi da CSP.

Le categorie generali dei ruoli sono: 

- Ruoli di amministratore
- Ruoli di agente
- Ruoli di incentivi
- Ruoli di riferimento e marketing

All'interno di ognuna di queste categorie generali, un utente può avere un solo ruolo, ma lo stesso utente può avere ruoli nelle altre categorie generali. 

>**Importante** Se per un utente non è necessario un ruolo specifico, lascia la designazione sull'impostazione predefinita **Gestisce l'account dell'organizzazione come**. Gli utenti devono essere assegnati ad almeno un ruolo per utilizzare il dashboard del partner.

La tabella seguente illustra le operazioni che ogni ruolo può eseguire nel dashboard del partner. Quando devi assegnare i ruoli, prendi in considerazione il lavoro eseguito dall'utente all'interno dell'organizzazione. Potrebbe ad esempio essere opportuno che l'amministratore globale sia anche l'agente amministratore. La persona che gestisce l'attività di marketing potrebbe anche gestire il profilo di lavoro.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Ruolo nel dashboard del partner</strong></p></td>
<td><p><strong>Operazioni consentite</strong></p></td>
</tr>
<tr class="odd">
<td><p><strong>Amministratore globale</strong></p></td>
<td><ul>
<li><p>Accesso a tutti gli account/servizi Microsoft con privilegi completi</p></li>
<li><p>Creazione di ticket di supporto per il dashboard del partner</p></li>
<li><p>Visualizzazione di contratti, listini prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Visualizzazione, creazione e gestione di utenti partner</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Amministratore fatturazione</strong></p></td>
<td><ul>
<li><p>Accesso a tutte le fatture di Microsoft con privilegi completi</p></li>
<li><p>Visualizzazione di contratti, listini prezzi e offerte</p></li>
<li><p>Fatturazione</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Amministratore gestione utenti</strong></p></td>
<td><ul>
<li><p>Visualizzazione, creazione e gestione di utenti</p></li>
<li><p>Visualizzazione di tutti i profili dei partner</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Amministratore profilo di lavoro</strong></p></td>
<td><ul>
<li><p>Visualizzazione, creazione e gestione del profilo di lavoro  </p></li>
<li><p>Visualizzazione, creazione e gestione delle richieste del servizio per i partner</p></li>
</ul></td>
<tr class="odd">
<td><p><strong>Amministratore dei riferimenti </strong></p></td>
<td><ul>
<li><p>Visualizzazione, creazione e gestione dei profili di lavoro</p></li>
<li><p>Ricezione e gestione dei riferimenti</p></li>
<li><p>Visualizzazione, creazione e gestione delle richieste del servizio per i partner</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Amministratore dei partner MPN</strong></p></td>
<td><ul>
<li><p>Visualizzazione, creazione e gestione delle richieste del servizio per i partner</p></li>
<li><p>Visualizzazione dei profili MPN, di lavoro, dell'organizzazione e legali</p></li>
<li><p>Visualizzazione dei dettagli dell'utente e i relativi dati delle competenze</p></li>
<li><p>Visualizzazione delle competenze</p></li>
<li><p>Visualizzazione e gestione dei benefit</p></li>
<li><p>Visualizzazione e acquisto di offerte MPN</p></li>
<li><p>Visualizzazione di fatture e cronologia degli ordini di offerte MPN </p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente amministratore</strong></p></td>
<td><ul>
<li><p>Gestione dei clienti</p></li>
<li><p>Aggiunta dell'elenco dei dispositivi al dashboard del partner</p></li>
<p><li>Creazione e applicazione di profili ai dispositivi</p></li>
<li><p>Gestione delle sottoscrizioni</p></li>
<li><p>Assistenza alle richieste di integrità e di servizio per i clienti</p></li>
<li><p>Richiesta dei privilegi di amministrazione delegati</p></li>
<li><p>Visualizzazione dei prezzi e delle offerte</p></li>
<li><p>Fatturazione</p></li>
<li><p>Amministrazione per conto di un cliente</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente di vendita</strong></p></td>
<td><ul>
<li><p>Gestione dei clienti</p></li>
<li><p>Aggiunta dell'elenco dei dispositivi al dashboard del partner</p></li>
<li><p>Gestione delle sottoscrizioni</p></li>
<li><p>Visualizzazione dei ticket di supporto</p></li>
<li><p>Richiesta di una relazione con un cliente</p></li>
<li><p>Gestione dei lead dei clienti</p></li>
<li><p>Visualizzazione del contratto per il cliente</p></li>
<li><p>Registrazione di un rivenditore a valore aggiunto</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente help desk</strong></p></td>
<td><ul>
<li><p>Ricerca e visualizzazione di un cliente</p></li>
<li><p>Modifica dei dettagli dei clienti</p></li>
<li><p>Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o sottoscrizioni</p></li>
<li><p>Richiesta di supporto per conto dei clienti (Nota: è necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)</p></li>
<li><p>Gestione delle sottoscrizioni e dei servizi per conto dei clienti (Nota: è necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)</p></li>
</ul></td>
</tr>
 

 

 



