# US-2.3 — Visualizzazione primaria dei documenti in relazione al tipo di utente

**Attore:** utente autenticato (Admin o User)
**Necessità:** schermata principale con documenti e funzioni prioritari in base al tipo di utente
**Obiettivo:** accesso immediato alle informazioni più rilevanti per il proprio ruolo

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente". Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md).

## Criteri di accettazione

- **Dato** un utente con ruolo User, **quando** effettua il login, **allora** il sistema mostra come vista primaria ricerca documenti, cartelle personali, preferiti e notifiche.
- **Dato** un utente con ruolo Admin, **quando** effettua il login, **allora** il sistema mostra come vista primaria la gestione di utenti, documenti e richieste ricevute (nuovi comuni, assistenza).
- **Dato** un utente con ruolo User, **quando** tenta di accedere a una funzione riservata all'Admin, **allora** il sistema nega l'accesso.

## Fuori scope

- Personalizzazione della vista in base alla professione (Architetto, Geometra, ecc.).
- Personalizzazione della home da parte dell'utente.

## Note

- Assunzione: "tipo di utente" = ruolo (Admin/User). Da confermare se la vista deve variare anche per professione.
