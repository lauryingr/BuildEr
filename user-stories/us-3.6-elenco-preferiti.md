# US-3.6 — Elenco e visualizzazione dei preferiti

**Attore:** utente registrato (User)
**Necessità:** consultazione dell'elenco dei documenti/comuni salvati tra i preferiti
**Obiettivo:** accesso rapido ai contenuti più usati, con evidenza degli aggiornamenti

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (salvataggio dei comuni più utilizzati) e archetipo 4.1. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- **Dato** un utente con preferiti salvati, **quando** accede alla sezione "Preferiti", **allora** il sistema mostra l'elenco con nome del documento, comune, data/versione di aggiornamento.
- **Dato** un elenco di preferiti, **quando** l'utente li raggruppa o filtra per comune, provincia o tipologia, **allora** il sistema mostra solo gli elementi corrispondenti.
- **Dato** un elemento dell'elenco, **quando** l'utente lo seleziona, **allora** il sistema apre la scheda del documento (vedi [US-6.1](us-6.1-scheda-documento.md)).
- **Dato** un documento preferito aggiornato di recente, **quando** l'elenco viene visualizzato, **allora** il sistema lo evidenzia come aggiornato.
- **Dato** nessun preferito salvato, **quando** l'utente accede alla sezione, **allora** il sistema mostra un messaggio informativo.

## Fuori scope

- Aggiunta e rimozione dei preferiti (vedi US-3.2).
- Preferiti condivisi con lo studio.

## Note

- Da confermare se i preferiti sono a livello di documento o di comune (vedi US-3.2).
