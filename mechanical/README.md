# Mechanická konštrukcia

## Pracovné prostredia
- Hlavný CAD: FreeCAD 1.1.4 na Linuxe, Flatpak.
- Jednotky: mm, sústava Standard.
- Hlavné editovateľné súbory: freecad/*.FCStd.
- SolidWorks: prípadná externá spolupráca.
- Výmena geometrie: STEP; výkresy: PDF.
- Verzia FreeCAD: FreeCAD 1.1.4 cez Flatpak

Externé úpravy evidovať ako samostatnú revíziu.
STEP export nenahrádza pôvodný parametrický model FreeCAD.

## Ukladanie
- solidworks/: pôvodné diely a zostavy SolidWorks.
- freecad/: pôvodné dokumenty FreeCAD.
- exports/step/: STEP exporty označené ID a revíziou.
- drawings/: výrobné výkresy v PDF.

Pre každý diel alebo zostavu urči jeden hlavný editovateľný
zdroj. STEP používaj na výmenu geometrie; nezachováva celú
históriu modelovania.

## Spoločné pravidlá
- Jednotky: mm.
- Počiatok a orientáciu osí dohodnúť pred návrhom.
- Evidovať materiál, revíziu a výrobný postup.
- Evidovať polohu a orientáciu senzorov.
- Zachovať všetky referencie zostavy.
- Pred úpravami na druhom počítači synchronizovať Git.
- Súbežne neupravovať rovnaký CAD súbor na dvoch počítačoch.

## Otvorené rozhodnutia
- Umiestnenie počiatku a smer osí.
- Výrobná technológia a materiály.
