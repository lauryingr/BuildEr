# US-4.6 — Stato letto/non letto delle notifiche

**Attore:** utente registrato (User)
**Necessità:** distinzione tra notifiche lette e non lette
**Obiettivo:** priorità immediata a ciò che è nuovo

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-4.5](us-4.5-centro-notifiche.md).

## Criteri di accettazione

- Quando viene generata una nuova notifica, il sistema la segna come non letta e mostra un indicatore con il numero di notifiche non lette.
- Quando l'utente apre una notifica non letta, il sistema la segna come letta e aggiorna il contatore.
- L'utente può scegliere "segna tutte come lette"; il sistema segna tutte le notifiche non lette come lette.
- L'utente può segnare una notifica letta come non letta; il sistema ripristina lo stato "non letta".

## Fuori scope

- Sincronizzazione dello stato su più dispositivi (da valutare).

## Note

- Sostituisce il criterio "segnata come letta" già presente in US-4.1: le due story vanno rese coerenti.
