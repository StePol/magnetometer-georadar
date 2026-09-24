# Laboratórny test LSM303DLHC

## Úloha
LSM303DLHC používame hlavne ako akcelerometer pre náklon/pohyb a ako pomocný magnetometer pre orientáciu a diagnostiku.

## Akcelerometer
Zmerať pokojný modul v troch polohách (+X, +Y, +Z hore), každú 30–60 s.
Vyhodnotiť offset, priemer, šum a opakovateľnosť.

## Magnetometer
Pred kalibráciou vykonať pomalé 3D otáčanie modulu a zaznamenať X/Y/Z.
Vytvoriť scatter/3D graf a vyhodnotiť hard-iron offset a soft-iron deformáciu.

## Kalibrácia po montáži
Kalibráciu zopakovať na hotovej zostave, pretože ESP32, SD, DC/DC meniče, káble a kovové časti môžu meniť lokálne magnetické pole.

## GPS porovnanie
Pri dostatočnej rýchlosti možno porovnať magnetický heading s headingom odvodeným z GPS trajektórie.
