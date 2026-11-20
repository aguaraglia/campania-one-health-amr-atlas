# Campania One Health AMR Atlas

Edizione regionale `campania_amr_atlas`, pubblicata da Codex Vitae ETS sulla stessa
base delle edizioni Lazio e Molise.

## Stato

La letteratura pubblicata con collegamento territoriale esplicito alla Campania
è concentrata su Napoli e Salerno. Ne restano 91 inclusi (20 novembre 2026):
36 di struttura, 18 di comune, 11 di provincia e 26 a scala regionale.

Cinque strutture nominate, georiferite con Nominatim (© OpenStreetMap
contributors, ODbL):

- AOU Università della Campania Luigi Vanvitelli (Napoli, indirizzo di Piazza Luigi Miraglia): 12 studi;
- AOU Federico II (Napoli): 5 studi;
- Ospedale V. Monaldi (Napoli): 3 studi;
- AOU San Giovanni di Dio e Ruggi d'Aragona (Salerno): 15 studi;
- AORN Sant'Anna e San Sebastiano (Caserta): 1 studio.

A Napoli gli altri studi stanno sul comune o sulla provincia; Portici ha 1
studio. A Salerno, oltre al Ruggi, 4 studi stanno sulla provincia e 1 a
Castellabate. A Caserta i 2 studi sono l'AORN e i presidi ASL di Marcianise,
Piedimonte Matese, Sessa Aurunca e Maddaloni. Uno studio sugli allevamenti di
bufale copre Caserta e Salerno. Ad Avellino 1 studio sui cinghiali. Benevento
non ha studi con luogo provinciale esplicito. Ventisei studi a scala regionale
usano il contorno della regione: 13 umani sul layer di contorno e gli altri
sul layer del proprio settore.

I punti vicini a Napoli sono raggruppati con Leaflet.markercluster, la stessa
libreria cartografica dell'edizione Lazio, e si aprono con lo zoom.

L'IZS del Mezzogiorno copre Campania e Calabria: sono inclusi solo gli studi
che separano i dati campani.

L'edizione pubblica AR-ISS 2024 (copertura 52,4%, rete regionale con 24
presidi, CC BY 4.0; attribuzione Istituto Superiore di Sanità), AIFA Open Data
2024, antibatterici J01 (CC BY 4.0; attribuzione Agenzia Italiana del Farmaco)
e il rapporto Si.Re.Ar. 2022 della Regione Campania (riuso non commerciale con
attribuzione e copyleft, equivalente CC BY-NC-SA). I dati 2022 di Si.Re.Ar.
non sono direttamente confrontabili con AR-ISS 2024.

Sei layer (AMR umana, veterinaria, alimentare, ambientale, fauna selvatica,
contorno regionale):

- AMR umana: 9 elementi, 50 studi (5 punti; comune di Napoli; quattro comuni ASL Caserta; province di Napoli e Salerno);
- AMR veterinaria: 4 elementi, 16 studi;
- AMR alimentare: 2 elementi, 3 studi;
- AMR ambientale: 1 elemento (regione), 2 studi;
- AMR nella fauna selvatica: 4 elementi (Castellabate, Portici, provincia di Avellino, regione), 7 studi;
- studi a scala regionale: 1 elemento, 13 studi umani sul contorno.

I layer vuoti e le aree senza segnaposto sono nessuna evidenza pubblicata,
non resistenza zero. Ogni popup cita lo studio e il DOI (o il record PubMed
se il DOI non è assegnato) e ricorda che il segnaposto è il luogo dello
studio, non una prevalenza.

Confini ISTAT 2026 (550 comuni, 5 unità sovracomunali, regione 15), letti in
UTF-8. dati.regione.campania.it, ICAAROweb, le ASL, l'ARPAC, il catalogo open
data dell'IZSM e il PDF OsMed sono esclusi: vedi
`metadata/EXCLUDED_SOURCES.md`.

Il conteggio in homepage e in pubblicazioni legge
`public/data/literature-catalog.json` (91).

## Pagine

Sorgente su `main`. Il sito statico è pubblicato dal branch `gh-pages`
(GitHub Pages, cartella `/`). Nessun file `CNAME`. Analitica: GoatCounter
`https://atlanteamr.goatcounter.com/count`, come le edizioni Lazio e Molise.

## Build locale

```bash
python3 -m http.server 8000
```

Aprire `http://localhost:8000/`.

Per rigenerare i dati pubblici servono gli input in `raw/` e, per i confini,
l'archivio ISTAT indicato in `metadata/SNAPSHOTS.tsv`. I DBF ISTAT si leggono
in UTF-8:

```bash
pip install -r requirements-geodata.txt
python3 scripts/build_istat_geography.py --source-root <Limiti01012026_g> --output-root public/geography
python3 scripts/build_literature_catalog.py
python3 scripts/build_study_evidence_layers.py
```

## Directory

- `public/`: dati e asset approvati per il sito;
- `metadata/`: fonti, snapshot, ambito pubblico e fonti escluse;
- `raw/`: curatela, esummary e risposte Nominatim;
- `scripts/`: ricostruzione del catalogo e dei layer;
- `private/`: nessun dato riservato in questa edizione.
