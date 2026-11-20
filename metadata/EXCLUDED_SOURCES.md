# Fonti escluse o non disponibili (edizione Campania, 2026-11-20)

Regola di riuso (decisione di Alex, 2026-11-20): sono accettabili le licenze aperte CC BY e CC0, e anche CC BY-NC e CC BY-NC-SA, perché CodexVitae ETS non ha scopi commerciali. Servono sempre l'attribuzione e, per NC-SA, la stessa licenza sui file derivati. Non usiamo fonti senza licenza dichiarata o con il riuso vietato. Le pagine che rispondono 403 o 500, o che mostrano una challenge anti-bot, non vengono aggirate. Il rapporto OsMed (con i rapporti regionali OsMed e il rapporto AIFA sugli antibiotici basato su OsMed) è escluso per decisione di progetto.

## Fonte regionale accettata
- **Si.Re.Ar. 2022, Regione Campania** (rapporto pubblicato nel 2024, ISBN 9788831204170). Il PDF non riporta una licenza propria; vale la clausola delle note legali del Portale Regione Campania (https://www.regione.campania.it/note-legali): «Ove non diversamente specificato, i materiali contenuti in questo Portale sono Copyfree [...] Tutto il materiale presente sul Portale può essere liberamente riprodotto, parzialmente o integralmente e modificato purché non a scopo di lucro e nel rispetto del Copyleft. La citazione della fonte è sempre obbligatoria». Equivale in pratica a CC BY-NC-SA: accettato, con attribuzione e stessa licenza sul file derivato `public/data/sirear_2022_campania.json`. Estratti solo valori regionali (sangue e liquor, consumo J01 convenzionata). Dati 2022, non confrontabili direttamente con AR-ISS 2024.

## Rapporti ISS/ISTISAN regionali
- NON TROVATO. La pagina EpiCentro «Documentazione Regioni» (https://www.epicentro.iss.it/farmaci/DocumentazioneRegioni) non cita la Campania. Il percorso https://www.epicentro.iss.it/farmaci/pdf/campania/ restituisce la pagina 404 di EpiCentro. La pagina EpiCentro «Resistenza agli antibiotici - Documentazione Regioni» rimanda solo ai rapporti regionali Si.Re.Ar. 2011 e 2013 (documenti della Regione, non ISS). Una ricerca web (2026-11-20) trova solo i rapporti Si.Re.Ar., il rapporto AIFA sugli antibiotici e il rapporto regionale OsMed «Campania 2024», escluso.

## Open data regionali
- https://dati.regione.campania.it/ chiude la connessione TLS (errore SSL); http://dati.regione.campania.it/ risponde HTTP 500. Non aggirato. NON DISPONIBILE.

## ICAAROweb (Regione Campania)
- https://icaaroweb.regione.campania.it/ riporta solo «© Regione Campania» nel piè di pagina, senza licenza propria; le infografiche interattive non sono state usate. I report annuali sono gli stessi del portale regionale: usato il PDF del portale, coperto dalle note legali regionali. ESCLUSO.

## ASL
- ASL Napoli 3 Sud: «© 2024 ASL Napoli 3 Sud - Tutti i diritti riservati»; la pagina sulla settimana degli antibiotici è una notizia, senza dati. ESCLUSO.
- ASL Avellino: le note legali non concedono riuso e rinviano ai «diritti d'uso e/o copia dei rispettivi proprietari». ESCLUSO.
- ASL Salerno: le note legali consentono la riproduzione con indicazione della fonte (licenza compatibile), ma sul sito non è stato trovato nessun dato AMR o di consumo. NON DISPONIBILE. Gli studi su ASL Salerno entrano come articoli del catalogo.
- ASL Napoli 1 Centro, ASL Napoli 2 Nord, ASL Caserta, ASL Benevento: connessione HTTPS non riuscita (catena di certificati incompleta; con curl nessuna risposta). Non aggirato (nessuna verifica TLS disattivata). NON VERIFICABILE.

## ARPA Campania (ARPAC)
- Licenza compatibile: note legali CC BY 3.0 IT e portale https://dati.arpacampania.it/ CC BY 4.0. Ma nessun dato AMR: la ricerca CKAN «antibiotic» dà 0 risultati e i dataset riguardano aria, acque, rifiuti, rumore e Legionella. NON DISPONIBILE.

## IZS del Mezzogiorno (IZSM, Portici)
- Licenza compatibile: note legali CC BY-NC 4.0 per testi e tabelle. Il catalogo open data (https://www.izsmportici.it/catalogo-open-data/) pubblica solo conteggi di esami per laboratorio e provincia di prelievo (anche «Antibiogramma da coltura batterica con M.I.C.», 2024-2026), senza esiti di resistenza: un conteggio di antibiogrammi non è un indicatore AMR. ESCLUSO per contenuto. Il CSV DIPSANITANIMALE (120 MB) è stato letto e non conservato; l'hash è in SNAPSHOTS.
- L'IZSM copre Campania e Calabria: gli articoli IZSM entrano solo se la quota campana è separata. Restano dubbi 20401533, 33801648 e 36982566 (Campania e Calabria insieme) e 38674761 (coste di quattro regioni).

## OsMed
- Escluso per decisione di progetto, insieme al rapporto regionale OsMed «Campania 2024» (AIFA) e al rapporto AIFA «L'uso degli antibiotici in Italia» (dati OsMed).

## Letteratura: testi integrali
- I testi integrali open access sono stati letti dall'archivio PMC tramite NCBI E-utilities (efetch db=pmc, API pubblica), 20 PMCID per richiesta: 32 richiesti, 32 scaricati, 30 con corpo del testo (32015041 e 34339281 senza body: decisi su titolo e abstract).
- Nessuna pagina 403 o challenge anti-bot è stata aggirata.
