# US-2.2 — Condivisione di una cartella con altri utenti (team)

**Attore:** utente registrato (User) membro di una cartella
**Necessità:** condivisione di una cartella di documenti normativi con altri utenti della piattaforma, invitandoli per email
**Obiettivo:** lavoro congiunto sulla stessa documentazione, dove ognuno aggiunge i documenti che ritiene necessari per la propria competenza (architetto, ingegnere, ecc.), senza ripetere la ricerca da capo

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (condivisione fascicoli tra colleghi) e archetipo 6.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.1](us-2.1-cartelle-personalizzabili.md).

**Modello di team:** non esistono studi, responsabili o ruoli di team. Il "team" coincide con i membri di una cartella condivisa. Tutti i membri sono pari: ciascuno può consultare, scaricare, aggiungere e rimuovere documenti, rinominare la cartella e invitare altri utenti. Gli utenti con cui si condivide una cartella non devono appartenere ad alcuno studio o gruppo preesistente: l'unico legame è la cartella stessa. Un utente può far parte di più cartelle condivise con persone diverse. Il modello è analogo a una cartella condivisa su un servizio di archiviazione online: qualsiasi utente registrato può creare una cartella e condividerla, senza bisogno di un amministratore.

## Criteri di accettazione

- Un membro di una cartella può inserire l'email di un utente e inviare l'invito; il sistema invia l'invito e lo mostra come "in attesa".
- Quando un utente registrato riceve un invito, il sistema lo avvisa con una notifica in-app (vedi [US-4.7](us-4.7-notifica-invito-cartella.md)); finché non risponde non ha alcun accesso alla cartella. Può accettare o rifiutare anche in un secondo momento dalla sezione "Inviti ricevuti" del proprio profilo; chiudere la notifica non annulla l'invito.
- Quando l'invitato accetta, il sistema lo aggiunge ai membri della cartella con gli stessi poteri di tutti gli altri; se rifiuta, l'invito viene chiuso e non concede accesso.
- Quando un utente non registrato completa la registrazione (vedi [US-1.1](us-1.1-creazione-profilo.md)) e accetta l'invito ricevuto, il sistema lo aggiunge ai membri della cartella.
- Un membro invitato può a sua volta invitare altri utenti nella stessa cartella.
- Quando un membro accede a una cartella condivisa, il sistema mostra l'elenco dei documenti contenuti, con data/versione di aggiornamento, e consente di aggiungere e rimuovere documenti.
- Se un documento nella cartella condivisa viene aggiornato, il sistema mostra la versione più recente a tutti i membri.
- Se chi ha inviato l'invito lo annulla mentre è in attesa, o l'invito scade, il sistema lo invalida e il link non è più utilizzabile.
- Se un membro tenta di invitare un'email già membro della cartella, il sistema mostra un messaggio di errore.
- Un utente che non è membro di una cartella non può vederla né accedervi, nemmeno conoscendone l'indirizzo.

## Fuori scope

- Ruoli o livelli di permesso diversi tra i membri (sola lettura, responsabile, ecc.): tutti i membri sono pari.
- Entità "studio" o gruppo di lavoro persistente oltre la cartella.
- Condivisione dei preferiti.
- Rimozione di altri membri (vedi note); uscita volontaria in [US-2.4](us-2.4-membri-cartella-condivisa.md).
- Inviti in blocco (import da file) e aggiunta di membri senza consenso.

## Note

- Poiché ogni membro può invitare altri e nessuno può rimuoverli, un invito per errore non è reversibile da parte di un singolo membro: da valutare se introdurre la rimozione di un membro (e con quale regola) o limitare chi può invitare.
- Da definire la durata di validità dell'invito (ipotesi: 7 giorni).
- Per le cartelle non condivise vale solo [US-2.1](us-2.1-cartelle-personalizzabili.md).
