# US-4.3 — Notifiche di aggiunta documento provincia

**Attore:** utente registrato (User) con una provincia di interesse impostata
**Necessità:** notifica in-app quando viene aggiunto un nuovo documento relativo alla provincia
**Obiettivo:** scoperta tempestiva di nuovi contenuti nelle province in cui si lavora

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-3.2](us-3.2-preferenza-documenti-provincia.md).

## Criteri di accettazione

- **Dato** una provincia di interesse impostata, **quando** viene aggiunto un nuovo documento (o un nuovo comune) della provincia, **allora** il sistema mostra un banner di notifica con comune e tipologia di documento.
- **Dato** una notifica ricevuta, **quando** l'utente la apre, **allora** il sistema porta al documento aggiunto.
- **Dato** una provincia non impostata come di interesse, **quando** viene aggiunto un documento, **allora** il sistema non invia alcuna notifica.

## Fuori scope

- Notifiche via email o push.

## Note

- Assunzione: la "provincia" è quella impostata nelle preferenze (US-3.2), non dedotta dal profilo.
