# US-3.4 — Modifica di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) proprietario di una cartella
**Necessità:** modifica di una cartella esistente (nome, documenti contenuti, condivisione)
**Obiettivo:** cartelle sempre coerenti con le commesse in corso

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md).

## Criteri di accettazione

- L'utente può modificare il nome di una cartella esistente; quando salva, il sistema aggiorna il nome.
- L'utente può aggiungere o rimuovere un documento da una cartella; il sistema aggiorna il contenuto senza cancellare il documento dalla piattaforma.
- Il proprietario di una cartella condivisa può aggiungere o rimuovere un collega; il sistema aggiorna gli accessi di conseguenza.
- Se un utente che non è proprietario di una cartella condivisa tenta di modificarla, il sistema nega l'operazione.

## Fuori scope

- Creazione ed eliminazione delle cartelle.

## Note

- Da definire se anche i colleghi con cui la cartella è condivisa possano modificarne il contenuto.
