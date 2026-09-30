# US-2.7 — Gestione dei permessi dei membri dello studio

**Attore:** responsabile di uno studio (User)
**Necessità:** assegnazione e modifica dei permessi dei membri sui fascicoli condivisi
**Obiettivo:** controllo su chi può solo consultare e chi può modificare la documentazione dello studio

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (ruoli/permessi per studio) e archetipo 4.2 (junior e senior). Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.5](us-2.5-invito-membri-studio.md).

## Criteri di accettazione

- **Dato** un membro dello studio, **quando** il responsabile gli assegna il permesso "sola consultazione", **allora** il membro può visualizzare e scaricare i documenti ma non modificare le cartelle condivise.
- **Dato** un membro dello studio, **quando** il responsabile gli assegna il permesso "modifica", **allora** il membro può aggiungere e rimuovere documenti nelle cartelle condivise.
- **Dato** una modifica di permessi salvata, **quando** il membro accede alla cartella, **allora** il sistema applica subito i nuovi permessi.
- **Dato** un membro senza permesso di modifica, **quando** tenta di modificare una cartella condivisa, **allora** il sistema nega l'operazione.

## Fuori scope

- Permessi per singolo documento.
- Nuovi ruoli di sistema oltre ad Admin e User.

## Note

- Assunzione: 2 livelli di permesso (consultazione / modifica). I permessi per studio sono distinti dai ruoli di piattaforma (Admin/User).
