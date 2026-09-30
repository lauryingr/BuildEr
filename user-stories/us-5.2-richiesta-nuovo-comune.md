# US-5.2 — Invio modulo di richiesta inserimento nuovo comune

**Attore:** utente registrato (User)
**Necessità:** invio di un modulo per richiedere i documenti di un comune non ancora presente nell'archivio
**Obiettivo:** disponibilità della normativa del comune su cui si sta lavorando

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (richiesta via form dei pdf di un comune non ancora nel DB) e sezione 2.3 "Non incluso" (copertura graduale dei comuni). Epic di riferimento: [epic-5-assistenza.md](../epics/epic-5-assistenza.md). Collegata a [US-4.1](us-4.1-notifica-documento-richiesto.md).

## Criteri di accettazione

- **Dato** un comune non presente nell'archivio, **quando** l'utente compila il modulo indicando regione, provincia e comune, **allora** il sistema invia la richiesta e mostra una conferma di ricezione.
- **Dato** un comune già presente, **quando** l'utente tenta di inviare la richiesta, **allora** il sistema segnala che i documenti sono già disponibili e propone il link.
- **Dato** una richiesta inviata, **quando** viene ricevuta, **allora** il sistema la rende consultabile all'Admin.
- **Dato** una richiesta evasa, **quando** i documenti vengono inseriti, **allora** il sistema notifica l'utente richiedente (vedi US-4.1).

## Fuori scope

- Garanzia di tempi di evasione.
- Inserimento automatico dei documenti.

## Note

- Da definire: campi facoltativi (es. tipologia di documento cercata) e priorità delle richieste multiple sullo stesso comune.
