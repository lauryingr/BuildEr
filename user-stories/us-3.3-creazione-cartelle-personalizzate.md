# US-3.3 — Creazione di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User)
**Necessità:** creazione di una cartella personalizzata, con possibilità di renderla condivisibile con i colleghi
**Obiettivo:** organizzazione dei documenti per commessa/comune, singolarmente o insieme allo studio

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Collegata a [US-2.1](us-2.1-cartelle-personalizzabili.md) e [US-2.2](us-2.2-condivisione-fascicoli.md).

## Criteri di accettazione

- Un utente autenticato può creare una cartella indicando un nome; il sistema crea la cartella, inizialmente privata.
- L'utente può impostare una cartella appena creata come condivisibile e selezionare dei colleghi; il sistema la rende accessibile ai colleghi selezionati.
- Se il nome è vuoto o già usato da un'altra cartella dello stesso utente, il sistema mostra un messaggio di errore e non crea la cartella.

## Fuori scope

- Modifica ed eliminazione delle cartelle (vedi US-3.4 e US-3.5).

## Note

- Sovrapposizione con US-2.1 (creazione cartelle) e US-2.2 (condivisione): da valutare se accorpare o distinguere chiaramente i perimetri.
