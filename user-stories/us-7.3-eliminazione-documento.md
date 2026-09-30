# US-7.3 — Eliminazione o archiviazione di un documento

**Attore:** Admin (super admin)
**Necessità:** eliminazione o archiviazione di un documento non più valido
**Obiettivo:** nessun documento obsoleto presentato come in vigore

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-7.1](us-7.1-inserimento-documento.md).

## Criteri di accettazione

- **Dato** un documento esistente, **quando** l'Admin ne richiede l'eliminazione, **allora** il sistema chiede una conferma esplicita.
- **Dato** una conferma di eliminazione, **quando** l'operazione va a buon fine, **allora** il documento non è più disponibile nella ricerca.
- **Dato** un documento presente nelle cartelle o nei preferiti di utenti, **quando** viene eliminato, **allora** il sistema lo segnala come non più disponibile negli elenchi degli utenti.
- **Dato** un documento sostituito da una nuova versione, **quando** viene archiviato, **allora** il sistema lo rimuove dalla ricerca mantenendone traccia interna.

## Fuori scope

- Recupero di documenti eliminati (da valutare).

## Note

- Da decidere se prevedere eliminazione definitiva o solo archiviazione.
