# US-8.2 — Configurazione delle fonti da monitorare

**Attore:** Admin (super admin)
**Necessità:** definizione delle fonti istituzionali da monitorare per ogni comune e tipologia di documento
**Obiettivo:** monitoraggio mirato delle sole fonti ufficiali

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.1](us-8.1-pagina-monitoraggio.md).

## Criteri di accettazione

- **Dato** la pagina di monitoraggio, **quando** l'Admin aggiunge una fonte indicando comune, tipologia di documento e URL, **allora** il sistema salva la fonte e la include nei controlli successivi.
- **Dato** una fonte esistente, **quando** l'Admin la modifica, la disattiva o la elimina, **allora** il sistema applica la modifica dal controllo successivo.
- **Dato** un URL non valido o duplicato, **quando** l'Admin tenta il salvataggio, **allora** il sistema mostra un messaggio di errore.
- **Dato** una fonte configurata, **quando** l'Admin imposta la frequenza di controllo, **allora** il sistema la utilizza per pianificare i controlli.

## Fuori scope

- Fonti non istituzionali.

## Note

- Da definire le frequenze di controllo disponibili (es. giornaliera, settimanale).
