# CSV dátový formát

Verzia: `magnetometer-csv-v1`

Pravidlá:
- oddeľovač: `,`
- desatinný oddeľovač: `.`
- čas: ISO 8601, ideálne UTC
- jeden riadok = jeden synchronizovaný vzorkovací okamih
- chýbajúca hodnota = prázdne pole
- RAW hodnoty sa neprepisujú

## Hlavička V1

```csv
timestamp_utc,sequence,latitude_deg,longitude_deg,altitude_m,gps_speed_mps,gps_fix,heading_deg,roll_deg,pitch_deg,ref_a_x_uT,ref_a_y_uT,ref_a_z_uT,mag_01_raw,mag_02_raw,mag_03_raw,mag_04_raw,mag_05_raw,mag_06_raw,mag_07_raw,mag_08_raw,mag_09_raw,mag_10_raw,mag_11_raw,mag_12_raw,mag_13_raw,mag_14_raw,mag_15_raw,mag_16_raw,ref_b_x_uT,ref_b_y_uT,ref_b_z_uT,temperature_C,battery_V,quality_flags
```

Jednotky:
- poloha: stupne
- výška: m
- rýchlosť: m/s
- heading/roll/pitch: stupne
- `*_uT`: mikrotesla
- `*_raw`: priamy výstup ADC/senzora bez predpokladu jednotky
- teplota: °C
- batéria: V

Kým K49E nebude kalibrovaný, používať `mag_NN_raw`, nie `mag_NN_uT`.

## Quality flags

bit 0 GPS fix neplatný
bit 1 nízka GPS kvalita
bit 2 veľký náklon
bit 3 vysoké vibrácie
bit 4 senzor mimo rozsahu
bit 5 ADC overflow
bit 6 výpadok senzora
bit 7 manuálne označený problém
