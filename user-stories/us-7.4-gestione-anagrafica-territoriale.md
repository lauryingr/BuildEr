# US-7.4 — Gestione di regioni, province e comuni

**Attore:** Admin (super admin)
**Necessità:** gestione dell'anagrafica territoriale (regioni, province, comuni) su cui si basa l'archivio
**Obiettivo:** archivio organizzato per localizzazione geografica e ampliabile gradualmente

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md).

## Criteri di accettazione

- L'Admin può consultare l'anagrafica territoriale; il sistema mostra regioni, province e comuni con il numero di documenti per comune.
- L'Admin può aggiungere un comune non ancora presente indicando provincia e regione; il sistema lo rende selezionabile nei filtri e nell'inserimento documenti.
- L'Admin può contrassegnare un comune senza documenti come "non ancora coperto"; il sistema lo mostra come tale agli utenti.
- Se l'Admin tenta di eliminare un comune con documenti, il sistema lo impedisce.

## Fuori scope

- Import automatico dell'elenco completo dei comuni italiani (da valutare).

## Note

- Il PRD esclude la copertura dei 7900 comuni al lancio: l'anagrafica deve poter crescere gradualmente.
