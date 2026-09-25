# US-1.3 — Eliminazione profilo utente personale

**Come** utente registrato (Admin o User)
**Voglio** poter eliminare il mio profilo personale
**Così da** rimuovere definitivamente il mio account e i miei dati dalla piattaforma quando non ne ho più bisogno

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md). Dipende da [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- **Dato** che sono autenticato, **quando** richiedo l'eliminazione del profilo dalla sezione "Profilo", **allora** mi viene chiesta una conferma esplicita prima di procedere.
- **Dato** che confermo l'eliminazione, **quando** l'operazione va a buon fine, **allora** il mio account e i miei dati personali vengono rimossi e non posso più accedere con quelle credenziali.
- **Dato** un utente che appartiene a uno studio con fascicoli condivisi, **quando** elimina il proprio profilo, **allora** i fascicoli condivisi restano accessibili agli altri membri dello studio (solo l'account personale viene rimosso).

## Fuori scope

- Eliminazione di un profilo da parte dell'Admin per conto di un altro utente (gestione amministrativa, non trattata in questa US).
- Periodo di recupero/undo dopo l'eliminazione (da valutare in futuro).

## Note

- Da definire in futuro la policy di retention/anonimizzazione dei dati dopo l'eliminazione.
