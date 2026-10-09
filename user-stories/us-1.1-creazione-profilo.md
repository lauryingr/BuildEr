# US-1.1 — Creazione profilo utente personale

**Attore:** visitatore non registrato (futuro Admin o User: Architetto, Geometra, Urbanista, Ingegnere civile)
**Necessità:** creazione di un profilo personale sulla piattaforma
**Obiettivo:** accesso ai documenti normativi e alle funzionalità riservate agli utenti registrati

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (creazione utente) e archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md).

## Criteri di accettazione

- Un utente non registrato può compilare il form di registrazione inserendo i dati richiesti (nome, cognome, email, password, ruolo/professione); il sistema crea il profilo utente.
- Se la registrazione va a buon fine, il sistema mostra un messaggio di conferma e l'utente può effettuare il login.
- Se l'email inserita è già associata a un altro profilo, il sistema mostra un messaggio di errore chiaro e non crea un duplicato.
- Il sistema assegna di default al nuovo profilo il ruolo "User"; il ruolo "Admin" viene assegnato solo manualmente/internamente.

## Fuori scope

- Login/registrazione tramite provider esterni (Google, LinkedIn, ecc.), salvo diversa decisione futura.
- Gestione degli inviti alle cartelle condivise (vedi US-2.2); un invitato non registrato completa la registrazione e poi accetta l'invito.

## Note

- I 2 ruoli previsti sono Admin (gestione completa della piattaforma e degli utenti) e User (Architetto, Geometra, Urbanista, Ingegnere civile).
