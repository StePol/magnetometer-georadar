# Magnetometer + Georadar

Samostatný vývojový projekt nízkonákladového viacsenzorového magnetometra s možnosťou budúceho rozšírenia o georadar.

## Aktuálny stav

K dispozícii: K49E/AH49E Hall senzory a LSM303DLHC.
Zatiaľ nie sú zakúpené: ESP32-S3 a ADS1256.

Aktuálna fáza: laboratórne meranie, charakterizácia senzorov a návrh dátového modelu.

## Ciele

- viacsenzorové magnetické meranie,
- charakterizácia K49E,
- LSM303DLHC pre náklon, pohyb a pomocnú orientáciu,
- neskoršie overenie MMC5983MA ako referenčného senzora,
- GNSS georeferencovanie,
- lokálny záznam na SD,
- Wi-Fi/webové rozhranie pre telefón,
- Python + QGIS spracovanie,
- modulárna mechanika,
- budúce samostatné georadarové rozšírenie.

## Navrhovaná architektúra

```text
SMARTFÓN ──Wi-Fi──> ESP32-S3
                     ├── GNSS
                     ├── LSM303DLHC
                     ├── SD
                     ├── ADS1256 #1 ── K49E × 8
                     └── ADS1256 #2 ── K49E × 8

budúce REF-A / REF-B: MMC5983MA
```

## Dátové pravidlo

RAW dáta sú nemenný zdroj pravdy. Kalibrácia a spracovanie vytvárajú nové súbory.

Podrobný formát: `docs/measurements/data-format.md`
