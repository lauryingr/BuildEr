# US-7.2 — Modifica di un documento

**Attore:** Admin (super admin)
**Necessità:** modifica dei metadati o del file di un documento esistente
**Obiettivo:** correzione di errori e pubblicazione di nuove versioni

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 3 "Ruoli utente" (Admin: gestione completa della piattaforma e degli utenti). Epic di riferimento: [epic-7-amministrazione-contenuti.md](../epics/epic-7-amministrazione-contenuti.md). Dipende da [US-7.1](us-7.1-inserimento-documento.md).

## Criteri di accettazione

- L'Admin può modificare i metadati di un documento esistente (es. tipologia, fonte); quando salva, il sistema aggiorna i dati.
- L'Admin può caricare un nuovo file come nuova versione di un documento; il sistema aggiorna data/versione e mantiene i riferimenti nelle cartelle e nei preferiti degli utenti.
- Quando una nuova versione viene salvata, il sistema genera le notifiche di aggiornamento (vedi Epic 4).

## Fuori scope

- Modifica dei documenti da parte degli utenti User.

## Note

- Da decidere se conservare le versioni precedenti (archivio storico).
