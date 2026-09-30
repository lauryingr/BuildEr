# US-2.6 — Rimozione di membri dallo studio

**Attore:** responsabile di uno studio (User)
**Necessità:** rimozione di un membro dallo studio
**Obiettivo:** controllo su chi accede ai fascicoli condivisi

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.5](us-2.5-invito-membri-studio.md).

## Criteri di accettazione

- **Dato** un membro dello studio, **quando** il responsabile ne richiede la rimozione, **allora** il sistema chiede una conferma esplicita.
- **Dato** una conferma di rimozione, **quando** l'operazione va a buon fine, **allora** il membro perde l'accesso a tutte le cartelle condivise dello studio.
- **Dato** un membro rimosso, **quando** viene rimosso, **allora** il sistema mantiene il suo account personale e le sue cartelle private.
- **Dato** un membro che vuole lasciare lo studio, **quando** ne fa richiesta, **allora** il sistema lo rimuove dall'elenco dei membri.
- **Dato** il responsabile dello studio, **quando** tenta di rimuovere se stesso senza aver designato un altro responsabile, **allora** il sistema blocca l'operazione.

## Fuori scope

- Eliminazione dell'intero studio (da valutare in futuro).

## Note

- Coerenza con US-1.3: le cartelle condivise restano accessibili ai membri rimasti.
