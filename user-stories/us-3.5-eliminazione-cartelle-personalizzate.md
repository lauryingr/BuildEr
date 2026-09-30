# US-3.5 — Eliminazione di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) proprietario di una cartella
**Necessità:** eliminazione di una cartella non più necessaria
**Obiettivo:** area personale ordinata, senza cartelle obsolete

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md).

## Criteri di accettazione

- **Dato** una cartella esistente, **quando** l'utente ne richiede l'eliminazione, **allora** il sistema chiede una conferma esplicita.
- **Dato** una conferma di eliminazione, **quando** l'operazione va a buon fine, **allora** la cartella scompare dall'elenco e i documenti in essa contenuti restano disponibili nella piattaforma.
- **Dato** una cartella condivisa, **quando** il proprietario la elimina, **allora** la cartella non è più accessibile ai colleghi con cui era condivisa.
- **Dato** una cartella condivisa, **quando** un utente che non ne è proprietario tenta di eliminarla, **allora** il sistema nega l'operazione.

## Fuori scope

- Recupero di cartelle eliminate (undo/cestino).

## Note

- Coerenza con US-1.3: alla cancellazione di un profilo, il comportamento sulle cartelle condivise è già definito (restano accessibili agli altri membri).
