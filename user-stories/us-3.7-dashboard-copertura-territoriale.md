# US-3.7 — Dashboard di copertura territoriale nella home

**Attore:** utente registrato (User)
**Necessità:** vista d'insieme nella home della copertura normativa, navigabile per regione, provincia e comune
**Obiettivo:** capire a colpo d'occhio per quali comuni la normativa è già presente e per quali no, e raggiungere rapidamente i documenti o la richiesta di inserimento

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (ricerca per provincia e comune, richiesta di comuni non presenti, copertura progressiva). Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Alimentata dall'anagrafica territoriale di [US-7.4](us-7.4-gestione-anagrafica-territoriale.md); collegata a [US-3.1](us-3.1-ricerca-filtri-documenti.md) e [US-5.2](us-5.2-richiesta-nuovo-comune.md).

## Criteri di accettazione

- Nella home l'utente vede un pulsante per ciascuna delle 20 regioni.
- Quando l'utente seleziona una regione, il sistema mostra i pulsanti delle sue province; quando seleziona una provincia, mostra i pulsanti dei suoi comuni. L'utente può tornare al livello precedente.
- Ogni comune è verde se per quel comune è presente almeno un documento normativo, rosso altrimenti. Il colore è accompagnato da un'indicazione testuale o da un'icona ("disponibile" / "non ancora disponibile").
- Quando l'utente seleziona un comune verde, il sistema mostra i documenti di quel comune (come in [US-3.1](us-3.1-ricerca-filtri-documenti.md)).
- Quando l'utente seleziona un comune rosso, il sistema indica che i documenti non sono ancora disponibili e propone l'invio della richiesta di inserimento ([US-5.2](us-5.2-richiesta-nuovo-comune.md)).
- Quando l'Admin inserisce il primo documento di un comune (US-7.1), il comune diventa verde senza altre operazioni.

## Fuori scope

- Mappa geografica interattiva.
- Indicazione della completezza dei documenti del comune (quali tipologie sono presenti o mancano).
- Colorazione o contatori a livello di regione e provincia.

## Note

- Il colore verde indica "almeno un documento presente", non che tutta la normativa del comune sia coperta: da valutare se segnalare la completezza in futuro.
- Il pulsante rosso coincide con il comune "non ancora coperto" di US-7.4: un comune è sempre presente in anagrafica, il rosso indica solo l'assenza di documenti.
- Da decidere se la dashboard sia visibile anche ai visitatori non registrati, per mostrare la copertura ai potenziali clienti.
- La dashboard richiede l'anagrafica completa di regioni, province e comuni precaricata (vedi US-7.4).
