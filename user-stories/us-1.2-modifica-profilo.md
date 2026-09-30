# US-1.2 — Modifica profilo utente personale

**Attore:** utente registrato (Admin o User)
**Necessità:** modifica dei dati del profilo personale
**Obiettivo:** informazioni sempre aggiornate (es. dati anagrafici, professione, email, password)

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md). Dipende da [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- **Dato** un utente autenticato, **quando** accede alla sezione "Profilo", **allora** il sistema mostra i dati attuali e ne consente la modifica.
- **Dato** la modifica di un campo del profilo (es. nome, professione), **quando** si salva, **allora** i nuovi dati vengono aggiornati e resi subito visibili.
- **Dato** una richiesta di cambio password, **quando** vengono inserite la password attuale e la nuova, **allora** la password viene aggiornata solo se quella attuale è corretta.
- **Dato** una modifica dell'email con un indirizzo già in uso da un altro profilo, **quando** si salva, **allora** il sistema mostra un messaggio di errore e non applica la modifica.

## Fuori scope

- Modifica del ruolo utente da parte dell'utente stesso (riservata all'Admin).

## Note

- Nessuna nota aggiuntiva al momento.
