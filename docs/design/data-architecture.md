# Dátová architektúra

Tri vrstvy:
1. RAW acquisition
2. Calibration/processing
3. GIS visualization

RAW vrstva je nemenná.

Každé meranie má mať timestamp, sequence number, konfiguráciu zariadenia, verziu dátového formátu a verziu kalibrácie.

Kalibrácie sú oddelené od RAW CSV a obsahujú minimálne sensor_id, dátum, metódu, offset, gain, teplotný koeficient a poznámky.

Pri georeferencovaní sa uchováva poloha, smer, náklon a rýchlosť, aby bolo možné neskôr vypočítať polohu jednotlivých senzorov vzhľadom na referenčný bod zostavy.
