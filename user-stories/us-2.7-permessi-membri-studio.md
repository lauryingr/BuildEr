# US-2.7 — Gestione dei permessi dei membri dello studio

**Attore:** responsabile di uno studio (User)
**Necessità:** assegnazione e modifica dei permessi dei membri sui fascicoli condivisi
**Obiettivo:** controllo su chi può solo consultare e chi può modificare la documentazione dello studio

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (ruoli/permessi per studio) e archetipo 4.2 (junior e senior). Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.5](us-2.5-invito-membri-studio.md).

## Criteri di accettazione

- Il responsabile può assegnare a un membro il permesso "sola consultazione": il membro può visualizzare e scaricare i documenti ma non modificare le cartelle condivise.
- Il responsabile può assegnare a un membro il permesso "modifica": il membro può aggiungere e rimuovere documenti nelle cartelle condivise.
- Quando una modifica di permessi viene salvata, il sistema applica subito i nuovi permessi al membro.
- Se un membro senza permesso di modifica tenta di modificare una cartella condivisa, il sistema nega l'operazione.

## Fuori scope

- Permessi per singolo documento.
- Nuovi ruoli di sistema oltre ad Admin e User.

## Note

- Assunzione: 2 livelli di permesso (consultazione / modifica). I permessi per studio sono distinti dai ruoli di piattaforma (Admin/User).
