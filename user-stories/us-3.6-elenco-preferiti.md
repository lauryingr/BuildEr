# US-3.6 — Elenco e visualizzazione dei preferiti

**Attore:** utente registrato (User)
**Necessità:** consultazione dell'elenco dei documenti/comuni salvati tra i preferiti
**Obiettivo:** accesso rapido ai contenuti più usati, con evidenza degli aggiornamenti

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (salvataggio dei comuni più utilizzati) e archetipo 4.1. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- Un utente con preferiti salvati può accedere alla sezione "Preferiti", dove il sistema mostra l'elenco con nome del documento, comune, data/versione di aggiornamento.
- L'utente può raggruppare o filtrare i preferiti per comune, provincia o tipologia; il sistema mostra solo gli elementi corrispondenti.
- Quando l'utente seleziona un elemento dell'elenco, il sistema apre la scheda del documento (vedi [US-6.1](us-6.1-scheda-documento.md)).
- Se un documento preferito è stato aggiornato di recente, il sistema lo evidenzia come aggiornato nell'elenco.
- Se non ci sono preferiti salvati, il sistema mostra un messaggio informativo.

## Fuori scope

- Aggiunta e rimozione dei preferiti (vedi US-3.2).
- Preferiti condivisi con altri utenti.

## Note

- Da confermare se i preferiti sono a livello di documento o di comune (vedi US-3.2).
