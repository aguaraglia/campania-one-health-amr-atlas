# Geografia pubblica - edizione Campania

La cartografia pubblica dell'edizione Campania comprende:

- `atlas_region.geojson`: confine regionale ISTAT 2026 (codice 15);
- `atlas_provinces.geojson`: 5 unità sovracomunali ISTAT 2026: Caserta (061), Benevento (062), Città metropolitana di Napoli (263), Avellino (064), Salerno (065);
- `atlas_municipalities.geojson`: 550 comuni ISTAT al 1/1/2026.

Fonte: ISTAT, «Confini delle unità amministrative a fini statistici al 1° gennaio 2026», versione generalizzata (Limiti01012026_g.zip, SHA-256 in `metadata/SNAPSHOTS.tsv`), CC BY 4.0. Gli attributi dei DBF sono letti in UTF-8 e le coordinate sono convertite da EPSG:32632 a WGS84 da `scripts/build_istat_geography.py`.

Gli studi della letteratura curata stanno in layer distinti sotto `public/data/`. Le cinque strutture nominate (AOU Federico II, AOU Vanvitelli, Ospedale Monaldi a Napoli; AOU Ruggi d'Aragona a Salerno; AORN Sant'Anna e San Sebastiano a Caserta) sono geocodificate tramite OSM Nominatim (1 richiesta al secondo, 2026-11-20; risposte grezze in `raw/nominatim/`). Il punto Vanvitelli è l'indirizzo di Piazza Luigi Miraglia, non un edificio OSM. Gli ospedali non nominati negli studi restano su comune, provincia o regione.
