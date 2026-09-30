# US-2.2 — Condivisione fascicoli tra colleghi

**Attore:** utente registrato (User) appartenente a uno studio (archetipo 4.2, Studio Rossi & Bianchi)
**Necessità:** condivisione di cartelle/fascicoli di documenti normativi con i colleghi dello studio
**Obiettivo:** accesso di tutto lo studio alla documentazione già raccolta, senza ripetere la ricerca da capo

---

## Contesto

Riferimento: [BuildEr.md](../BuildEr.md) — sezione 2.3 "Cosa è incluso" (gestione multi-utente/permessi per studio) e archetipo 4.2. Epic di riferimento: [epic-2-gestione-multi-utente.md](../epics/epic-2-gestione-multi-utente.md). Dipende da [US-2.1](us-2.1-cartelle-personalizzabili.md).

## Criteri di accettazione

- **Dato** una cartella personale con almeno un documento, **quando** l'utente sceglie di condividerla con uno o più colleghi dello studio, **allora** il sistema rende la cartella visibile ai colleghi selezionati.
- **Dato** una cartella condivisa, **quando** un collega vi accede, **allora** il sistema mostra l'elenco dei documenti contenuti, con data/versione di aggiornamento.
- **Dato** una cartella condivisa, **quando** il proprietario revoca la condivisione a un collega, **allora** il collega non ha più accesso alla cartella.
- **Dato** un documento nella cartella condivisa che viene aggiornato, **quando** un collega lo consulta, **allora** il sistema mostra la versione più recente a tutti i membri con accesso.

## Fuori scope

- Definizione della struttura "studio" e dell'invito dei membri (da chiarire, vedi note).
- Livelli di permesso granulari (sola lettura / modifica) oltre l'accesso in consultazione.

## Note

- Il PRD cita "ruoli e permessi per studio", ma i ruoli previsti sono solo Admin e User: da definire come si crea uno studio e come si aggiungono i membri.
- Da decidere se i colleghi con cui si condivide possano modificare il contenuto della cartella o solo consultarlo.
