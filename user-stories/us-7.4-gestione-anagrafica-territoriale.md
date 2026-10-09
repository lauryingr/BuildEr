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
- Un comune senza documenti risulta "non ancora coperto" e viene mostrato in rosso agli utenti nella dashboard ([US-3.7](us-3.7-dashboard-copertura-territoriale.md)); diventa verde quando viene inserito il primo documento. Lo stato è calcolato dal sistema, non impostato a mano.
- Se l'Admin tenta di eliminare un comune con documenti, il sistema lo impedisce.

## Fuori scope


## Note

- Il PRD esclude la copertura dei 7900 comuni al lancio: i documenti crescono gradualmente, ma l'anagrafica di 20 regioni, province e comuni deve essere precaricata per intero fin dal lancio, perché la dashboard della home mostra anche i comuni senza documenti. L'import iniziale dell'elenco è quindi prerequisito.
- Aggiungere un comune serve solo per variazioni successive (es. nuovi comuni da fusione).
