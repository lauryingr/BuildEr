# US-1.3 — Eliminazione profilo utente personale

**Attore:** utente registrato (Admin o User)
**Necessità:** eliminazione del profilo personale
**Obiettivo:** rimozione definitiva dell'account e dei dati personali dalla piattaforma

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.1 (Elia). Epic di riferimento: [epic-1-profilo-utente.md](../epics/epic-1-profilo-utente.md). Dipende da [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- Un utente autenticato può richiedere l'eliminazione del proprio profilo dalla sezione "Profilo"; il sistema chiede una conferma esplicita prima di procedere.
- Se l'utente conferma e l'operazione va a buon fine, il sistema rimuove account e dati personali e le credenziali non consentono più l'accesso.
- Se l'utente è membro di cartelle condivise, l'eliminazione equivale all'uscita da ciascuna: le cartelle restano accessibili agli altri membri. Le cartelle di cui era l'unico membro vengono eliminate.

## Fuori scope

- Eliminazione di un profilo da parte dell'Admin per conto di un altro utente (gestione amministrativa, non trattata in questa US).
- Periodo di recupero/undo dopo l'eliminazione (da valutare in futuro).

## Note

- Da definire in futuro la policy di retention/anonimizzazione dei dati dopo l'eliminazione.
