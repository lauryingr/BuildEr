# US-7.5 — Gestione delle richieste di nuovo comune

**Attore:** Admin (super admin)
**Necessità:** consultazione e gestione delle richieste di inserimento di nuovi comuni inviate dagli utenti
**Obiettivo:** evasione ordinata delle richieste e informazione all'utente richiedente

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-5.2](us-5.2-richiesta-nuovo-comune.md); alimenta [US-4.1](us-4.1-notifica-documento-richiesto.md).

## Criteri di accettazione

- Nella sezione dedicata l'Admin vede le richieste ricevute con comune, utente richiedente, data e stato (aperta, in lavorazione, evasa, rifiutata).
- Se ci sono più richieste per lo stesso comune, il sistema le raggruppa indicando il numero di richiedenti.
- L'Admin può cambiare lo stato di una richiesta; il sistema salva il nuovo stato.
- Quando l'Admin chiude una richiesta evasa (documenti inseriti), il sistema notifica gli utenti richiedenti.

## Fuori scope

- Risposta diretta all'utente via chat o email.

## Note

- Il raggruppamento per comune aiuta a dare priorità ai comuni più richiesti.
