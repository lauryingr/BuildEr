# US-3.5 — Eliminazione di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) proprietario di una cartella
**Necessità:** eliminazione di una cartella non più necessaria
**Obiettivo:** area personale ordinata, senza cartelle obsolete

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md).

## Criteri di accettazione

- L'utente può richiedere l'eliminazione di una cartella esistente; il sistema chiede una conferma esplicita.
- Se l'utente conferma e l'operazione va a buon fine, la cartella scompare dall'elenco e i documenti in essa contenuti restano disponibili nella piattaforma.
- Quando il proprietario elimina una cartella condivisa, la cartella non è più accessibile ai colleghi con cui era condivisa.
- Se un utente che non è proprietario di una cartella condivisa tenta di eliminarla, il sistema nega l'operazione.

## Fuori scope

- Recupero di cartelle eliminate (undo/cestino).

## Note

- Coerenza con US-1.3: alla cancellazione di un profilo, il comportamento sulle cartelle condivise è già definito (restano accessibili agli altri membri).
