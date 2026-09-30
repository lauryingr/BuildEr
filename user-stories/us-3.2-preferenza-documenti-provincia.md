# US-3.2 — Azioni di preferenza sui documenti e provincia

**Attore:** utente registrato (User)
**Necessità:** salvataggio tra i preferiti di documenti/comuni e indicazione di una provincia di interesse
**Obiettivo:** accesso rapido ai contenuti più usati e base per le notifiche di aggiornamento

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (salvataggio dei comuni più utilizzati, notifiche sui preferiti). Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Alimenta le notifiche dell'Epic 4 ([US-4.2](us-4.2-notifica-aggiornamento-preferito.md), [US-4.3](us-4.3-notifica-documento-provincia.md), [US-4.4](us-4.4-notifica-aggiornamento-provincia.md)).

## Criteri di accettazione

- **Dato** un documento consultato, **quando** l'utente lo aggiunge ai preferiti, **allora** il sistema lo salva nell'elenco dei preferiti.
- **Dato** un documento tra i preferiti, **quando** l'utente lo rimuove dai preferiti, **allora** il sistema lo elimina dall'elenco senza cancellare il documento dalla piattaforma.
- **Dato** il profilo utente, **quando** l'utente imposta una o più province di interesse, **allora** il sistema le salva come preferenza.
- **Dato** una provincia di interesse impostata, **quando** l'utente la rimuove, **allora** il sistema non la considera più per le notifiche.

## Fuori scope

- Gestione delle notifiche stesse (vedi Epic 4).
- Preferiti condivisi tra colleghi.

## Note

- Da chiarire se i preferiti sono a livello di singolo documento, di comune o entrambi: il PRD parla di "comune salvato tra i preferiti".
