# US-6.3 — Fonte ufficiale del documento

**Attore:** utente registrato (User)
**Necessità:** visualizzazione della fonte istituzionale da cui proviene ogni documento
**Obiettivo:** verifica dell'attendibilità del documento e possibilità di risalire alla fonte originale

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (data/versione e fonte visibili su ogni documento, download PDF) e archetipo 4.1 (Elia). Epic di riferimento: [epic-6-consultazione-documento.md](../epics/epic-6-consultazione-documento.md). Dipende da [US-6.1](us-6.1-scheda-documento.md).

## Criteri di accettazione

- **Dato** un documento, **quando** viene visualizzato, **allora** il sistema mostra la fonte di provenienza (es. sito istituzionale del comune, BUR regionale, normativa nazionale).
- **Dato** l'indicazione della fonte, **quando** l'utente la seleziona, **allora** il sistema apre il link alla pagina originale in una nuova scheda.
- **Dato** un link alla fonte non più raggiungibile, **quando** l'utente lo seleziona, **allora** il sistema segnala che la fonte non è raggiungibile mantenendo l'indicazione testuale.

## Fuori scope

- Documenti da fonti non istituzionali (esclusi per principio).

## Note

- Le fonti sono esclusivamente istituzionali (PRD, sezione 2.1).
