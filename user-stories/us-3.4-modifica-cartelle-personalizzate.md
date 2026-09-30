# US-3.4 — Modifica di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) proprietario di una cartella
**Necessità:** modifica di una cartella esistente (nome, documenti contenuti, condivisione)
**Obiettivo:** cartelle sempre coerenti con le commesse in corso

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md).

## Criteri di accettazione

- **Dato** una cartella esistente, **quando** l'utente ne modifica il nome e salva, **allora** il sistema aggiorna il nome.
- **Dato** una cartella esistente, **quando** l'utente aggiunge o rimuove un documento, **allora** il sistema aggiorna il contenuto senza cancellare il documento dalla piattaforma.
- **Dato** una cartella condivisa, **quando** il proprietario aggiunge o rimuove un collega, **allora** il sistema aggiorna gli accessi di conseguenza.
- **Dato** una cartella condivisa, **quando** un utente che non ne è proprietario tenta di modificarla, **allora** il sistema nega l'operazione.

## Fuori scope

- Creazione ed eliminazione delle cartelle.

## Note

- Da definire se anche i colleghi con cui la cartella è condivisa possano modificarne il contenuto.
