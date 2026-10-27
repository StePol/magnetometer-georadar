# Pravidlá práce na projekte

Tieto pravidlá sú určené na vloženie do koreňa repozitára magnetometer-georadar.

- Komunikuj po slovensky. Pred zmenami čítaj existujúcu dokumentáciu a rešpektuj dátové formáty.
- Zachovaj pôvodné podklady; RAW dáta a záznamy uskutočnených meraní spätne neupravuj na nový experiment.
- Rozlišuj navrhnuté, vypočítané, simulované a namerané výsledky. Nevymýšľaj výsledky merania, absolvované kontroly ani hodnoty súčiastok.
- Každý návrh, meranie, kalibrácia a rozhodnutie má stabilné ID. Zmeny zapojenia majú revíziu.
- Udržuj väzbu na HW, FW, mechaniku, kalibráciu a konfiguráciu záznamu. Vydané konfigurácie označ Git tagom a manifestom.
- Firmvér musí mať reprodukovateľný postup zostavenia a nahratia. SDK a dosku nevyberaj potichu; zaznamenaj výber a dôvody.
- Overuj rozsahy napätí, pinout, referencie ADC, časovanie, chyby a chýbajúce dáta podľa konkrétnych komponentov.
- Knižnice KiCad a modely ulož prenositeľne v projekte. Zachovaj editovateľné originály a pridaj čitateľné exporty.
- Mechanické zmeny posudzuj spolu s polohou/osami senzorov, materiálmi, PCB a kabelážou.
- Vyhodnotenia musia uvádzať vstupy, verziu skriptu, parametre, jednotky a reprodukovateľný príkaz.
- Kontroly prispôsob zmene: zostavenie FW; testy parsera/kalibrácie; ERC/DRC pre dotknutý HW; kontrola zostavy a výkresov pre mechaniku. Ak nástroj nie je dostupný, označ kontrolu ako nevykonanú.
- Nepridávaj prihlasovacie údaje, lokálne virtuálne prostredia ani generované build adresáre do Gitu.
- Pred úpravou existujúcich nastavení ich porovnaj a zlúč; neprepisuj používateľské nastavenia plošne.
- Po práci stručne uveď zmenené súbory, vykonané kontroly, neistoty a ďalší krok.
