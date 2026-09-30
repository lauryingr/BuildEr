# US-2.5 — Invito di membri nello studio

**Attore:** responsabile di uno studio (User)
**Necessità:** invio di inviti a colleghi per farli entrare nello studio
**Obiettivo:** team dello studio operativo sulla stessa documentazione

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.4](us-2.4-creazione-studio.md). Citata come fuori scope in [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- **Dato** un responsabile di studio, **quando** inserisce l'email di un collega e invia l'invito, **allora** il sistema invia l'invito e lo mostra come "in attesa".
- **Dato** un invito ricevuto da un utente registrato, **quando** l'utente lo accetta, **allora** il sistema lo aggiunge all'elenco dei membri dello studio.
- **Dato** un invito ricevuto da un utente non registrato, **quando** l'utente completa la registrazione, **allora** il sistema lo associa allo studio dopo l'accettazione.
- **Dato** un invito in attesa, **quando** il responsabile lo annulla o l'invito scade, **allora** il sistema lo invalida e il link non è più utilizzabile.
- **Dato** un'email già membro dello studio, **quando** il responsabile tenta di invitarla di nuovo, **allora** il sistema mostra un messaggio di errore.

## Fuori scope

- Aggiunta di membri senza consenso.
- Inviti in blocco (import da file).

## Note

- Da definire la durata di validità dell'invito.
