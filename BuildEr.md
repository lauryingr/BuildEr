# BuildEr — PRD

> Product Requirements Document
> **Autore:** Laura Ingrid Ragoni
> **Data:** 23/09/2026
> **Versione:** 1.0 (bozza)
> **Stato:** bozza

---

## 1. Idea

L’idea nasce da molte conversazioni nate con il mio compagno Elia, Architetto neo laureato che ha iniziato a lavorare come come tale in uno studio di Ingegneria Edile integrata ad Oderzo. Il suo compito è quello di progettare opere urbane molto diverse in base alla committenza.

---

## 2. Contesto e problema

Durante questi ragionamenti mi presenta il suo problema: la reperibilità delle normative di ogni comune. Ogni comune italiano non pubblica le proprie norme urbanistiche ed edilizie in un formato standard, né in un luogo prevedibile del proprio sito istituzionale. Non esiste un portale unico nazionale che raccolga in modo organico Regolamenti Edilizi, Piani Regolatori (PRG/PGT/PAT/PI) e relative Norme Tecniche di Attuazione: ogni professionista è costretto a cercare manualmente, comune per comune, spesso tra decine di PDF sparsi tra sezioni "Urbanistica", "Edilizia Privata" e "Amministrazione Trasparente", senza alcuna garanzia che il documento trovato sia effettivamente l'ultima versione in vigore.

Questo chiaramente porta via molto tempo solo nella ricerca dei documenti e ulteriore tempo per la consultazione.

### 2.1 Problema da risolvere

La soluzione per risolvere parzialmente questo problema sarebbe una sorta di applicativo web basato su un archivio digitale, organizzato per localizzazione geografica (regione, provincia, comune), che raccoglie in un unico punto tutta la documentazione normativa edilizia e urbanistica ufficiale, ovviamente reperita esclusivamente da fonti istituzionali (siti comunali, BUR regionali, Normativa) e la mantiene aggiornata tramite un sistema di monitoraggio automatico, così che un architetto non debba più chiedersi se la norma che sta consultando sia ancora quella in vigore.

### 2.2 Perché ora

Cioò che ha dato origine a BuildEr non nasce da un'analisi di mercato a tavolino, ma da una richiesta concreta e diretta del mio compagno, nel confrontarsi ogni giorno con le normative urbanistiche ed edilizie dei comuni in cui lavora. Non è un'ipotesi di prodotto in cerca di un problema — è un problema reale, vissuto da un professionista sul campo, che cerca una soluzione.

Che il bisogno sia reale e non isolato è confermato: esiste già un'Ai arcai.it, che si propone di risolvere lo stesso problema per l'Italia, offrendo interrogazione in linguaggio naturale delle normative di migliaia di comuni. La sua esistenza è una validazione indiretta: il problema della reperibilità e dell'aggiornamento delle normative comunali è reale.
Arcai.it è una soluzione a pagamento, circa 40euro al mese, il mio obiettivo è di realizzare un'applicazione simile, senza AI all'interno ma che restituisca la normativa corretta e aggiornata scaricabile in pdf solo con dei filtri per provincia e comune.

### 2.3 Cosa è incluso e cosa non è incluso

E' inclusa:

- La possibilità di crare un utente e di salvare i pdf dei comuni più utilizzati.
- La possibilità di richiedere attraverso una form, i pdf dei documenti di un comune non ancora nel DB
- Scaricare qualsiasi pdf presente dei comuni inseriti
- Banner di notifica all'utente quando viene aggiornata una normativa di un comune che ha salvato tra i preferiti
- Data/versione di ultimo aggiornamento visibile su ogni documento con chiara indicazione della fonte da cui proviene per sicurezza.
- Ricerca filtro per tipologia di documento oltre che per provincia e comune.
- Gestione multi-utente/permessi per studio (ruoli, condivisione fascicoli tra colleghi)

Non è incluso:

- Interrogazione in linguaggi naturale/AI sulle normative. Le normative potranno solo essere consultate oppure scaricate.
- integrazioni con altri software di progettazione/CAD.
- Verifica di conformità automatica di un progetto rispetto alla normativa
- Copertura di tutti i 7900 comuni italiani al lancio, (le integrazioni, se possibili, saranno graduali)

---

- ***

## 3. Ruoli utente

| Ruolo | Descrizione |
| ----- | ----------- |
| Admin | Gestione completa della piattaforma e degli utenti |
| User  | Architetto, Geometra, Urbanista, Ingegnere civile |

2 tipologie di utente previste: Admin e User.

---

## 4. Stackeholder

| 👤 Persona                                                  | 🎯 Bisogno principale                                                                                                                                                                          | 📍 Contesto d'uso                                                                                                                                                                                                 |
| ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Architetto, ingegnere edile/civile, urbanista, geometra** | Reperire rapidamente la normativa edilizia/urbanistica ufficiale e aggiornata (Regolamento Edilizio, PRG/PGT/PAT/PI, NTA) di uno specifico comune, con certezza di avere la versione in vigore | Fase di progettazione preliminare o di verifica di conformità, spesso sotto scadenza verso il committente; lavoro su più comuni/province diversi, con esigenza di consultare e scaricare in PDF la documentazione |
| **Studio tecnico / Società di progettazione**               | Standardizzare e velocizzare la ricerca normativa per tutti i collaboratori, riducendo il tempo (e costo) speso in attività non progettuali                                                    | Gestione di più commesse contemporanee in comuni diversi; necessità che junior e collaboratori trovino la normativa corretta senza dover ricorrere sistematicamente al senior                                     |

---

## 5. Archetipi utente

### 4.1 Elia, l'Architetto sul campo

- **Ruolo:** Architetto neolaureato, dipendente di uno studio di ingegneria edile
- **Età:** 25 anni
- **Obiettivi:**
  - Trovare in pochi minuti la normativa in vigore per il comune su cui sta lavorando
  - Avere la certezza che il documento scaricato sia la versione aggiornata, senza doverla verificare a mano sul sito del comune
  - Archiviare i PDF consultati nel fascicolo di pratica in modo ordinato
- **Frustrazioni attuali:**
  - Perde ore a cercare PDF sparsi tra sezioni "Urbanistica", "Edilizia Privata" e "Amministrazione Trasparente"
  - Non ha mai la certezza di essere di fronte all'ultima versione in vigore di un regolamento
  - Deve ripetere la stessa ricerca ogni volta che lo studio prende una commessa in un nuovo comune
- **Comportamento d'uso:** Consulta la normativa soprattutto nella fase preliminare di progettazione e nella verifica di conformità, spesso sotto scadenza; lavora su più comuni/province in parallelo
- **Citazione rappresentativa:** _"voglio essere sicuro di avere in mano il PDF giusto e aggiornato e di consultarlo in pochi click."_

### 4.2 Studio Associato Rossi & Bianchi, lo Studio tecnico

- **Ruolo:** Piccolo/medio studio di progettazione con titolari, senior e collaboratori junior
- **Obiettivi:**
  - Ridurre il tempo (e quindi il costo) che i collaboratori junior spendono in attività di ricerca non progettuale
  - Rendere autonomi i junior nella ricerca normativa, senza che debbano interrompere continuamente i senior
  - Avere uno storico condiviso della documentazione normativa già raccolta per i comuni in cui lo studio opera abitualmente
- **Frustrazioni attuali:**
  - Ogni collaboratore rifà da zero la stessa ricerca già fatta da un collega per lo stesso comune
  - Difficoltà a garantire che tutti nello studio lavorino sulla stessa versione aggiornata della normativa
- **Comportamento d'uso:** Gestisce più commesse contemporanee in comuni diversi; ha bisogno di condividere fascicoli e preferiti tra i membri del team
- **Citazione rappresentativa:** _"Se un collega ha già trovato la normativa di un comune, voglio che tutto lo studio ci acceda senza rifare la ricerca da capo."_

---

## 6. Epic e User Story

Il backlog è organizzato in 8 Epic. Ogni Epic ha un proprio file di dettaglio in [epics/](epics/) con l'elenco delle User Story collegate, ciascuna in un proprio file in [user-stories/](user-stories/).

Tutte le User Story sono compilate con attore, necessità, obiettivo e criteri di accettazione; sono bozze da revisionare (le assunzioni aperte sono indicate nella sezione Note di ciascuna).

| Epic | Titolo | File |
| ---- | ------ | ---- |
| EPIC 1 | Profilo Utente | [epic-1-profilo-utente.md](epics/epic-1-profilo-utente.md) |
| EPIC 2 | Gestione Multi Utente | [epic-2-gestione-multi-utente.md](epics/epic-2-gestione-multi-utente.md) |
| EPIC 3 | Azioni sui Documenti | [epic-3-azioni-documenti.md](epics/epic-3-azioni-documenti.md) |
| EPIC 4 | Banner e Notifiche | [epic-4-banner-notifiche.md](epics/epic-4-banner-notifiche.md) |
| EPIC 5 | Assistenza | [epic-5-assistenza.md](epics/epic-5-assistenza.md) |
| EPIC 6 | Consultazione del Documento | [epic-6-consultazione-documento.md](epics/epic-6-consultazione-documento.md) |
| EPIC 7 | Amministrazione dei Contenuti (Admin) | [epic-7-amministrazione-contenuti.md](epics/epic-7-amministrazione-contenuti.md) |
| EPIC 8 | Monitoraggio Automatico delle Fonti | [epic-8-monitoraggio-automatico.md](epics/epic-8-monitoraggio-automatico.md) |

| ID | Titolo | Epic | File |
| -- | ------ | ---- | ---- |
| US-1.1 | Creazione profilo utente personale | EPIC 1 | [us-1.1-creazione-profilo.md](user-stories/us-1.1-creazione-profilo.md) |
| US-1.2 | Modifica profilo utente personale | EPIC 1 | [us-1.2-modifica-profilo.md](user-stories/us-1.2-modifica-profilo.md) |
| US-1.3 | Eliminazione profilo utente personale | EPIC 1 | [us-1.3-eliminazione-profilo.md](user-stories/us-1.3-eliminazione-profilo.md) |
| US-2.1 | Cartelle personalizzabili | EPIC 2 | [us-2.1-cartelle-personalizzabili.md](user-stories/us-2.1-cartelle-personalizzabili.md) |
| US-2.2 | Condivisione fascicoli tra colleghi | EPIC 2 | [us-2.2-condivisione-fascicoli.md](user-stories/us-2.2-condivisione-fascicoli.md) |
| US-2.3 | Visualizzazione primaria dei documenti in relazione al tipo di utente | EPIC 2 | [us-2.3-visualizzazione-primaria-documenti.md](user-stories/us-2.3-visualizzazione-primaria-documenti.md) |
| US-2.4 | Creazione studio | EPIC 2 | [us-2.4-creazione-studio.md](user-stories/us-2.4-creazione-studio.md) |
| US-2.5 | Invito di membri nello studio | EPIC 2 | [us-2.5-invito-membri-studio.md](user-stories/us-2.5-invito-membri-studio.md) |
| US-2.6 | Rimozione di membri dallo studio | EPIC 2 | [us-2.6-rimozione-membri-studio.md](user-stories/us-2.6-rimozione-membri-studio.md) |
| US-2.7 | Gestione dei permessi dei membri dello studio | EPIC 2 | [us-2.7-permessi-membri-studio.md](user-stories/us-2.7-permessi-membri-studio.md) |
| US-3.1 | Ricerca con filtri dei documenti | EPIC 3 | [us-3.1-ricerca-filtri-documenti.md](user-stories/us-3.1-ricerca-filtri-documenti.md) |
| US-3.2 | Azioni di preferenza sui documenti e provincia | EPIC 3 | [us-3.2-preferenza-documenti-provincia.md](user-stories/us-3.2-preferenza-documenti-provincia.md) |
| US-3.3 | Creazione di cartelle personalizzate e condivisibili | EPIC 3 | [us-3.3-creazione-cartelle-personalizzate.md](user-stories/us-3.3-creazione-cartelle-personalizzate.md) |
| US-3.4 | Modifica di cartelle personalizzate e condivisibili | EPIC 3 | [us-3.4-modifica-cartelle-personalizzate.md](user-stories/us-3.4-modifica-cartelle-personalizzate.md) |
| US-3.5 | Eliminazione di cartelle personalizzate e condivisibili | EPIC 3 | [us-3.5-eliminazione-cartelle-personalizzate.md](user-stories/us-3.5-eliminazione-cartelle-personalizzate.md) |
| US-3.6 | Elenco e visualizzazione dei preferiti | EPIC 3 | [us-3.6-elenco-preferiti.md](user-stories/us-3.6-elenco-preferiti.md) |
| US-4.1 | Notifiche di aggiunta documento richiesto | EPIC 4 | [us-4.1-notifica-documento-richiesto.md](user-stories/us-4.1-notifica-documento-richiesto.md) |
| US-4.2 | Notifiche di aggiornamento documento preferito | EPIC 4 | [us-4.2-notifica-aggiornamento-preferito.md](user-stories/us-4.2-notifica-aggiornamento-preferito.md) |
| US-4.3 | Notifiche di aggiunta documento provincia | EPIC 4 | [us-4.3-notifica-documento-provincia.md](user-stories/us-4.3-notifica-documento-provincia.md) |
| US-4.4 | Notifiche di aggiornamento documento provincia | EPIC 4 | [us-4.4-notifica-aggiornamento-provincia.md](user-stories/us-4.4-notifica-aggiornamento-provincia.md) |
| US-4.5 | Centro notifiche e storico | EPIC 4 | [us-4.5-centro-notifiche.md](user-stories/us-4.5-centro-notifiche.md) |
| US-4.6 | Stato letto/non letto delle notifiche | EPIC 4 | [us-4.6-stato-letto-notifiche.md](user-stories/us-4.6-stato-letto-notifiche.md) |
| US-5.1 | Invio modulo di assistenza tecnica (bug, ecc.) | EPIC 5 | [us-5.1-assistenza-tecnica.md](user-stories/us-5.1-assistenza-tecnica.md) |
| US-5.2 | Invio modulo di richiesta inserimento nuovo comune | EPIC 5 | [us-5.2-richiesta-nuovo-comune.md](user-stories/us-5.2-richiesta-nuovo-comune.md) |
| US-6.1 | Scheda di dettaglio del documento | EPIC 6 | [us-6.1-scheda-documento.md](user-stories/us-6.1-scheda-documento.md) |
| US-6.2 | Data e versione di ultimo aggiornamento | EPIC 6 | [us-6.2-data-versione-documento.md](user-stories/us-6.2-data-versione-documento.md) |
| US-6.3 | Fonte ufficiale del documento | EPIC 6 | [us-6.3-fonte-ufficiale-documento.md](user-stories/us-6.3-fonte-ufficiale-documento.md) |
| US-6.4 | Download del documento in PDF | EPIC 6 | [us-6.4-download-pdf.md](user-stories/us-6.4-download-pdf.md) |
| US-6.5 | Consultazione online del documento | EPIC 6 | [us-6.5-consultazione-online-documento.md](user-stories/us-6.5-consultazione-online-documento.md) |
| US-7.1 | Inserimento di un documento | EPIC 7 | [us-7.1-inserimento-documento.md](user-stories/us-7.1-inserimento-documento.md) |
| US-7.2 | Modifica di un documento | EPIC 7 | [us-7.2-modifica-documento.md](user-stories/us-7.2-modifica-documento.md) |
| US-7.3 | Eliminazione o archiviazione di un documento | EPIC 7 | [us-7.3-eliminazione-documento.md](user-stories/us-7.3-eliminazione-documento.md) |
| US-7.4 | Gestione di regioni, province e comuni | EPIC 7 | [us-7.4-gestione-anagrafica-territoriale.md](user-stories/us-7.4-gestione-anagrafica-territoriale.md) |
| US-7.5 | Gestione delle richieste di nuovo comune | EPIC 7 | [us-7.5-gestione-richieste-nuovo-comune.md](user-stories/us-7.5-gestione-richieste-nuovo-comune.md) |
| US-7.6 | Gestione delle segnalazioni di assistenza | EPIC 7 | [us-7.6-gestione-segnalazioni-assistenza.md](user-stories/us-7.6-gestione-segnalazioni-assistenza.md) |
| US-7.7 | Gestione degli utenti | EPIC 7 | [us-7.7-gestione-utenti.md](user-stories/us-7.7-gestione-utenti.md) |
| US-8.1 | Pagina di monitoraggio riservata al super admin | EPIC 8 | [us-8.1-pagina-monitoraggio.md](user-stories/us-8.1-pagina-monitoraggio.md) |
| US-8.2 | Configurazione delle fonti da monitorare | EPIC 8 | [us-8.2-configurazione-fonti-monitorate.md](user-stories/us-8.2-configurazione-fonti-monitorate.md) |
| US-8.3 | Rilevamento automatico delle modifiche | EPIC 8 | [us-8.3-rilevamento-modifiche.md](user-stories/us-8.3-rilevamento-modifiche.md) |
| US-8.4 | Revisione e approvazione degli aggiornamenti rilevati | EPIC 8 | [us-8.4-revisione-aggiornamenti-rilevati.md](user-stories/us-8.4-revisione-aggiornamenti-rilevati.md) |
| US-8.5 | Log e storico dei controlli | EPIC 8 | [us-8.5-log-monitoraggio.md](user-stories/us-8.5-log-monitoraggio.md) |
| US-8.6 | Avvio manuale del controllo di una fonte | EPIC 8 | [us-8.6-controllo-manuale.md](user-stories/us-8.6-controllo-manuale.md) |

---

