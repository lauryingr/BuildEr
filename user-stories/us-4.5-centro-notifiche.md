# US-4.5 — Centro notifiche e storico

**Attore:** utente registrato (User)
**Necessità:** consultazione di un centro notifiche con lo storico di tutte le notifiche ricevute
**Obiettivo:** nessuna informazione persa anche se il banner è stato chiuso

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Raccoglie le notifiche di [US-4.1](us-4.1-notifica-documento-richiesto.md), [US-4.2](us-4.2-notifica-aggiornamento-preferito.md), [US-4.3](us-4.3-notifica-documento-provincia.md), [US-4.4](us-4.4-notifica-aggiornamento-provincia.md), [US-4.7](us-4.7-notifica-invito-cartella.md).

## Criteri di accettazione

- Un utente autenticato può accedere al centro notifiche, dove il sistema mostra l'elenco cronologico delle notifiche, dalla più recente.
- Per ogni notifica il sistema mostra tipo (richiesto, preferito, provincia, invito cartella), comune, documento e data.
- Quando l'utente seleziona una notifica, il sistema apre il documento collegato.
- L'utente può filtrare le notifiche per tipo o per stato; il sistema mostra solo quelle corrispondenti.
- L'utente può eliminare una notifica dallo storico; il sistema la rimuove solo dal suo elenco.

## Fuori scope

- Notifiche via email o push.
- Impostazioni di frequenza/canale delle notifiche.

## Note

- Da definire per quanto tempo si conserva lo storico.
