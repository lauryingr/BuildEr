# BuildEr – Flusso di ricerca delle fonti

> Stato: **bozza, DA VALIDARE con Elia (architetto / committente)**
> Ultimo aggiornamento: 30/09/2026

## 1. Flusso di ricerca

| #   | Fase                                                                                                                                       | Output                                 | Stato        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------- | ------------ |
| 1   | Elia mi ha fornito un elaborato sul quadro normativo (Stato → Regione → Provincia → Comune, esempio: Oderzo)                               | PDF sorgente                           | ✅ fatto     |
| 2   | Studio dell'elaborato e scrematura: **tolgo le pratiche** dell'architetto (CILA, SCIA, PdC, depositi, istanze…) e tengo solo le **regole** | Lista "Da salvare"                     | ✅ fatto     |
| 3   | **Validazione con Elia**: conferma cosa è utile, cosa manca, cosa è superfluo                                                              | Lista                                  | ⏳ da fare   |
| 4   | Per ogni voce validata: trovo il **link alla fonte primaria**                                                                              | Lista documento + URL                  | ⏳ dopo l'ok |
| 5   | **Controllo manuale** dei portali e flag di accessibilità (libero / captcha / login / SPID)                                                | Lista con flag                         | ⏳           |
| 6   | Progettazione dell'app sulla base di cosa è davvero raggiungibile                                                                          | Tassonomia dati + architettura scraper | ⏳           |

### Criterio di scrematura (fase 2)

- **Si salva:** regole valide per un territorio (norme, piani, regolamenti, moduli vuoti, tariffe, tempi normati).
- **Non si tratta:** pratiche individuali dell'architetto (atti su un singolo immobile, con SPID / firma digitale / PEC / responsabilità professionale).
- **Esclusi anche:** giurisprudenza, statistiche, interpretazioni e ragionamenti sui ruoli professionali (non sono normativa).
- **Requisito trasversale:** solo fonti primarie (sito dell'ente, BUR, Normattiva), mai aggregatori.

## 2. Lista – DA SALVARE in BuildEr

Legenda flag: 🟡 **DA VALIDARE** (Elia) · link e accessibilità ancora da verificare.

### Stato

| Documento | Flag |
| --------- | ---- |
| DPR 380/2001 – Testo Unico Edilizia | 🟡 |
| DL 69/2024 e L. 105/2024 – Salva Casa | 🟡 |
| D.Lgs. 42/2004 – Codice Beni Culturali e Paesaggio | 🟡 |
| DPR 31/2017 – Autorizzazione paesaggistica semplificata (Allegati A e B) | 🟡 |
| L. 241/1990 – Procedimento amministrativo e accesso agli atti | 🟡 |
| L. 447/1995 e DPCM 5/12/1997 – Acustica | 🟡 |
| DM 26/06/2015 e L. 10/1991 – APE / efficienza energetica | 🟡 |
| D.Lgs. 152/2006 e DPR 357/1997 – Ambiente e VIncA | 🟡 |
| RD 2537/1925 e RD 274/1929 – Competenze professionali | 🟡 |
| RD 368/1904 – Bonifiche (fasce di rispetto) | 🟡 |
| NTC 2018 – Norme Tecniche per le Costruzioni | 🟡 |
| L. 13/1989 – Superamento barriere architettoniche negli edifici privati | 🟡 |
| L. 164/2014 (11 novembre 2014) – Conversione DL 133/2014 "Sblocca Italia" | 🟡 |
| D.Lgs. 207/2021 – Codice europeo delle comunicazioni elettroniche | 🟡 |
| Decreto ministeriale 130/2025 – aggiornamenti infrastrutturazione digitale (estremi da verificare) | 🟡 |

### Regione Veneto

| Documento                                                               | Flag |
| ----------------------------------------------------------------------- | ---- |
| LR 11/2004 – Governo del territorio (PAT / PI)                          | 🟡   |
| LR 14/2017 – Contenimento consumo di suolo                              | 🟡   |
| LR 14/2019 – Veneto 2050 (riqualificazione urbana e rinaturalizzazione) | 🟡   |
| LR 55/2012 – SUAP                                                       | 🟡   |
| LR 12/2024 (Capo IV) e Reg. Reg. 4/2025 – VIncA                         | 🟡   |
| DGR 2948/2009 – Valutazione compatibilità idraulica                     | 🟡   |
| DGR 244/2021 – Classificazione sismica                                  | 🟡   |
| DGR 121/2011, 659/2012, 1090/2019 – APE                                 | 🟡   |
| DGR 438/2025 e DGR 28/2025 – VIncA                                      | 🟡   |
| PTRC – Piano Territoriale Regionale di Coordinamento                    | 🟡   |
| Dati cartografici IDT-RV 2.0 (CTRN, DTM, uso suolo)                     | 🟡   |

### Provincia (Treviso)

| Documento                                                | Flag |
| -------------------------------------------------------- | ---- |
| PTCP di Treviso                                          | 🟡   |
| Zone di interesse archeologico (art. 142 D.Lgs. 42/2004) | 🟡   |

> Il livello provinciale è quasi assente nell'elaborato: da approfondire con Elia.

### Comune (esempio: Oderzo)

| Documento                                                 | Flag |
| --------------------------------------------------------- | ---- |
| PAT + Variante n.1 (consumo di suolo, L.R. 14/2017)       | 🟡   |
| PI n.3 con NTO, Varianti 9 e 10                           | 🟡   |
| Registro Crediti Edilizi e Accordi Pubblico-Privati (APP) | 🟡   |
| Piano Comunale delle Acque (TAV 2, 3, 7)                  | 🟡   |
| Piano di Classificazione Acustica                         | 🟡   |
| Regolamento del verde                                     | 🟡   |
| Regolamento di accesso documentale                        | 🟡   |
| Tariffe: diritti di segreteria e oneri istruttori         | 🟡   |
| Regolamento Edilizio Comunale                             | 🟡   |
| Regolamento di Polizia Urbana                             | 🟡   |
| Regolamento di Igiene                                     | 🟡   |

### Enti terzi

| Documento                                                                           | Flag |
| ----------------------------------------------------------------------------------- | ---- |
| Regolamenti e fasce di rispetto del Consorzio di Bonifica Piave                     | 🟡   |
| ATS (Alto Trevigiano Servizi) – Regolamento e modulo (es. allacciamenti / scarichi) | 🟡   |

### Metadati normativi da conservare (non sono pratiche)

Tempi e costi derivati da norma, sempre collegati alla norma di origine: 30 gg accesso agli atti · 60 gg paesaggistica semplificata · 500 m³/ha invaso idraulico · 4 m fascia di rispetto Consorzio · 15 € deposito APE.

## 3. Prossimi passi

1. **Mostrare questo documento a Elia** e raccogliere: cosa confermare, cosa togliere, cosa aggiungere.
2. Dopo l'ok: per ogni voce validata, cercare il **link alla fonte primaria** e **accessibilità alla fonte e download del documento**
3. **Controllare a mano ogni portale** e assegnare un flag di accessibilità:
   - 🟢 libero
   - 🟠 captcha / parametri fragili
   - 🔴 login / SPID (fuori scopo)
4. Da lì definire la tassonomia dati per ogni documento: `livello`, `tipo`, `ente emittente`, `vigenza (da/a)`, `URL primario`, `hash file`.

## 4. Avvertenza

L'elaborato di Elia cita anche fonti secondarie (blog, aggregatori). Alcuni dati specifici (es. sentenze, date di efficacia delle varianti) **non vanno copiati**: l'elaborato serve come mappa di _dove cercare_, e ogni dato va preso dalla fonte primaria.
