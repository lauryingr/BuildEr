# US-8.2 — Configurazione delle fonti da monitorare

**Attore:** Admin (super admin)
**Necessità:** definizione delle fonti istituzionali da monitorare per ogni comune e tipologia di documento
**Obiettivo:** monitoraggio mirato delle sole fonti ufficiali

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.1](us-8.1-pagina-monitoraggio.md).

## Criteri di accettazione

- Dalla pagina di monitoraggio l'Admin può aggiungere una fonte indicando comune, tipologia di documento e URL; il sistema salva la fonte e la include nei controlli successivi.
- L'Admin può modificare, disattivare o eliminare una fonte esistente; il sistema applica la modifica dal controllo successivo.
- Se l'URL non è valido o è duplicato, il sistema mostra un messaggio di errore al tentativo di salvataggio.
- L'Admin può impostare la frequenza di controllo di una fonte; il sistema la utilizza per pianificare i controlli.

## Fuori scope

- Fonti non istituzionali.

## Note

- Da definire le frequenze di controllo disponibili (es. giornaliera, settimanale).
