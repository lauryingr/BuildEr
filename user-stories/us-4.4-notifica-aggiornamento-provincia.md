# US-4.4 — Notifiche di aggiornamento documento provincia

**Attore:** utente registrato (User) con una provincia di interesse impostata
**Necessità:** notifica in-app quando un documento già presente della provincia viene aggiornato
**Obiettivo:** aggiornamento costante sulle modifiche normative nelle province di interesse

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- Quando un documento di un comune di una provincia di interesse viene aggiornato, il sistema mostra un banner di notifica con comune, documento e data di aggiornamento.
- Quando l'utente apre la notifica, il sistema mostra il documento nella versione aggiornata.
- Se il documento è già stato notificato tramite i preferiti (US-4.2), il sistema mostra una sola notifica, senza duplicati.

## Fuori scope

- Notifiche via email o push.

## Note

- Da valutare se accorpare US-4.3 e US-4.4 in un'unica story: cambiano solo il trigger (nuovo vs aggiornato).
