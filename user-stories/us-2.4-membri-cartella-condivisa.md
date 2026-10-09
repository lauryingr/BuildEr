# US-2.4 — Elenco membri e uscita da una cartella condivisa

**Attore:** utente registrato (User) membro di una cartella condivisa
**Necessità:** visualizzazione di chi ha accesso alla cartella e possibilità di lasciarla
**Obiettivo:** trasparenza su chi vede i documenti raccolti e libertà di uscire da un team

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 6.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.2](us-2.2-condivisione-fascicoli.md). Sostituisce le precedenti US su creazione studio, rimozione membri e permessi (non più previste: tutti i membri sono pari).

## Criteri di accettazione

- Un membro può vedere l'elenco dei membri della cartella (nome ed email) e degli inviti in attesa.
- Un membro può scegliere "Esci dalla cartella"; il sistema chiede una conferma esplicita e, se confermata, lo rimuove dall'elenco dei membri e gli toglie subito l'accesso.
- Quando un membro esce, la cartella e i documenti restano accessibili agli altri membri, senza alcuna modifica.
- Se chi esce è l'ultimo membro, il sistema elimina la cartella (i documenti della piattaforma non vengono toccati); il sistema avvisa l'utente nella conferma.
- Dopo l'uscita il sistema mantiene l'account personale e le altre cartelle dell'utente.

## Fuori scope

- Rimozione di un altro membro da parte di un membro (vedi nota di [US-2.2](us-2.2-condivisione-fascicoli.md)).
- Ripristino dell'accesso senza un nuovo invito.

## Note

- Coerenza con [US-1.3](us-1.3-eliminazione-profilo.md) e [US-3.5](us-3.5-eliminazione-cartelle-personalizzate.md): l'eliminazione del profilo equivale all'uscita da tutte le cartelle.
