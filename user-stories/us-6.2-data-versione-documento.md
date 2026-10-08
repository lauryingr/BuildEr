# US-6.2 — Data e versione di ultimo aggiornamento

**Attore:** utente registrato (User)
**Necessità:** visualizzazione della data/versione di ultimo aggiornamento di ogni documento
**Obiettivo:** certezza di consultare la normativa in vigore, senza verifiche manuali sul sito del comune

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 (data/versione e fonte visibili su ogni documento, download PDF) e archetipo 4.1 (Elia). Epic di riferimento: [epic-6-consultazione-documento.md](../epics/epic-6-consultazione-documento.md). Dipende da [US-6.1](us-6.1-scheda-documento.md).

## Criteri di accettazione

- Il sistema mostra sempre la data/versione di ultimo aggiornamento di un documento, sia nella scheda sia negli elenchi.
- Se è stata pubblicata una nuova versione, quando l'utente apre il documento il sistema mostra la versione più recente in vigore.
- Se la data di aggiornamento non è nota, il sistema indica esplicitamente "data non disponibile" invece di lasciare il campo vuoto.
- Per un documento aggiornato di recente, il sistema mostra anche la data di ultimo controllo sulla fonte.

## Fuori scope

- Confronto automatico tra versioni.
- Storico completo delle versioni precedenti (da valutare in futuro).

## Note

- Da chiarire se "data" indica la data del provvedimento, di pubblicazione sulla fonte o di caricamento su BuildEr: sono tre informazioni diverse.
