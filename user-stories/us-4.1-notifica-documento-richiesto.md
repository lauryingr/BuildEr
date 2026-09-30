# US-4.1 — Notifiche di aggiunta documento richiesto

**Attore:** utente registrato (User) che ha richiesto l'inserimento di un comune/documento
**Necessità:** notifica in-app quando il documento richiesto viene aggiunto alla piattaforma
**Obiettivo:** informazione tempestiva sulla disponibilità del documento, senza controlli manuali

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (richiesta via form di comuni non presenti, banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md).

## Criteri di accettazione

- **Dato** una richiesta di inserimento inviata dall'utente, **quando** il documento richiesto viene aggiunto alla piattaforma, **allora** il sistema mostra all'utente un banner di notifica con il link al documento.
- **Dato** una notifica ricevuta, **quando** l'utente la apre o la chiude, **allora** il sistema la segna come letta e non la ripropone.
- **Dato** più notifiche non lette, **quando** l'utente accede alla piattaforma, **allora** il sistema le mostra in ordine cronologico.

## Fuori scope

- Notifiche via email o push (le notifiche sono in-app).

## Note

- Il PRD parla di "banner di notifica": da confermare se limitato a banner in-app o anche email.
