# US-2.5 — Invito di membri nello studio

**Attore:** responsabile di uno studio (User)
**Necessità:** invio di inviti a colleghi per farli entrare nello studio
**Obiettivo:** team dello studio operativo sulla stessa documentazione

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.4](us-2.4-creazione-studio.md). Citata come fuori scope in [US-1.1](us-1.1-creazione-profilo.md).

## Criteri di accettazione

- Un responsabile di studio può inserire l'email di un collega e inviare l'invito; il sistema invia l'invito e lo mostra come "in attesa".
- Quando un utente registrato accetta un invito ricevuto, il sistema lo aggiunge all'elenco dei membri dello studio.
- Quando un utente non registrato completa la registrazione e accetta l'invito ricevuto, il sistema lo associa allo studio.
- Se il responsabile annulla un invito in attesa o l'invito scade, il sistema lo invalida e il link non è più utilizzabile.
- Se il responsabile tenta di invitare un'email già membro dello studio, il sistema mostra un messaggio di errore.

## Fuori scope

- Aggiunta di membri senza consenso.
- Inviti in blocco (import da file).

## Note

- Da definire la durata di validità dell'invito.
