# US-4.2 — Notifiche di aggiornamento documento preferito

**Attore:** utente registrato (User) con documenti/comuni tra i preferiti
**Necessità:** notifica in-app quando un documento preferito viene aggiornato
**Obiettivo:** certezza di lavorare sempre sulla versione in vigore della normativa

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica sui preferiti) e archetipo 4.1. Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- **Dato** un documento tra i preferiti, **quando** viene pubblicata una nuova versione, **allora** il sistema mostra un banner di notifica indicando documento, comune e data di aggiornamento.
- **Dato** una notifica di aggiornamento, **quando** l'utente la apre, **allora** il sistema mostra il documento nella versione aggiornata con data/versione e fonte.
- **Dato** un documento rimosso dai preferiti, **quando** viene aggiornato, **allora** il sistema non invia alcuna notifica.

## Fuori scope

- Notifiche via email o push.
- Confronto automatico tra versione precedente e nuova.

## Note

- Le notifiche dipendono dal monitoraggio automatico delle fonti citato nel PRD (sezione 2.1): fuori dal perimetro di questa US.
