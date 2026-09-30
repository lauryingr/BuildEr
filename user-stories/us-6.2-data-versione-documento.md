# US-6.2 — Data e versione di ultimo aggiornamento

**Attore:** utente registrato (User)
**Necessità:** visualizzazione della data/versione di ultimo aggiornamento di ogni documento
**Obiettivo:** certezza di consultare la normativa in vigore, senza verifiche manuali sul sito del comune

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (data/versione e fonte visibili su ogni documento, download PDF) e archetipo 4.1 (Elia). Epic di riferimento: [epic-6-consultazione-documento.md](../epics/epic-6-consultazione-documento.md). Dipende da [US-6.1](us-6.1-scheda-documento.md).

## Criteri di accettazione

- **Dato** un documento, **quando** viene visualizzato (scheda o elenco), **allora** il sistema mostra sempre la data/versione di ultimo aggiornamento.
- **Dato** un documento con una nuova versione pubblicata, **quando** l'utente lo apre, **allora** il sistema mostra la versione più recente in vigore.
- **Dato** un documento senza data di aggiornamento nota, **quando** viene visualizzato, **allora** il sistema indica esplicitamente "data non disponibile" invece di lasciare il campo vuoto.
- **Dato** un documento aggiornato di recente, **quando** viene visualizzato, **allora** il sistema mostra la data di ultimo controllo sulla fonte.

## Fuori scope

- Confronto automatico tra versioni.
- Storico completo delle versioni precedenti (da valutare in futuro).

## Note

- Da chiarire se "data" indica la data del provvedimento, di pubblicazione sulla fonte o di caricamento su BuildEr: sono tre informazioni diverse.
