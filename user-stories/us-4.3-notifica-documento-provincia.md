# US-4.3 — Notifiche di aggiunta documento provincia

**Attore:** utente registrato (User) con una provincia di interesse impostata
**Necessità:** notifica in-app quando viene aggiunto un nuovo documento relativo alla provincia
**Obiettivo:** scoperta tempestiva di nuovi contenuti nelle province in cui si lavora

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- Quando viene aggiunto un nuovo documento (o un nuovo comune) di una provincia di interesse, il sistema mostra un banner di notifica con comune e tipologia di documento.
- Quando l'utente apre la notifica, il sistema lo porta al documento aggiunto.
- Se la provincia non è impostata come di interesse, il sistema non invia alcuna notifica all'aggiunta di un documento.

## Fuori scope

- Notifiche via email o push.

## Note

- Assunzione: la "provincia" è quella impostata nelle preferenze (US-3.2), non dedotta dal profilo.
