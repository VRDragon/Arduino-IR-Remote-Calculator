# 🔢 IR Remote Calculator

**Kalkulačka ovládaná televíznym diaľkovým ovládačom, výsledok svieti na štvormiestnom sedemsegmentovom displeji.**

![Rok](https://img.shields.io/badge/rok-2017-blue) ![Arduino](https://img.shields.io/badge/Arduino-C%2FC%2B%2B-00979d) ![Displej](https://img.shields.io/badge/TM1650-7--segment-red) ![Stav](https://img.shields.io/badge/stav-experimentálny-lightgrey)

> **Rok realizácie:** 2017 · **Tagy:** `arduino` `infrared` `ir-remote` `calculator` `tm1650` `seven-segment` `embedded` `electronics`

## O projekte

Experiment z roku 2017, ktorý spája tri veci: príjem infračerveného signálu, dekódovanie tlačidiel diaľkového ovládača a ovládanie displeja s čipom **TM1650**. Číslice zadávate na ovládači, Arduino ich spracuje a vypíše na displeji.

## Funkcie

- Zadávanie čísel 0–9 diaľkovým ovládačom.
- Sčítanie a odčítanie, tlačidlá `+`, `−`, `100+` a `200+`.
- Zobrazenie na 4 miestach, pri preplnení (> 9999) displej ukáže `Err`.
- Vlastná tabuľka znakov pre sedemsegmentovku (číslice, `E`, `r`).
- Dekódované kódy tlačidiel sú v komentároch v zdrojáku, takže ich ľahko prispôsobíte inému ovládaču.

## Zapojenie

| Pin Arduina | Pripojené na |
|---|---|
| D2, D3 | TM1650 (displej) |
| D4 | výstup IR prijímača |

## Knižnice

`TM1650.h` a `IRSendRev.h` (príjem a dekódovanie IR).

## Nahratie

1. Nainštalujte obe knižnice do Arduino IDE.
2. Otvorte `arduino_ir_calc.ino`, zapojte hardvér podľa tabuľky.
3. Nahrajte skicu a namierte ovládač na prijímač.

## Stav

Archívny experiment, logika kalkulačky nie je dokončená a bez úprav sa nemusí skompilovať. Staršie anglické README je v [docs/README.en.md](docs/README.en.md).

## Autor

**Vratislav Režo** ([@VRDragon](https://github.com/VRDragon))
