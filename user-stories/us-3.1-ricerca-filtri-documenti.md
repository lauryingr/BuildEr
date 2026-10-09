# US-3.1 — Ricerca con filtri dei documenti

**Attore:** utente registrato (User)
**Necessità:** ricerca dei documenti normativi con filtri per provincia, comune e tipologia di documento, e download in PDF
**Obiettivo:** individuazione rapida della normativa in vigore per il comune di interesse

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (ricerca per filtri, download PDF, data/versione e fonte) e archetipo 4.1 (Elia). Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md).

## Criteri di accettazione

- Un utente autenticato può selezionare provincia e comune; il sistema mostra l'elenco dei documenti disponibili per quel comune.
- L'utente può filtrare l'elenco per tipologia (es. Regolamento Edilizio, PRG/PGT/PAT/PI, NTA); il sistema mostra solo i documenti di quella tipologia.
- Per ogni documento in elenco il sistema mostra data/versione di ultimo aggiornamento (dettaglio in [US-6.2](us-6.2-data-versione-documento.md)).
- Quando l'utente seleziona un documento, il sistema apre la scheda di dettaglio, da cui si può scaricare il PDF (vedi [US-6.1](us-6.1-scheda-documento.md) e [US-6.4](us-6.4-download-pdf.md)).
- Se la ricerca riguarda un comune senza documenti disponibili, il sistema mostra un messaggio chiaro e propone l'invio della richiesta di inserimento (vedi [US-5.2](us-5.2-richiesta-nuovo-comune.md)).
- In alternativa alla ricerca, l'utente può raggiungere i documenti navigando la dashboard di copertura nella home (vedi [US-3.7](us-3.7-dashboard-copertura-territoriale.md)).

## Fuori scope

- Ricerca in linguaggio naturale/AI.
- Ricerca full-text all'interno del contenuto dei PDF.

## Note

- Il filtro per regione è previsto dall'organizzazione geografica (regione, provincia, comune) ma il PRD cita solo provincia e comune come filtri: da confermare.
