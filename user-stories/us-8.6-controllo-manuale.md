# US-8.6 — Avvio manuale del controllo di una fonte

**Attore:** Admin (super admin)
**Necessità:** avvio di un controllo immediato su una o più fonti, fuori dalla pianificazione
**Obiettivo:** verifica puntuale quando si sospetta una modifica o dopo la correzione di un errore

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.2](us-8.2-configurazione-fonti-monitorate.md).

## Criteri di accettazione

- **Dato** una fonte configurata, **quando** l'Admin avvia il controllo manuale, **allora** il sistema esegue subito il controllo e ne mostra l'esito.
- **Dato** un controllo manuale in corso sulla stessa fonte, **quando** l'Admin tenta di avviarne un altro, **allora** il sistema lo impedisce.
- **Dato** un controllo manuale concluso, **quando** viene registrato, **allora** il sistema lo riporta nello storico (vedi [US-8.5](us-8.5-log-monitoraggio.md)).

## Fuori scope

- Controllo manuale da parte di utenti User.

## Note

- Nessuna nota aggiuntiva al momento.
