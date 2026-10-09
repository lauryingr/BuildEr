# US-4.7 — Notifica di invito a una cartella condivisa

**Attore:** utente registrato (User) invitato in una cartella condivisa
**Necessità:** notifica in-app quando un altro utente lo invita in una cartella, con la possibilità di accettare o rifiutare; notifica a chi ha invitato quando l'invito viene rifiutato
**Obiettivo:** decidere consapevolmente se entrare in una cartella condivisa, senza essere aggiunto senza consenso, e permettere a chi invita di sapere se un collega non parteciperà

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (condivisione fascicoli tra colleghi). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-2.2](us-2.2-condivisione-fascicoli.md). Le notifiche confluiscono nel centro notifiche ([US-4.5](us-4.5-centro-notifiche.md)) con stato letto/non letto ([US-4.6](us-4.6-stato-letto-notifiche.md)).

## Criteri di accettazione

- Quando un membro invita un utente già registrato in una cartella, il sistema mostra all'invitato un banner di notifica con nome della cartella, nome di chi ha invitato e le azioni "Accetta" e "Rifiuta".
- Finché l'invitato non risponde, non ha alcun accesso alla cartella e la cartella non compare nel suo elenco.
- Se l'invitato chiude il banner o segna la notifica come letta, l'invito resta in attesa e non viene né accettato né rifiutato. Lo stesso vale se elimina la notifica dallo storico.
- Gli inviti in attesa restano sempre consultabili nell'area personale dell'utente, nella sezione "Inviti ricevuti" del profilo, da cui può accettarli o rifiutarli finché sono validi.
- Se l'invitato accetta, il sistema lo aggiunge ai membri della cartella (vedi [US-2.2](us-2.2-condivisione-fascicoli.md)) e aggiorna la notifica come gestita.
- Se l'invitato rifiuta, il sistema chiude l'invito, non concede accesso e non lo ripropone; chi ha invitato può inviarne uno nuovo.
- Quando un invito viene rifiutato, il sistema mostra a chi ha invitato una notifica con nome della cartella e dell'utente che ha rifiutato.
- Se un invito viene accettato, il sistema non invia notifica a chi ha invitato: il nuovo membro compare nell'elenco dei membri della cartella (vedi [US-2.4](us-2.4-membri-cartella-condivisa.md)).
- Se l'invito viene annullato o scade prima della risposta, il sistema rimuove le azioni dalla notifica e indica che l'invito non è più valido.
- Se l'invitato non è registrato, riceve l'invito per email e vede la notifica in-app dopo la registrazione.
- L'invito compare nel centro notifiche con tipo "invito cartella".

## Fuori scope

- Notifica a chi ha invitato quando l'invito viene accettato o scade (decisione da rivedere in futuro).
- Notifiche via email o push per gli utenti già registrati.
- Notifiche sulle modifiche ai documenti di una cartella condivisa.

## Note

- Nessun utente può essere aggiunto a una cartella senza aver accettato l'invito.
- La regola "aprire o chiudere una notifica la segna come letta e non la ripropone" ([US-4.1](us-4.1-notifica-documento-richiesto.md)) vale per la visualizzazione del banner, ma non risolve l'invito.
- Da definire la durata di validità dell'invito (ipotesi: 7 giorni, vedi US-2.2).
