# US-7.5 — Gestione delle richieste di nuovo comune

**Attore:** Admin (super admin)
**Necessità:** consultazione e gestione delle richieste di inserimento di nuovi comuni inviate dagli utenti
**Obiettivo:** evasione ordinata delle richieste e informazione all'utente richiedente

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md); alimenta [US-4.1](us-4.1-notifica-documento-richiesto.md).

## Criteri di accettazione

- **Dato** le richieste ricevute, **quando** l'Admin accede alla sezione dedicata, **allora** il sistema le mostra con comune, utente richiedente, data e stato (aperta, in lavorazione, evasa, rifiutata).
- **Dato** più richieste per lo stesso comune, **quando** l'elenco viene visualizzato, **allora** il sistema le raggruppa indicando il numero di richiedenti.
- **Dato** una richiesta, **quando** l'Admin ne cambia lo stato, **allora** il sistema salva il nuovo stato.
- **Dato** una richiesta evasa (documenti inseriti), **quando** l'Admin la chiude, **allora** il sistema notifica gli utenti richiedenti.

## Fuori scope

- Risposta diretta all'utente via chat o email.

## Note

- Il raggruppamento per comune aiuta a dare priorità ai comuni più richiesti.
