# BuildEr — PRD

> Product Requirements Document
> **Autore:** Laura Ingrid Ragoni
> **Data:** 23/09/2026
> **Versione:** 1.0 (bozza)
> **Stato:** bozza

---

## Idea

L’idea nasce da molte conversazioni nate con il mio compagno Elia, Architetto neo laureato che ha iniziato a lavorare come come tale in uno studio di Ingegneria Edile integrata ad Oderzo. Il suo compito è quello di progettare opere urbane molto diverse in base alla committenza.

## 1. Riepilogo esecutivo

_In 2-3 frasi: cosa si sta costruendo e perché._

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

---

- ***

## 3. Utenti target e persona

| Persona                                                 | Bisogno principale                                                                                                                                                                               | Contesto d'uso                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Architetto, ingegnere edile/civile, urbanista, geometra | Reperire rapidamente la normativa edilizia/urbanistica ufficiale e aggiornata (Regolamento Edilizio, PRG/PGT/PAT/PI, NTA) di uno specifico comune, con la certezza che sia la versione in vigore | Fase di progettazione preliminare o di verifica di conformità di un progetto, spesso sotto scadenza verso il committente; lavoro su più comuni/province diversi nello stesso periodo, con esigenza di consultare e scaricare in PDF la documentazione per archiviarla nel fascicolo di pratica |
| Studio tecnico / società di progettazione               | Standardizzare e velocizzare la ricerca normativa per tutti i collaboratori dello studio, riducendo il tempo (e quindi il costo) speso in attività non progettuali                               | Gestione di più commesse contemporanee in comuni diversi; necessità che junior e collaboratori trovino la normativa corretta senza dover ricorrere sistematicamente al senior                                                                                                                  |

---

