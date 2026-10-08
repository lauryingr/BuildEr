# US-8.5 — Log e storico dei controlli

**Attore:** Admin (super admin)
**Necessità:** consultazione dello storico dei controlli eseguiti e degli errori
**Obiettivo:** diagnosi rapida di fonti che non funzionano e tracciabilità degli aggiornamenti

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.1 (aggiornamento tramite sistema di monitoraggio automatico) e sezione 3 (Admin). Epic di riferimento: [epic-8-monitoraggio-automatico.md](../epics/epic-8-monitoraggio-automatico.md). Tutte le funzioni sono disponibili solo nella pagina riservata al super admin (Admin). Dipende da [US-8.3](us-8.3-rilevamento-modifiche.md).

## Criteri di accettazione

- Quando l'Admin consulta lo storico dei controlli, il sistema mostra per ogni controllo fonte, data/ora, esito (nessuna modifica, aggiornamento rilevato, errore).
- L'Admin può filtrare lo storico per esito, comune o periodo; il sistema mostra solo le voci corrispondenti.
- Se una fonte ha errori ripetuti, il sistema la evidenzia come problematica nell'elenco.

## Fuori scope

- Esportazione dei log (da valutare).

## Note

- Da definire per quanto tempo si conserva lo storico.
