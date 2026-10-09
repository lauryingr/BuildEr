# US-3.4 — Modifica di cartelle personalizzate e condivisibili

**Attore:** utente registrato (User) membro di una cartella
**Necessità:** modifica di una cartella esistente (nome, documenti contenuti)
**Obiettivo:** cartelle sempre coerenti con le commesse in corso, aggiornabili da tutti i membri

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3. Epic di riferimento: [epic-3-azioni-documenti.md](../epics/epic-3-azioni-documenti.md). Dipende da [US-3.3](us-3.3-creazione-cartelle-personalizzate.md). Per membri e inviti vedi [US-2.2](us-2.2-condivisione-fascicoli.md).

## Criteri di accettazione

- Qualsiasi membro può modificare il nome della cartella; quando salva, il sistema aggiorna il nome per tutti i membri.
- Qualsiasi membro può aggiungere o rimuovere un documento dalla cartella; il sistema aggiorna il contenuto per tutti i membri senza cancellare il documento dalla piattaforma.
- Se il nuovo nome è vuoto o già usato da un'altra cartella dello stesso utente, il sistema mostra un errore e non applica la modifica.
- Se un utente che non è membro tenta di modificare la cartella, il sistema nega l'operazione.

## Fuori scope

- Creazione ed eliminazione delle cartelle.
- Cronologia delle modifiche o indicazione di chi ha aggiunto/rimosso un documento.

## Note

- Tutti i membri hanno gli stessi poteri: non c'è un proprietario. Poiché chiunque può rimuovere i documenti inseriti da altri, valutare in futuro una cronologia delle modifiche.
