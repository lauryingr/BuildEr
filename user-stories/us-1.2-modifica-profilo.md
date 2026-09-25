# US-1.2 — Modifica profilo utente personale

**Come** utente registrato (Admin o User)
**Voglio** modificare i dati del mio profilo personale
**Così da** mantenere aggiornate le mie informazioni (es. dati anagrafici, professione, email, password)

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md). Dipende da [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- **Dato** che sono autenticato, **quando** accedo alla sezione "Profilo", **allora** vedo i miei dati attuali e posso modificarli.
- **Dato** che modifico un campo del profilo (es. nome, professione), **quando** salvo, **allora** i nuovi dati vengono aggiornati e visibili immediatamente.
- **Dato** che voglio cambiare la password, **quando** inserisco la password attuale e la nuova password, **allora** la password viene aggiornata solo se la password attuale è corretta.
- **Dato** che provo a modificare l'email con una già in uso da un altro profilo, **quando** salvo, **allora** vedo un messaggio di errore e la modifica non viene applicata.

## Fuori scope

- Modifica del ruolo utente da parte dell'utente stesso (riservata all'Admin).

## Note

- Nessuna nota aggiuntiva al momento.
