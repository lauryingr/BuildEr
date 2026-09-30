# US-4.6 — Stato letto/non letto delle notifiche

**Attore:** utente registrato (User)
**Necessità:** distinzione tra notifiche lette e non lette
**Obiettivo:** priorità immediata a ciò che è nuovo

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-4.5](us-4.5-centro-notifiche.md).

## Criteri di accettazione

- **Dato** una nuova notifica, **quando** viene generata, **allora** il sistema la segna come non letta e mostra un indicatore con il numero di notifiche non lette.
- **Dato** una notifica non letta, **quando** l'utente la apre, **allora** il sistema la segna come letta e aggiorna il contatore.
- **Dato** più notifiche non lette, **quando** l'utente sceglie "segna tutte come lette", **allora** il sistema le segna tutte come lette.
- **Dato** una notifica letta, **quando** l'utente la segna come non letta, **allora** il sistema ripristina lo stato "non letta".

## Fuori scope

- Sincronizzazione dello stato su più dispositivi (da valutare).

## Note

- Sostituisce il criterio "segnata come letta" già presente in US-4.1: le due story vanno rese coerenti.
