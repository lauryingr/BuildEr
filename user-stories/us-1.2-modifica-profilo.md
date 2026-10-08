# US-1.2 — Modifica profilo utente personale

**Attore:** utente registrato (Admin o User)
**Necessità:** modifica dei dati del profilo personale
**Obiettivo:** informazioni sempre aggiornate (es. dati anagrafici, professione, email, password)

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md). Dipende da [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- Un utente autenticato può accedere alla sezione "Profilo", dove il sistema mostra i dati attuali e ne consente la modifica.
- Quando l'utente modifica un campo del profilo (es. nome, professione) e salva, il sistema aggiorna i dati e li rende subito visibili.
- Per cambiare la password, l'utente inserisce la password attuale e la nuova; il sistema aggiorna la password solo se quella attuale è corretta.
- Se l'utente modifica l'email con un indirizzo già in uso da un altro profilo, il sistema mostra un messaggio di errore e non applica la modifica.

## Fuori scope

- Modifica del ruolo utente da parte dell'utente stesso (riservata all'Admin).

## Note

- Nessuna nota aggiuntiva al momento.
