# US-4.2 — Notifiche di aggiornamento documento preferito

**Attore:** utente registrato (User) con documenti/comuni tra i preferiti
**Necessità:** notifica in-app quando un documento preferito viene aggiornato
**Obiettivo:** certezza di lavorare sempre sulla versione in vigore della normativa

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (banner di notifica sui preferiti) e archetipo 4.1. Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- Quando viene pubblicata una nuova versione di un documento tra i preferiti, il sistema mostra un banner di notifica indicando documento, comune e data di aggiornamento.
- Quando l'utente apre la notifica, il sistema mostra il documento nella versione aggiornata con data/versione e fonte.
- Se un documento è stato rimosso dai preferiti, il sistema non invia alcuna notifica al suo aggiornamento.

## Fuori scope

- Notifiche via email o push.
- Confronto automatico tra versione precedente e nuova.

## Note

- Le notifiche dipendono dal monitoraggio automatico delle fonti citato nel PRD (sezione 2.1): fuori dal perimetro di questa US.
