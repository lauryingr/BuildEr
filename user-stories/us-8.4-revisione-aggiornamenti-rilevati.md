# US-8.4 — Revisione e approvazione degli aggiornamenti rilevati

**Attore:** Admin (super admin)
**Necessità:** revisione manuale degli aggiornamenti proposti dal monitoraggio prima della pubblicazione
**Obiettivo:** garanzia che gli utenti vedano solo documenti verificati e realmente in vigore

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.3](us-8.3-rilevamento-modifiche.md); alla pubblicazione generano le notifiche dell'Epic 4.

## Criteri di accettazione

- **Dato** un aggiornamento proposto, **quando** l'Admin lo apre, **allora** il sistema mostra fonte, data rilevamento, nuovo file e documento attualmente pubblicato.
- **Dato** un aggiornamento proposto, **quando** l'Admin lo approva, **allora** il sistema pubblica la nuova versione, aggiorna data/versione e genera le notifiche agli utenti interessati.
- **Dato** un aggiornamento proposto, **quando** l'Admin lo rifiuta, **allora** il sistema lo scarta senza modificare il documento pubblicato.
- **Dato** un elenco di aggiornamenti in attesa, **quando** l'Admin accede alla pagina, **allora** il sistema li mostra ordinati per data di rilevamento.

## Fuori scope

- Approvazione automatica basata su regole (da valutare).

## Note

- Assunzione: revisione umana obbligatoria, coerente con l'obiettivo di garantire la versione in vigore.
