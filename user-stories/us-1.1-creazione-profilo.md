# US-1.1 — Creazione profilo utente personale

**Come** nuovo utente (Admin o User: Architetto, Geometra, Urbanista, Ingegnere civile)
**Voglio** creare il mio profilo personale sulla piattaforma
**Così da** poter accedere ai documenti normativi e alle funzionalità riservate agli utenti registrati

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (creazione utente) e archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md).

## Criteri di accettazione

- **Dato** che sono un visitatore non registrato, **quando** compilo il form di registrazione con i dati richiesti (es. nome, cognome, email, password, ruolo/professione), **allora** viene creato il mio profilo utente.
- **Dato** un profilo appena creato, **quando** la registrazione va a buon fine, **allora** ricevo conferma e posso accedere (login) alla piattaforma.
- **Dato** che sto registrando un profilo, **quando** inserisco un'email già associata a un altro profilo, **allora** vedo un messaggio di errore chiaro e non viene creato un duplicato.
- **Dato** un nuovo profilo, **quando** viene creato, **allora** gli viene assegnato di default il ruolo "User" (Admin assegnato solo manualmente/internamente).

## Fuori scope

- Login/registrazione tramite provider esterni (Google, LinkedIn, ecc.), salvo diversa decisione futura.
- Gestione degli inviti multi-utente/studio (vedi Epic 2).

## Note

- I 2 ruoli previsti sono Admin (gestione completa della piattaforma e degli utenti) e User (Architetto, Geometra, Urbanista, Ingegnere civile).
