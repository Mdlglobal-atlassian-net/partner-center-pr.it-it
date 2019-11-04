---
title: Stato dei requisiti di sicurezza per i partner | Centro per i partner
ms.date: 10/11/2019
description: Puoi rimanere sempre aggiornato sulla conformità della tua azienda ai requisiti MFA.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.openlocfilehash: 3ca0bcda7be69f0785207f29fbbab20d2402e780
ms.sourcegitcommit: 9dd6f1ee0ebc132442126340c9df8cf7e3e1d3ad
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/16/2019
ms.locfileid: "72425108"
---
# <a name="partner-security-requirements-status"></a><span data-ttu-id="a2210-104">Stato dei requisiti di sicurezza per i partner</span><span class="sxs-lookup"><span data-stu-id="a2210-104">Partner security requirements status</span></span>

<span data-ttu-id="a2210-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="a2210-105">**Applies to**</span></span>

- <span data-ttu-id="a2210-106">Tutti i partner nell'ambito del programma Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="a2210-106">All partners in the Cloud Solution Provider program</span></span>
  - <span data-ttu-id="a2210-107">Fatturazione diretta</span><span class="sxs-lookup"><span data-stu-id="a2210-107">Direct bill</span></span>
  - <span data-ttu-id="a2210-108">Provider indiretto</span><span class="sxs-lookup"><span data-stu-id="a2210-108">Indirect provider</span></span>
  - <span data-ttu-id="a2210-109">Rivenditore indiretto</span><span class="sxs-lookup"><span data-stu-id="a2210-109">Indirect reseller</span></span>
- <span data-ttu-id="a2210-110">Tutti i fornitori del pannello di controllo</span><span class="sxs-lookup"><span data-stu-id="a2210-110">All Control Panel Vendors</span></span>
- <span data-ttu-id="a2210-111">Tutti gli advisor</span><span class="sxs-lookup"><span data-stu-id="a2210-111">All Advisors</span></span>

<span data-ttu-id="a2210-112">Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti.</span><span class="sxs-lookup"><span data-stu-id="a2210-112">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="a2210-113">Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli.</span><span class="sxs-lookup"><span data-stu-id="a2210-113">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="a2210-114">Questo è il motivo per cui è necessario che tutti gli utenti nell'ecosistema agiscano e si assicurino di disporre di protezioni di sicurezza appropriate.</span><span class="sxs-lookup"><span data-stu-id="a2210-114">That is why we need everyone in our ecosystem to act and ensure they have appropriate security protections in place.</span></span> <span data-ttu-id="a2210-115">Per garantire la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori del pannello di controllo e i partner che partecipano al programma Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="a2210-115">To help safeguard partners and customers, we’re introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="a2210-116">A partire dal 1° agosto 2019 tutti i partner sono tenuti a implementare l'autenticazione a più fattori (MFA) per tutti gli utenti, inclusi gli account di servizio, nel tenant partner.</span><span class="sxs-lookup"><span data-stu-id="a2210-116">Starting August 1, 2019, all partners are required to enforce multi-factor authentication for all users, including service accounts, in their partner tenant.</span></span> <span data-ttu-id="a2210-117">Per informazioni più dettagliate sui nuovi criteri di sicurezza, vedi [Requisiti di sicurezza per i partner](partner-security-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="a2210-117">For more detailed information on the new security policies, read [Partner Security Requirements](partner-security-requirements.md).</span></span>

<span data-ttu-id="a2210-118">L'obiettivo è che ogni utente sia sottoposto a un test MFA per ogni singola autenticazione.</span><span class="sxs-lookup"><span data-stu-id="a2210-118">We want to ensure that each user has an MFA challenge for every single authentication.</span></span> <span data-ttu-id="a2210-119">Questo risultato può essere ottenuto in uno dei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="a2210-119">This can be accomplished through one of the following ways:</span></span>

- <span data-ttu-id="a2210-120">Implementazione di Azure AD Premium per fare in modo che l'autenticazione MFA venga applicata per ogni utente</span><span class="sxs-lookup"><span data-stu-id="a2210-120">Implementing Azure AD Premium to ensure that MFA is enforced for each user</span></span>
- <span data-ttu-id="a2210-121">Implementazione dei criteri di protezione di base</span><span class="sxs-lookup"><span data-stu-id="a2210-121">Implementing the baseline protection policies</span></span>
- <span data-ttu-id="a2210-122">Implementazione di una soluzione di terze parti in modo che l'autenticazione MFA venga applicata per ogni utente</span><span class="sxs-lookup"><span data-stu-id="a2210-122">Implementing a third-party solution to ensure MFA is enforced for each user</span></span>

## <a name="partner-security-requirements-status"></a><span data-ttu-id="a2210-123">Stato dei requisiti di sicurezza per i partner</span><span class="sxs-lookup"><span data-stu-id="a2210-123">Partner security requirements status</span></span>

<span data-ttu-id="a2210-124">Questo report può essere utile per verificare lo stato dei requisiti di sicurezza poiché consente di individuare i punti deboli.</span><span class="sxs-lookup"><span data-stu-id="a2210-124">This report can help you verify the security requirements status by providing a way to see where you might be falling short.</span></span> <span data-ttu-id="a2210-125">Il rilevamento viene aggiornato regolarmente.</span><span class="sxs-lookup"><span data-stu-id="a2210-125">The tracking is regularly updated.</span></span>

>[!NOTE]
><span data-ttu-id="a2210-126">Il report sullo stato dei requisiti di sicurezza per i partner è supportato solo nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2210-126">The Partner security requirements status report is supported only in Partner Center.</span></span> <span data-ttu-id="a2210-127">Non è disponibile in Microsoft Cloud for US Government o Microsoft Cloud Germania.</span><span class="sxs-lookup"><span data-stu-id="a2210-127">It’s not available in the Microsoft Cloud for US Government or Microsoft Cloud Germany.</span></span> <span data-ttu-id="a2210-128">È fortemente consigliabile che tutti i partner che effettuano transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) adottino immediatamente questi nuovi requisiti di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="a2210-128">We strongly recommend that all partners transacting through a sovereign cloud (21Vianet, US Government, and Germany) adopt these new security requirements immediately.</span></span> <span data-ttu-id="a2210-129">Tuttavia, non è necessario che questi partner soddisfino i nuovi requisiti di sicurezza con decorrenza a partire dal 1° agosto 2019.</span><span class="sxs-lookup"><span data-stu-id="a2210-129">However, these partners are not required to meet the new security requirements effective August 1, 2019.</span></span> <span data-ttu-id="a2210-130">Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.</span><span class="sxs-lookup"><span data-stu-id="a2210-130">Microsoft will provide additional details regarding the enforcement of these security requirements for sovereign clouds in the future.</span></span> 

<span data-ttu-id="a2210-131">Ogni volta che i tuoi dipendenti accedono al Centro per i partner per lavorare oppure, tramite le API, ricevono o inviano dati attraverso il Centro per i partner, il loro stato di sicurezza viene testato e monitorato.</span><span class="sxs-lookup"><span data-stu-id="a2210-131">Each time your employees sign in to Partner Center to work or, through APIs, get or send data through Partner Center, their security status is challenged and tracked.</span></span> <span data-ttu-id="a2210-132">Sono incluse nel rilevamento dello stato di sicurezza anche le tue applicazioni e tutte le applicazioni del fornitore del pannello di controllo.</span><span class="sxs-lookup"><span data-stu-id="a2210-132">Also included in security-status tracking, are your applications and any control panel vendor applications.</span></span> <span data-ttu-id="a2210-133">Lo stato visualizzato è relativo ai sette giorni precedenti.</span><span class="sxs-lookup"><span data-stu-id="a2210-133">The status displayed is for the previous 7 days.</span></span>

## <a name="multi-factor-authentication-mfa-report"></a><span data-ttu-id="a2210-134">Report sull'autenticazione a più fattori ("MFA")</span><span class="sxs-lookup"><span data-stu-id="a2210-134">Multi-factor authentication ("MFA") report</span></span>

<span data-ttu-id="a2210-135">Il report MFA del Centro per i partner offre informazioni dettagliate sull'implementazione dell'autenticazione MFA per partner fornendo due metriche basate sulle attività del Centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="a2210-135">The Partner Center MFA report offers insights into partner MFA implementation by providing two metrics based on Partner Center activities:</span></span>

<span data-ttu-id="a2210-136">**Verifica MFA completata dagli utenti**</span><span class="sxs-lookup"><span data-stu-id="a2210-136">**MFA verification completed by users**</span></span>

<span data-ttu-id="a2210-137">Questa metrica è correlata alle attività nel dashboard del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2210-137">This metric is related to activities within the Partner Center dashboard.</span></span> <span data-ttu-id="a2210-138">Misura la percentuale di operazioni eseguite dagli utenti che hanno completato la verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-138">It measures the percentage of operations made by users who have completed MFA verification.</span></span> <span data-ttu-id="a2210-139">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="a2210-139">For example:</span></span>

- <span data-ttu-id="a2210-140">Contoso è un partner CSP con due agenti di amministrazione, Jane e John.</span><span class="sxs-lookup"><span data-stu-id="a2210-140">Contoso is a CSP partner with two admin agents, Jane and John.</span></span>
- <span data-ttu-id="a2210-141">Il primo giorno Jane ha eseguito l'accesso al dashboard del Centro per i partner senza verifica MFA e ha effettuato tre operazioni.</span><span class="sxs-lookup"><span data-stu-id="a2210-141">On the first day, Jane logged in to Partner Center dashboard without MFA verification and made 3 operations.</span></span>
- <span data-ttu-id="a2210-142">Il secondo giorno John ha eseguito l'accesso al dashboard del Centro per i partner senza verifica MFA e ha effettuato cinque operazioni.</span><span class="sxs-lookup"><span data-stu-id="a2210-142">On the second day, John logged in to Partner Center dashboard without MFA verification and made 5 operations.</span></span>
- <span data-ttu-id="a2210-143">Il terzo giorno Jane ha eseguito l'accesso al dashboard del Centro per i partner con verifica MFA e ha effettuato due operazioni.</span><span class="sxs-lookup"><span data-stu-id="a2210-143">On the third day, Jane logged in to Partner Center dashboard with MFA verification and made 2 operations.</span></span>
- <span data-ttu-id="a2210-144">Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.</span><span class="sxs-lookup"><span data-stu-id="a2210-144">There were no operations made by either agent on the remaining 4 days.</span></span>
- <span data-ttu-id="a2210-145">Delle dieci operazioni effettuate nella finestra di sette giorni, sue sono state effettuate dall'utente con verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-145">Out of the 10 operations made in the 7-day window, 2 were made by user with MFA verification.</span></span> <span data-ttu-id="a2210-146">Di conseguenza, la metrica indica il 20%.</span><span class="sxs-lookup"><span data-stu-id="a2210-146">Hence, the metric shows 20%.</span></span>

<span data-ttu-id="a2210-147">**Autenticazione app+utente**</span><span class="sxs-lookup"><span data-stu-id="a2210-147">**App+User authentication**</span></span>

<span data-ttu-id="a2210-148">Questa metrica è correlata all'uso di richieste API del Centro per i partner effettuate con l'autenticazione app+utente.</span><span class="sxs-lookup"><span data-stu-id="a2210-148">This metric is related to the use of Partner Center API requests made using App+User authentication.</span></span> <span data-ttu-id="a2210-149">Misura la percentuale di richieste API effettuate usando un token di accesso con attestazione MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-149">It measures the percentage of API requests made using an access token with MFA claim.</span></span> <span data-ttu-id="a2210-150">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="a2210-150">For example:</span></span>

- <span data-ttu-id="a2210-151">Fabrikam è un partner CSP che dispone di un'applicazione CSP che usa una combinazione di autenticazione app+utente e di metodi di autenticazione basati solo su app.</span><span class="sxs-lookup"><span data-stu-id="a2210-151">Fabrikam is a CSP partner and has a CSP application that uses a mix of App+User authentication and app-only authentication methods.</span></span>
- <span data-ttu-id="a2210-152">Il primo giorno l'applicazione ha effettuato tre richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente senza verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-152">On the first day, the application made 3 API requests which were backed by an access token obtained through App+User authentication method without MFA verification.</span></span>
- <span data-ttu-id="a2210-153">Il secondo giorno l'applicazione ha effettuato cinque richieste API supportate da un token di accesso ottenuto usando l'autenticazione basata solo su app.</span><span class="sxs-lookup"><span data-stu-id="a2210-153">On the second day, the application made 5 API requests which were backed by an access token obtained using App-only authentication.</span></span>
- <span data-ttu-id="a2210-154">Il terzo giorno l'applicazione ha effettuato due richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente con verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-154">On the third day, the application made 2 API requests which were backed by an access token obtained using App+User authentication method with MFA verification.</span></span>
- <span data-ttu-id="a2210-155">Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.</span><span class="sxs-lookup"><span data-stu-id="a2210-155">There were no operations made by either agent on the remaining 4 days.</span></span>
- <span data-ttu-id="a2210-156">Le cinque richieste API nel secondo giorno supportate da un token di accesso ottenuto tramite l'autenticazione basata solo su app vengono omesse dalla metrica perché non usano le credenziali utente.</span><span class="sxs-lookup"><span data-stu-id="a2210-156">The 5 API requests on the second day which were backed by an access token obtained through App-only authentication are omitted from the metric since it does not make use of user credentials.</span></span> <span data-ttu-id="a2210-157">Delle cinque operazioni rimanenti, due sono state supportate da un token di accesso ottenuto con la verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-157">Out of the remaining 5 operations, 2 of them were backed by an access token obtained with MFA verification.</span></span> <span data-ttu-id="a2210-158">Di conseguenza, la metrica indica il 40%.</span><span class="sxs-lookup"><span data-stu-id="a2210-158">Hence, the metric shows 40%.</span></span>

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a><span data-ttu-id="a2210-159">Come procedere se le metriche nel report MFA non sono pari al 100%</span><span class="sxs-lookup"><span data-stu-id="a2210-159">What should I do if the metrics under MFA report aren't 100%</span></span>

<span data-ttu-id="a2210-160">È possibile che le metriche nel report MFA del Centro per i partner non siano pari al 100% per i partner che hanno implementato l'autenticazione MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-160">It is possible that the metrics under Partner Center MFA report may not be 100% for partners who have implemented MFA.</span></span> <span data-ttu-id="a2210-161">Per capire perché, di seguito sono riportati alcuni fattori di cui tenere conto.</span><span class="sxs-lookup"><span data-stu-id="a2210-161">To understand why, here are some factors to consider.</span></span>

> [!NOTE]
> <span data-ttu-id="a2210-162">Dovrai collaborare con una persona dell'organizzazione che abbia familiarità con la gestione delle identità e l'implementazione dell'autenticazione MFA per il tenant partner.</span><span class="sxs-lookup"><span data-stu-id="a2210-162">You will need to work with somebody from your organization who is familiar with identity management and MFA implementation for your partner tenant.</span></span>

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a><span data-ttu-id="a2210-163">Hai implementato l'autenticazione MFA per il tenant partner?</span><span class="sxs-lookup"><span data-stu-id="a2210-163">Have you implemented MFA for your partner tenant?</span></span>

<span data-ttu-id="a2210-164">In caso negativo, devi prima effettuare questa operazione.</span><span class="sxs-lookup"><span data-stu-id="a2210-164">If not, you need to implement MFA for your partner tenant first.</span></span> <span data-ttu-id="a2210-165">Per informazioni dettagliate su come implementare l'autenticazione MFA, vedi l'articolo [Requisiti di sicurezza per i partner](partner-security-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="a2210-165">For details on how to implement MFA, please refer to article [Partner Security Requirement](partner-security-requirements.md).</span></span>

### <a name="have-you-only-recently-completed-mfa-implementation"></a><span data-ttu-id="a2210-166">Hai completato l'implementazione dell'autenticazione MFA solo di recente?</span><span class="sxs-lookup"><span data-stu-id="a2210-166">Have you only recently completed MFA implementation?</span></span>

<span data-ttu-id="a2210-167">Le metriche vengono calcolate su base giornaliera e prendono in considerazione le operazioni eseguite negli ultimi sette giorni.</span><span class="sxs-lookup"><span data-stu-id="a2210-167">The metrics is calculated on a daily basis and takes into account operations performed in the last 7 days.</span></span> <span data-ttu-id="a2210-168">Se hai completato l'implementazione dell'autenticazione per il tenant partner solo di recente, è possibile che le metriche non siano pari al 100%.</span><span class="sxs-lookup"><span data-stu-id="a2210-168">If you only recently completed MFA implementation for your partner tenant, the metrics may not be 100%.</span></span>

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a><span data-ttu-id="a2210-169">Alcuni account utente sono stati esclusi dall'implementazione dell'autenticazione MFA?</span><span class="sxs-lookup"><span data-stu-id="a2210-169">Have some user accounts been excluded from MFA implementation?</span></span>

<span data-ttu-id="a2210-170">Verifica se l'implementazione dell'autenticazione MFA corrente copre tutti gli account utente o solo alcuni.</span><span class="sxs-lookup"><span data-stu-id="a2210-170">Understand whether your current MFA implementation covers all user accounts or only some.</span></span> <span data-ttu-id="a2210-171">Alcune soluzioni MFA sono basate su criteri e supportano l'esclusione degli utenti, mentre altre potrebbero richiedere l'abilitazione esplicita dell'autenticazione MFA in base ai singoli utenti.</span><span class="sxs-lookup"><span data-stu-id="a2210-171">Some MFA solutions are policy-based and supports user exclusion, while others might require you to explicitly enable MFA on a per-user basis.</span></span> <span data-ttu-id="a2210-172">Verifica di non aver escluso alcun utente dall'implementazione MFA corrente.</span><span class="sxs-lookup"><span data-stu-id="a2210-172">Verify you have not excluded any user from your current MFA implementation.</span></span> <span data-ttu-id="a2210-173">Eventuali account utente esclusi che eseguono l'accesso al Centro per i partner per eseguire un'attività correlata a CSP possono causare il mancato raggiungimento del 100% nelle metriche.</span><span class="sxs-lookup"><span data-stu-id="a2210-173">Any user account that is excluded and logs in to Partner Center to perform any CSP related activity can cause the metrics to not be 100%.</span></span>

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a><span data-ttu-id="a2210-174">L'autenticazione MFA è necessaria solo se vengono soddisfatte determinate condizioni?</span><span class="sxs-lookup"><span data-stu-id="a2210-174">Is MFA only required when certain conditions are met?</span></span>

<span data-ttu-id="a2210-175">Verifica se l'implementazione corrente applica l'autenticazione MFA solo in condizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="a2210-175">Understand whether current implementation only enforce MFA under specific conditions only.</span></span> <span data-ttu-id="a2210-176">Alcune soluzioni MFA presentano caratteristiche di flessibilità e consentono di applicare l'autenticazione MFA solo quando vengono soddisfatte determinate condizioni,</span><span class="sxs-lookup"><span data-stu-id="a2210-176">Some MFA solutions provide flexibility to only enforce MFA when certain conditions are met.</span></span> <span data-ttu-id="a2210-177">ad esempio un utente che accede da un dispositivo o da una posizione sconosciuta.</span><span class="sxs-lookup"><span data-stu-id="a2210-177">For example, user is accessing from unknown device or unknown location.</span></span> <span data-ttu-id="a2210-178">Un utente che è abilitato per l'autenticazione MFA, ma non è tenuto a completare la verifica MFA quando accede al Centro per i partner, può causare il mancato raggiungimento del 100% nelle metriche.</span><span class="sxs-lookup"><span data-stu-id="a2210-178">A user, who is enabled for MFA but isn't required to complete MFA verification when accessing Partner Center, can cause the metrics to not be 100%.</span></span>

>[!NOTE]
><span data-ttu-id="a2210-179">Per i partner che hanno implementato l'autenticazione MFA usando i criteri di base per la protezione dell'utente finale di Azure AD, è importante notare che la protezione dell'utente finale è un criterio basato sul rischio.</span><span class="sxs-lookup"><span data-stu-id="a2210-179">For partners who have implemented MFA using Azure AD End-User Protection baseline policy, it is important to note that End-User Protection is a risk-based policy.</span></span> <span data-ttu-id="a2210-180">Agli utenti coperti dal criterio verrà chiesto di eseguire l'autenticazione MFA solo durante tentativi di accesso a rischio (ad esempio per l'accesso da una località diversa).</span><span class="sxs-lookup"><span data-stu-id="a2210-180">Users covered by the policy will be prompted for MFA only during risky sign-in attempts (e.g., user is signing in from a different location).</span></span> <span data-ttu-id="a2210-181">Inoltre, gli utenti a cui viene applicato questo criterio dispongono di un periodo massimo di 14 giorni per la registrazione per l'autenticazione MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-181">In addition, users under the policy have up to 14 days to register for MFA.</span></span> <span data-ttu-id="a2210-182">Agli utenti che non hanno completato la registrazione MFA non verrà richiesta la verifica MFA durante il periodo di 14 giorni.</span><span class="sxs-lookup"><span data-stu-id="a2210-182">Users who haven't complete MFA registration will not be challenged for MFA verification during the 14-day period.</span></span> <span data-ttu-id="a2210-183">È previsto pertanto che le metriche non siano pari al 100% per i partner che hanno implementato l'autenticazione MFA usando i criteri di base per la protezione dell'utente finale di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a2210-183">Therefore, it is expected that the metrics may not be 100% for partners who have implemented MFA using Azure AD End-User Protection baseline policy.</span></span>

### <a name="are-you-using-3rd-party-mfa-solution"></a><span data-ttu-id="a2210-184">Usi una soluzione MFA di terze parti?</span><span class="sxs-lookup"><span data-stu-id="a2210-184">Are you using 3rd party MFA solution?</span></span>

<span data-ttu-id="a2210-185">Se usi una soluzione MFA di terze parti, verifica come integrarla con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a2210-185">If you are using 3rd party MFA solution, identify how you are integrating it with Azure AD.</span></span> <span data-ttu-id="a2210-186">In generale, sono disponibili due metodi, tra cui la federazione e i controlli personalizzati:</span><span class="sxs-lookup"><span data-stu-id="a2210-186">In general, there are two methods, including federation and custom controls:</span></span>

* <span data-ttu-id="a2210-187">**Federazione delle identità**: quando riceve una richiesta di autenticazione, Azure AD reindirizza l'utente al provider di identità federato per l'autenticazione.</span><span class="sxs-lookup"><span data-stu-id="a2210-187">**Identity federation** – When Azure AD receives an authentication request, Azure AD will redirect the user to the federated identity provider for authentication.</span></span> <span data-ttu-id="a2210-188">Al completamento dell'autenticazione, il provider di identità federato reindirizza di nuovo l'utente ad Azure AD insieme a un token SAML.</span><span class="sxs-lookup"><span data-stu-id="a2210-188">Upon successful authentication, the federated identity provider will redirect the user back to Azure AD along with a SAML token.</span></span> <span data-ttu-id="a2210-189">Affinché Azure AD riconosca che l'utente ha completato la verifica MFA durante l'autenticazione al provider di identità federato, il token SAML deve includere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*).</span><span class="sxs-lookup"><span data-stu-id="a2210-189">In order for Azure AD to recognize that the user has completed MFA verification when authenticating to the federated identity provider, the SAML token must include the *authenticationmethodsreferences* claim (with value *multipleauthn*).</span></span> <span data-ttu-id="a2210-190">Controlla se il provider di identità federato supporta il rilascio di tale attestazione.</span><span class="sxs-lookup"><span data-stu-id="a2210-190">Check whether that the federated identity provider supports issuing such a claim.</span></span> <span data-ttu-id="a2210-191">In tal caso, verifica che il provider di identità federato sia stato configurato per questa operazione.</span><span class="sxs-lookup"><span data-stu-id="a2210-191">If so, check whether the federated identity provider has been configured to do so.</span></span> <span data-ttu-id="a2210-192">Se l'attestazione non è presente, Azure AD (e quindi il Centro per i partner) non saprà che l'utente ha completato la verifica MFA con il conseguente mancato raggiungimento del 100% nella metrica.</span><span class="sxs-lookup"><span data-stu-id="a2210-192">If the claim is missing, Azure AD (and therefore Partner Center) will not know that the user has completed MFA verification and this can cause the metric to not be 100%.</span></span>

* <span data-ttu-id="a2210-193">**Controllo personalizzato**: non è possibile usare Controllo personalizzato di Azure AD per determinare se un utente ha completato la verifica MFA tramite una soluzione MFA di terze parti.</span><span class="sxs-lookup"><span data-stu-id="a2210-193">**Custom Control** – Azure AD Custom Control cannot be used to identify whether a user has completed MFA verification through a 3rd party MFA solution.</span></span> <span data-ttu-id="a2210-194">Di conseguenza, tutti gli utenti che hanno completato la verifica MFA tramite un controllo personalizzato verranno sempre considerati da Azure AD e, a sua volta, dal Centro per i partner come utenti che non hanno completato la verifica MFA.</span><span class="sxs-lookup"><span data-stu-id="a2210-194">As a result, any user who has completed MFA verification through a custom control will always appear to Azure AD (and in turn Partner Center) as not having completed MFA verification.</span></span> <span data-ttu-id="a2210-195">Se possibile, è consigliabile passare all'uso della Federazione delle identità anziché di un controllo personalizzato durante l'integrazione con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a2210-195">Where possible, it is recommended that you switch to using Identity Federation as opposed to Custom Control when integrating with Azure AD.</span></span>

### <a name="identity-which-users-have-logged-into-partner-center-without-mfa"></a><span data-ttu-id="a2210-196">Identificare gli utenti che hanno effettuato l'accesso al Centro per i partner senza MFA</span><span class="sxs-lookup"><span data-stu-id="a2210-196">Identity which users have logged into Partner Center without MFA</span></span>

<span data-ttu-id="a2210-197">Può essere utile identificare gli utenti che accedono al Centro per i partner senza verifica MFA e verificarli a fronte della tua implementazione MFA corrente.</span><span class="sxs-lookup"><span data-stu-id="a2210-197">It may be helpful to identify which users are logging in to Partner Center without MFA verification and verify them against your current MFA implementation.</span></span> <span data-ttu-id="a2210-198">Per verificare se un utente ha completato o meno la verifica MFA, puoi usare il [report con le informazioni di accesso Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins).</span><span class="sxs-lookup"><span data-stu-id="a2210-198">You can use [Azure AD sign-in report](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) to find out whether a user has completed MFA verification or not.</span></span> <span data-ttu-id="a2210-199">Il report con le informazioni di accesso Azure AD è attualmente disponibile solo per i partner che hanno sottoscritto Azure AD Premium o qualsiasi SKU O365 che includa Azure AD Premium, ad esempio EMS.</span><span class="sxs-lookup"><span data-stu-id="a2210-199">Azure AD sign-in report is currently only available to partners who have subscribed to Azure AD Premium or any O365 SKU which includes Azure AD Premium (for example, EMS).</span></span>

<span data-ttu-id="a2210-200">**Per altre informazioni**</span><span class="sxs-lookup"><span data-stu-id="a2210-200">**For more information**</span></span>

- [<span data-ttu-id="a2210-201">Community del gruppo di linee guida per la sicurezza del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2210-201">Partner Center security guidance group community</span></span>](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [<span data-ttu-id="a2210-202">Requisiti di sicurezza del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2210-202">Partner Center security requirements</span></span>](partner-security-requirements.md)
- [<span data-ttu-id="a2210-203">Domande frequenti sui requisiti di sicurezza del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2210-203">Partner Center security requirements FAQ</span></span>](partner-security-requirements-faq.md)