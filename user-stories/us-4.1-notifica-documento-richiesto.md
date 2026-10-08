# US-4.1 — Notifiche di aggiunta documento richiesto

**Attore:** utente registrato (User) che ha richiesto l'inserimento di un comune/documento
**Necessità:** notifica in-app quando il documento richiesto viene aggiunto alla piattaforma
**Obiettivo:** informazione tempestiva sulla disponibilità del documento, senza controlli manuali

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (richiesta via form di comuni non presenti, banner di notifica). Epic di riferimento: [epic-4-banner-notifiche.md](../epics/epic-4-banner-notifiche.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md).

## Criteri di accettazione

- Quando il documento richiesto da un utente tramite richiesta di inserimento viene aggiunto alla piattaforma, il sistema mostra all'utente un banner di notifica con il link al documento.
- Quando l'utente apre o chiude una notifica, il sistema la segna come letta e non la ripropone.
- Se ci sono più notifiche non lette, il sistema le mostra in ordine cronologico quando l'utente accede alla piattaforma.

## Fuori scope

- Notifiche via email o push (le notifiche sono in-app).

## Note

- Il PRD parla di "banner di notifica": da confermare se limitato a banner in-app o anche email.
