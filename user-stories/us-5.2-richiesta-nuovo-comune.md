# US-5.2 — Invio modulo di richiesta inserimento nuovo comune

**Attore:** utente registrato (User)
**Necessità:** invio di un modulo per richiedere i documenti di un comune non ancora presente nell'archivio
**Obiettivo:** disponibilità della normativa del comune su cui si sta lavorando

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (richiesta via form dei pdf di un comune non ancora nel DB) e sezione 2.3 "Non incluso" (copertura graduale dei comuni). Epic di riferimento: [epic-5-assistenza.md](../epics/epic-5-assistenza.md). Collegata a [US-4.1](us-4.1-notifica-documento-richiesto.md).

## Criteri di accettazione

- Se per un comune non ci sono documenti disponibili (comune "rosso" nella dashboard, vedi [US-3.7](us-3.7-dashboard-copertura-territoriale.md), o esito vuoto di una ricerca), l'utente può compilare il modulo, con regione, provincia e comune già precompilati, il sistema invia la richiesta e mostra una conferma di ricezione.
- Se per il comune ci sono già documenti disponibili (comune "verde"), il sistema segnala che sono già disponibili e propone il link.
- Quando la richiesta viene ricevuta, il sistema la rende consultabile all'Admin.
- Quando la richiesta viene evasa e i documenti vengono inseriti, il sistema notifica l'utente richiedente (vedi US-4.1).

## Fuori scope

- Garanzia di tempi di evasione.
- Inserimento automatico dei documenti.

## Note

- Da definire: campi facoltativi (es. tipologia di documento cercata) e priorità delle richieste multiple sullo stesso comune.
