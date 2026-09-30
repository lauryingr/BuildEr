# US-7.7 — Gestione degli utenti

**Attore:** Admin (super admin)
**Necessità:** consultazione e gestione degli utenti registrati
**Obiettivo:** controllo sugli accessi e sui ruoli della piattaforma

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Il ruolo Admin viene assegnato solo manualmente/internamente (vedi [US-1.1](us-1.1-creazione-profilo.md)).

## Criteri di accettazione

- **Dato** gli utenti registrati, **quando** l'Admin accede alla sezione dedicata, **allora** il sistema mostra l'elenco con nome, email, professione, ruolo e data di registrazione.
- **Dato** un utente, **quando** l'Admin lo cerca per nome o email, **allora** il sistema mostra i risultati corrispondenti.
- **Dato** un utente, **quando** l'Admin ne modifica il ruolo (User/Admin), **allora** il sistema aggiorna i permessi dell'utente.
- **Dato** un utente, **quando** l'Admin lo sospende, **allora** il sistema gli impedisce l'accesso mantenendone i dati.

## Fuori scope

- Eliminazione del profilo per conto dell'utente (non trattata, vedi US-1.3).

## Note

- Da valutare se la sospensione è necessaria al lancio.
