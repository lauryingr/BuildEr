# US-3.5 — Eliminazione di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) membro di una cartella
**Necessità:** eliminazione di una cartella non più necessaria o uscita da una cartella condivisa
**Obiettivo:** area personale ordinata, senza cartelle obsolete

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md). Per le cartelle condivise vedi [US-2.4](us-2.4-membri-cartella-condivisa.md).

## Criteri di accettazione

- Su una cartella di cui è l'unico membro, l'utente può richiedere l'eliminazione; il sistema chiede una conferma esplicita e, se confermata, la cartella scompare e i documenti in essa contenuti restano disponibili nella piattaforma.
- Su una cartella con più membri, l'azione disponibile è "Esci dalla cartella" (US-2.4): la cartella scompare solo dall'elenco dell'utente e resta accessibile agli altri membri. Nessun membro può eliminare la cartella per tutti.
- Quando l'ultimo membro esce, la cartella viene eliminata definitivamente.
- Se un utente che non è membro tenta di eliminare o lasciare la cartella, il sistema nega l'operazione.

## Fuori scope

- Eliminazione di una cartella condivisa per tutti i membri contemporaneamente.
- Recupero di cartelle eliminate (undo/cestino).

## Note

- Scelta di prodotto: poiché i membri sono pari, nessuno può distruggere il lavoro degli altri.
- Coerenza con US-1.3: l'eliminazione del profilo equivale all'uscita da tutte le cartelle.
