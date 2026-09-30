# US-7.4 — Gestione di regioni, province e comuni

**Attore:** Admin (super admin)
**Necessità:** gestione dell'anagrafica territoriale (regioni, province, comuni) su cui si basa l'archivio
**Obiettivo:** archivio organizzato per localizzazione geografica e ampliabile gradualmente

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md).

## Criteri di accettazione

- **Dato** l'anagrafica territoriale, **quando** l'Admin la consulta, **allora** il sistema mostra regioni, province e comuni con il numero di documenti per comune.
- **Dato** un comune non ancora presente, **quando** l'Admin lo aggiunge indicando provincia e regione, **allora** il sistema lo rende selezionabile nei filtri e nell'inserimento documenti.
- **Dato** un comune senza documenti, **quando** l'Admin lo contrassegna come "non ancora coperto", **allora** il sistema lo mostra come tale agli utenti.
- **Dato** un comune con documenti, **quando** l'Admin tenta di eliminarlo, **allora** il sistema lo impedisce.

## Fuori scope

- Import automatico dell'elenco completo dei comuni italiani (da valutare).

## Note

- Il PRD esclude la copertura dei 7900 comuni al lancio: l'anagrafica deve poter crescere gradualmente.
