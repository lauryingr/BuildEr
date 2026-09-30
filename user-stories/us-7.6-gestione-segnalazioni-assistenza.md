# US-7.6 — Gestione delle segnalazioni di assistenza

**Attore:** Admin (super admin)
**Necessità:** consultazione e gestione delle segnalazioni tecniche inviate dagli utenti
**Obiettivo:** risoluzione dei problemi segnalati

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-5.1](us-5.1-assistenza-tecnica.md).

## Criteri di accettazione

- **Dato** le segnalazioni ricevute, **quando** l'Admin accede alla sezione dedicata, **allora** il sistema le mostra con oggetto, utente, data e stato.
- **Dato** una segnalazione, **quando** l'Admin ne cambia lo stato (aperta, in lavorazione, chiusa), **allora** il sistema salva il nuovo stato.
- **Dato** una segnalazione aperta, **quando** l'Admin la apre, **allora** il sistema mostra la descrizione completa e i dati di contatto dell'utente.

## Fuori scope

- Sistema di ticketing completo con risposte in piattaforma.

## Note

- Da definire se le segnalazioni arrivano anche via email.
