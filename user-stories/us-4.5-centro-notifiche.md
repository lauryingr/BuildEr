# US-4.5 — Centro notifiche e storico

**Attore:** utente registrato (User)
**Necessità:** consultazione di un centro notifiche con lo storico di tutte le notifiche ricevute
**Obiettivo:** nessuna informazione persa anche se il banner è stato chiuso

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Raccoglie le notifiche di [US-4.1](us-4.1-notifica-documento-richiesto.md), [US-4.2](us-4.2-notifica-aggiornamento-preferito.md), [US-4.3](us-4.3-notifica-documento-provincia.md), [US-4.4](us-4.4-notifica-aggiornamento-provincia.md).

## Criteri di accettazione

- **Dato** un utente autenticato, **quando** accede al centro notifiche, **allora** il sistema mostra l'elenco cronologico delle notifiche, dalla più recente.
- **Dato** una notifica in elenco, **quando** viene visualizzata, **allora** il sistema mostra tipo (richiesto, preferito, provincia), comune, documento e data.
- **Dato** una notifica in elenco, **quando** l'utente la seleziona, **allora** il sistema apre il documento collegato.
- **Dato** l'elenco delle notifiche, **quando** l'utente filtra per tipo o per stato, **allora** il sistema mostra solo le notifiche corrispondenti.
- **Dato** una notifica, **quando** l'utente la elimina dallo storico, **allora** il sistema la rimuove solo dal suo elenco.

## Fuori scope

- Notifiche via email o push.
- Impostazioni di frequenza/canale delle notifiche.

## Note

- Da definire per quanto tempo si conserva lo storico.
