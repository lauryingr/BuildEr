# US-8.6 — Avvio manuale del controllo di una fonte

**Attore:** Admin (super admin)
**Necessità:** avvio di un controllo immediato su una o più fonti, fuori dalla pianificazione
**Obiettivo:** verifica puntuale quando si sospetta una modifica o dopo la correzione di un errore

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.2](us-8.2-configurazione-fonti-monitorate.md).

## Criteri di accettazione

- L'Admin può avviare il controllo manuale di una fonte configurata; il sistema esegue subito il controllo e ne mostra l'esito.
- Se è già in corso un controllo manuale sulla stessa fonte, il sistema impedisce di avviarne un altro.
- Quando un controllo manuale si conclude, il sistema lo riporta nello storico (vedi [US-8.5](us-8.5-log-monitoraggio.md)).

## Fuori scope

- Controllo manuale da parte di utenti User.

## Note

- Nessuna nota aggiuntiva al momento.
