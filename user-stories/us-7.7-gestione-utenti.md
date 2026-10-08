# US-7.7 — Gestione degli utenti

**Attore:** Admin (super admin)
**Necessità:** consultazione e gestione degli utenti registrati
**Obiettivo:** controllo sugli accessi e sui ruoli della piattaforma

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Il ruolo Admin viene assegnato solo manualmente/internamente (vedi [US-1.1](us-1.1-creazione-profilo.md)).

## Criteri di accettazione

- Nella sezione dedicata l'Admin vede l'elenco degli utenti registrati con nome, email, professione, ruolo e data di registrazione.
- L'Admin può cercare un utente per nome o email; il sistema mostra i risultati corrispondenti.
- L'Admin può modificare il ruolo di un utente (User/Admin); il sistema aggiorna i permessi dell'utente.
- L'Admin può sospendere un utente; il sistema gli impedisce l'accesso mantenendone i dati.

## Fuori scope

- Eliminazione del profilo per conto dell'utente (non trattata, vedi US-1.3).

## Note

- Da valutare se la sospensione è necessaria al lancio.
