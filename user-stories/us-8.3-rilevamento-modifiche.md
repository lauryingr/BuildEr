# US-8.3 — Rilevamento automatico delle modifiche

**Attore:** Sistema di monitoraggio (visibile all'Admin)
**Necessità:** controllo periodico automatico delle fonti configurate per rilevare nuove versioni o nuovi documenti
**Obiettivo:** tempestività nell'individuare le modifiche normative senza controlli manuali

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.2](us-8.2-configurazione-fonti-monitorate.md).

## Criteri di accettazione

- Quando scatta il controllo pianificato di una fonte attiva, il sistema verifica se il documento è cambiato rispetto all'ultima versione registrata.
- Se rileva una modifica, il sistema registra una proposta di aggiornamento in stato "da revisionare" con il nuovo file.
- Se non rileva modifiche, il sistema aggiorna solo la data di ultimo controllo.
- Se la fonte non è raggiungibile o ha cambiato struttura, il sistema registra l'errore e lo segnala nella pagina di monitoraggio.

## Fuori scope

- Interpretazione del contenuto del documento con AI (esclusa dal PRD).
- Pubblicazione automatica senza revisione (vedi US-8.4).

## Note

- Assunzione tecnica: il rilevamento si basa sul confronto del file (es. impronta/hash) o della data pubblicata dalla fonte.
