# US-7.1 — Inserimento di un documento

**Attore:** Admin (super admin)
**Necessità:** caricamento di un nuovo documento normativo con i relativi metadati
**Obiettivo:** archivio sempre completo e organizzato per regione, provincia e comune

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md).

## Criteri di accettazione

- Un Admin autenticato può compilare il modulo di inserimento (file PDF, comune, tipologia, data/versione, fonte con link) e confermare; il sistema salva il documento e lo rende disponibile agli utenti.
- Se mancano campi obbligatori o il file non è un PDF, il sistema mostra un messaggio di errore e non salva.
- Se esiste già un documento con stessa tipologia, comune e versione, il sistema segnala il possibile duplicato.
- Quando un documento viene pubblicato, il sistema genera le notifiche previste agli utenti interessati (vedi Epic 4).

## Fuori scope

- Inserimento in blocco (import massivo).
- Inserimento tramite rilevazione automatica (vedi Epic 8).

## Note

- Fonti esclusivamente istituzionali: il campo fonte è obbligatorio.
