# US-2.4 — Creazione studio

**Attore:** utente registrato (User)
**Necessità:** creazione di uno studio (gruppo di lavoro) sulla piattaforma
**Obiettivo:** base per la condivisione di fascicoli e preferiti tra colleghi

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (gestione multi-utente/permessi per studio) e archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Prerequisito di [US-2.2](us-2.2-condivisione-fascicoli.md).

## Criteri di accettazione

- **Dato** un utente autenticato non ancora associato a uno studio, **quando** crea uno studio indicando il nome, **allora** il sistema crea lo studio e assegna all'utente il ruolo di responsabile dello studio.
- **Dato** la creazione di uno studio, **quando** il nome è vuoto, **allora** il sistema mostra un messaggio di errore e non crea lo studio.
- **Dato** uno studio appena creato, **quando** viene visualizzato, **allora** il sistema mostra l'elenco dei membri, inizialmente composto solo dal creatore.

## Fuori scope

- Fatturazione o piani a pagamento per studio.
- Appartenenza di un utente a più studi (da valutare).

## Note

- Il PRD non definisce lo "studio" come entità: assunzione che sia un gruppo di User con un responsabile. Il ruolo di responsabile studio non è un ruolo di sistema (i ruoli restano Admin e User).
