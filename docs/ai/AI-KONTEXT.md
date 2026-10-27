# Vstupný kontext pre AI — Magnetometer + Georadar

Tento dokument vlož do novej konverzácie alebo daj AI prečítať pri začatí práce.

## Zadanie a účel
Pomáhaj mi vyvíjať nízkonákladový viacsenzorový magnetometer od laboratórnych experimentov cez firmvér, PCB a mechaniku po overené integrované riešenie. Georadar je budúce samostatné rozšírenie. Súčasťou práce sú čiastkové návrhy zapojení na zistenie parametrov, simulácie, merania, programovanie a vyhodnotenie výsledkov.

Repozitár: https://github.com/StePol/magnetometer-georadar
Jazyk komunikácie a dokumentácie: slovenčina. Identifikátory kódu, názvy dátových polí a technické názvy súborov môžu byť anglické.

## Stav známy z chatu a README overeného 2026-10-27
- K dispozícii sú K49E/AH49E Hall senzory a LSM303DLHC.
- Podľa README ešte neboli zakúpené ESP32-S3 a ADS1256; pred objednaním alebo návrhom over aktuálny stav.
- Prebieha laboratórna charakterizácia senzorov a návrh dátového modelu.
- Uvažovaná architektúra: smartfón cez Wi-Fi, ESP32-S3, GNSS, LSM303DLHC, SD a dva ADS1256 pre spolu 16 K49E. Ide o návrh na overenie, nie potvrdenú realizáciu.
- MMC5983MA sa zvažuje ako budúci referenčný senzor.
- Spracovanie má využívať Python a QGIS.

## Zvolené a predbežné nástroje
- Obsidian: znalostná báza a technický denník.
- Zed: editor na programovanie, pravdepodobne ESP32.
- KiCad: schémy a PCB.
- FreeCAD 1.1.4 na Linuxe: hlavný nástroj pre mechanický návrh.
- SolidWorks: iba prípadná externá spolupráca cez STEP a PDF.
- Git/GitHub: verzovanie a spoločné úložisko projektu.
- Presná doska, SDK/framework, OS pre jednotlivé nástroje a verzie programov ešte nie sú určené.

## Navrhovaný spôsob práce
Lokálny koreň repozitára otvoriť ako Obsidian vault. Zachovať existujúce docs/, hardware/, firmware/, software/, tests/ a data/. Doplniť mechanical/. Dokumentácia má odkazovať na originálne súbory, bez vytvárania nezávislých kópií.

Sledovať reťazec: požiadavka → návrh → experiment/meranie → analýza → rozhodnutie → verzia systému.
Každý čiastkový návrh má cieľ, revíziu, schému, súčiastky, výpočty, plán overenia a výsledok. Každé vykonanie merania má vlastné ID a odkaz na konkrétnu revíziu návrhu.

## Pravidlá pre technické závery
- Odlišuj požiadavku, predpoklad, údaj výrobcu, výpočet, simuláciu a meranie.
- Nenavrhuj finálne hodnoty bez vstupných údajov; neisté hodnoty označ.
- Parametre komponentov overuj v datasheete presného výrobcu a variantu. Zaznamenaj revíziu, stranu a podmienky platnosti.
- RAW dáta nikdy neprepisuj. Kalibrácia, filtrovanie a prevody jednotiek vytvárajú nové súbory.
- Pri šume uvádzaj jednotky, šírku pásma, vzorkovanie a spôsob výpočtu. Pri presnosti uvádzaj podmienky a neistotu.
- Nenazývaj ADC rozlíšenie meracou presnosťou ani návrh overeným riešením.
- Návrh AI bez dôkazu zostáva návrhom.
- Zohľadni vplyv napájania, kabeláže, magnetických materiálov, teploty, orientácie a mechaniky na meranie.

## Formát podkladov
Poznámky Markdown UTF-8; metadáta JSON/YAML; malé a stredné merania CSV s dátovým slovníkom. Schémy: editovateľný KiCad projekt a PDF/SVG. Mechanika: pôvodné diely a zostavy plus STEP a PDF výkresy. Analýzy: skript/notebook, verzie závislostí, vstupy a nastavenia. Obrázky sú doplnkom, nie jediným zdrojom čísel a spojení.

## Čo urobiť pri prevzatí projektu
1. Prečítaj README, AGENTS.md, docs/index.md, existujúci dátový formát a relevantné protokoly.
2. Zisti skutočný stav súborov, hardvéru a otvorených rozhodnutí. Tento dokument je historický vstup, nie náhrada aktuálneho repozitára.
3. Pomenuj najbližší overiteľný cieľ a vykonaj prácu v jeho rozsahu.
4. Výsledok zaznamenaj s použitými vstupmi, kontrolami, obmedzeniami a ďalším krokom.

Aktuálna úloha pre AI: [DOPLNIŤ konkrétny problém, vstupné súbory a požadovaný výsledok].
