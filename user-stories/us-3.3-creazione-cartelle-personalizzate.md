# US-3.3 — Creazione di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User)
**Necessità:** creazione di una cartella personalizzata, con possibilità di invitare altri utenti fin dalla creazione
**Obiettivo:** organizzazione dei documenti per commessa/comune, singolarmente o insieme ad altri utenti

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Collegata a [US-2.1](us-2.1-cartelle-personalizzabili.md) (cartelle personali) e [US-2.2](us-2.2-condivisione-fascicoli.md) (condivisione, inviti e regole di team).

## Criteri di accettazione

- Un utente autenticato può creare una cartella indicando un nome; il sistema crea la cartella, inizialmente con un solo membro (il creatore).
- Durante la creazione l'utente può invitare altri utenti per email con le modalità di [US-2.2](us-2.2-condivisione-fascicoli.md); la cartella diventa condivisa quando almeno un invito viene accettato.
- Se il nome è vuoto o già usato da un'altra cartella di cui l'utente è membro, il sistema mostra un messaggio di errore e non crea la cartella.

## Fuori scope

- Modifica ed eliminazione delle cartelle (vedi US-3.4 e US-3.5).
- Permessi differenziati tra i membri.

## Note

- Qualsiasi utente registrato può creare una cartella condivisa: non serve un amministratore né un'autorizzazione. Il creatore non ha poteri speciali, dopo la creazione è un membro come gli altri.
- Sovrapposizione residua con US-2.1 (creazione cartelle): da valutare se accorpare.
