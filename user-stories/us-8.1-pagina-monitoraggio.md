# US-8.1 — Pagina di monitoraggio riservata al super admin

**Attore:** Admin (super admin)
**Necessità:** accesso a una pagina dedicata al monitoraggio automatico delle fonti
**Obiettivo:** controllo centralizzato dello stato di aggiornamento dell'intero archivio

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin).

## Criteri di accettazione

- Quando un Admin accede alla pagina di monitoraggio, il sistema mostra il riepilogo: numero di fonti monitorate, ultimo controllo, aggiornamenti da revisionare, errori recenti.
- Se un utente con ruolo User tenta di accedere alla pagina di monitoraggio, il sistema nega l'accesso.
- Se un utente non autenticato tenta di accedere alla pagina di monitoraggio, il sistema reindirizza al login.
- Nella pagina di monitoraggio l'Admin può filtrare per regione, provincia, comune e stato.

## Fuori scope

- Accesso alla pagina per ruoli diversi da Admin.

## Note

- Assunzione: la pagina è visibile solo a chi ha il ruolo Admin (super admin).
