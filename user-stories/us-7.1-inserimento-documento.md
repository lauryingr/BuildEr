# US-7.1 — Inserimento di un documento

**Attore:** Admin (super admin)
**Necessità:** caricamento di un nuovo documento normativo con i relativi metadati
**Obiettivo:** archivio sempre completo e organizzato per regione, provincia e comune

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md).

## Criteri di accettazione

- **Dato** un Admin autenticato, **quando** compila il modulo di inserimento (file PDF, comune, tipologia, data/versione, fonte con link) e conferma, **allora** il sistema salva il documento e lo rende disponibile agli utenti.
- **Dato** un modulo con campi obbligatori mancanti o file non PDF, **quando** l'Admin tenta il salvataggio, **allora** il sistema mostra un messaggio di errore e non salva.
- **Dato** un documento già presente con stessa tipologia, comune e versione, **quando** l'Admin tenta di inserirlo di nuovo, **allora** il sistema segnala il possibile duplicato.
- **Dato** un documento appena pubblicato, **quando** viene salvato, **allora** il sistema genera le notifiche previste agli utenti interessati (vedi Epic 4).

## Fuori scope

- Inserimento in blocco (import massivo).
- Inserimento tramite rilevazione automatica (vedi Epic 8).

## Note

- Fonti esclusivamente istituzionali: il campo fonte è obbligatorio.
