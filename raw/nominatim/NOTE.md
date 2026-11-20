# Geocodifica Nominatim (edizione Campania, 2026-11-20)

Solo le strutture nominate negli studi inclusi. 23 richieste, user agent `CodexVitae-AMR-atlas/1.0 (info@codexvitae.it)`, `countrycodes=it`, `jsonv2`, pausa di 1,1 s (limite di 1 richiesta al secondo della policy OSMF). Dati © OpenStreetMap contributors, ODbL 1.0.

## Punti usati
- `federico2`: «Policlinico Federico II Napoli» → AOU Federico II, Via Gaetano Quagliarello, Napoli (40.8703321, 14.2191868), amenity=hospital. 5 studi.
- `vanvitelli`: nessun oggetto ospedaliero OSM per il Policlinico Vanvitelli. Usato «Piazza Luigi Miraglia, Napoli» (40.8497934, 14.2534302), indirizzo della sede citato nel testo integrale di PMID 33845049 («Piazza Luigi Miraglia 2»): **punto di indirizzo, non edificio**. 12 studi (incluso il Policlinico della Seconda Università di Napoli, stesso ente rinominato).
- `monaldi`: «Ospedale Monaldi, Napoli» → Ospedale Vincenzo Monaldi (40.8699666, 14.2100466), amenity=hospital. 3 studi.
- `ruggi`: «Ospedale Ruggi Salerno» → San Giovanni di Dio e Ruggi d'Aragona, Via San Leonardo, Salerno 84131 (40.6490286, 14.8289198), sede principale di Largo Città di Ippocrate. Non usato il secondo risultato (presidio di Via Vernieri, 40.6820019, 14.7661092). 15 studi («University Hospital of Salerno» = Ruggi, unica AOU della provincia).
- `caserta`: «Azienda Ospedaliera Caserta» → AO Sant'Anna e San Sebastiano, Via Ferdinando Palasciano 1, Caserta (41.0869813, 14.3336646). 1 studio.

## Richieste senza risultato (0 risposte)
- «Policlinico Federico II, Via Sergio Pansini, Napoli»
- «Azienda Ospedaliera Universitaria Luigi Vanvitelli, Piazza Luigi Miraglia, Napoli»
- «Ospedale San Giovanni di Dio e Ruggi d'Aragona, Salerno»
- «Azienda Ospedaliera Sant'Anna e San Sebastiano, Caserta»
- «Policlinico Vanvitelli Napoli»
- «Ospedale Sant'Anna e San Sebastiano Caserta»
- «Università della Campania Luigi Vanvitelli Piazza Miraglia Napoli»
- «ospedale San Giovanni di Dio e Ruggi d'Aragona»
- «ospedale Largo Città di Ippocrate Salerno»
- «Policlinico Luigi Vanvitelli»
- «Vanvitelli, Napoli, ospedale»
- «San Giovanni di Dio Salerno ospedale»
- «Policlinico Napoli centro storico»
- «Azienda Ospedaliera Universitaria Università della Campania»

Le altre richieste con risultato («Ospedale Monaldi, Napoli», «Azienda Ospedaliera Universitaria Federico II», «Ruggi d'Aragona Salerno», «ospedale civile Caserta Via Palasciano», «Sant'Anna e San Sebastiano», «Ospedale Ruggi Salerno», «Piazza Luigi Miraglia, Napoli») sono servite da conferma.

## Non geocodificati
Ospedali non nominati (restano su comune, provincia o regione); AORN dei Colli citata senza presidio (comune di Napoli); i quattro presidi ASL Caserta di Marcianise, Piedimonte Matese, Sessa Aurunca e Maddaloni (poligoni comunali ISTAT); allevamenti, canili, ospedali veterinari universitari, centri di recupero della fauna, depuratori non nominati. Il Cotugno compare solo in PMID 30061868 insieme a Monaldi e CTO (AORN dei Colli, dati aggregati sui tre presidi): comune di Napoli, nessun punto. Cardarelli, Pascale, Santobono, Moscati, Rummo e Ospedale del Mare non compaiono come struttura nominata in nessuno studio incluso: nessun punto.
