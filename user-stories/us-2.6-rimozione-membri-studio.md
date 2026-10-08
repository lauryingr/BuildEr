# US-2.6 — Rimozione di membri dallo studio

**Attore:** responsabile di uno studio (User)
**Necessità:** rimozione di un membro dallo studio
**Obiettivo:** controllo su chi accede ai fascicoli condivisi

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.5](us-2.5-invito-membri-studio.md).

## Criteri di accettazione

- Il responsabile può richiedere la rimozione di un membro dello studio; il sistema chiede una conferma esplicita.
- Se il responsabile conferma e l'operazione va a buon fine, il membro perde l'accesso a tutte le cartelle condivise dello studio.
- Quando un membro viene rimosso, il sistema mantiene il suo account personale e le sue cartelle private.
- Un membro può richiedere di lasciare lo studio; il sistema lo rimuove dall'elenco dei membri.
- Se il responsabile tenta di rimuovere se stesso senza aver designato un altro responsabile, il sistema blocca l'operazione.

## Fuori scope

- Eliminazione dell'intero studio (da valutare in futuro).

## Note

- Coerenza con US-1.3: le cartelle condivise restano accessibili ai membri rimasti.
