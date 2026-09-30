# US-6.1 — Scheda di dettaglio del documento

**Attore:** utente registrato (User)
**Necessità:** apertura della scheda di dettaglio di un documento normativo
**Obiettivo:** visione in un unico punto di tutte le informazioni sul documento

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (data/versione e fonte visibili su ogni documento, download PDF) e archetipo 4.1 (Elia). Epic di riferimento: [epic-6-consultazione-documento.md](../epics/epic-6-consultazione-documento.md). Punto di ingresso da [US-3.1](us-3.1-ricerca-filtri-documenti.md) e [US-3.6](us-3.6-elenco-preferiti.md).

## Criteri di accettazione

- **Dato** un documento in elenco (ricerca, preferiti, cartella, notifica), **quando** l'utente lo seleziona, **allora** il sistema apre la scheda di dettaglio.
- **Dato** la scheda di dettaglio, **quando** viene visualizzata, **allora** il sistema mostra titolo, tipologia, comune, provincia, regione, data/versione e fonte.
- **Dato** la scheda di dettaglio, **quando** viene visualizzata, **allora** il sistema offre le azioni di download, aggiunta ai preferiti e aggiunta a cartella.
- **Dato** un documento non più disponibile, **quando** l'utente tenta di aprirlo, **allora** il sistema mostra un messaggio chiaro.

## Fuori scope

- Modifica del documento (riservata all'Admin, vedi Epic 7).

## Note

- Nessuna nota aggiuntiva al momento.
