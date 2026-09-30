# US-5.1 — Invio modulo di assistenza tecnica (bug, ecc.)

**Attore:** utente registrato (Admin o User)
**Necessità:** invio di un modulo per segnalare un problema tecnico o richiedere supporto
**Obiettivo:** risoluzione di bug o malfunzionamenti della piattaforma

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md). Epic di riferimento: [epic-5-assistenza.md](../epics/epic-5-assistenza.md).

## Criteri di accettazione

- **Dato** un utente autenticato, **quando** compila il modulo di assistenza con oggetto e descrizione del problema, **allora** il sistema invia la richiesta e mostra una conferma di ricezione.
- **Dato** un modulo con campi obbligatori mancanti, **quando** l'utente tenta l'invio, **allora** il sistema evidenzia i campi mancanti e non invia la richiesta.
- **Dato** una richiesta inviata, **quando** viene ricevuta, **allora** il sistema la rende consultabile all'Admin.

## Fuori scope

- Chat in tempo reale.
- Sistema di ticketing con tracciamento dello stato (da valutare in futuro).

## Note

- Il PRD non cita esplicitamente questa funzione tra le incluse: da confermare il canale di ricezione (email o area Admin).
