# Shrnutí pro poznámky

## Lekce 1: Přehled technik testování

### Kategorie technik

- **Černá skříňka (Black-Box):**
  - Testuje funkčnost **bez znalosti vnitřní struktury**, na základě specifikací (co má systém dělat).
  - _Analogie: Testování kávovaru – vstup/výstup._
- **Bílá skříňka (White-Box):**
  - Testuje na základě **znalosti vnitřní struktury** (kódu, architektury).
  - Cílem je ověřit vnitřní fungování a měřit pokrytí struktury.
  - _Analogie: Kontrola elektroinstalace elektrikářem._
- **Založené na zkušenostech (Experience-Based):**
  - Využívá **znalosti a intuici** testerů k nalezení chyb, které jiné techniky nemusí odhalit.
  - _Analogie: Zkušený automechanik diagnostikuje podle zvuku._

### Kombinace

- V praxi se techniky často **kombinují** pro dosažení nejlepšího pokrytí.

---

## Lekce 2: Rozdělení tříd ekvivalence (EP)

### Co to je

- Technika černé skříňky, která rozděluje možné vstupy/výstupy do **skupin (tříd)**, kde se předpokládá **stejné chování** systému.

### Cíl

- **Snížit počet testů** výběrem **jednoho reprezentanta** z každé třídy.

### Typy tříd

- **Platné (Valid):** Hodnoty, které má systém akceptovat.
- **Neplatné (Invalid):** Hodnoty, které má systém odmítnout/zpracovat jako chybu.

### Proces

1. Identifikuj vstup.
2. Identifikuj platné/neplatné třídy.
3. Navrhni testy (1 hodnota/třída).

### Testování neplatných tříd

- Každou neplatnou třídu testuj **samostatně**, aby se zabránilo maskování chyb.

### Pokrytí

- **100% EP:** Testována alespoň 1 hodnota z každé třídy.

### Omezení

- Nepokrývá specificky **hranice** tříd.

---

## Lekce 3: Analýza hraničních hodnot (BVA)

### Co to je

- Technika černé skříňky zaměřená na testování **hranic** mezi třídami ekvivalence a hodnot těsně kolem nich.

### Předpoklad

- Chyby se často vyskytují **na hranicích**.

### Předpoklad pro použití

- Musí být nejprve provedeno **Rozdělení tříd ekvivalence (EP)**.

### Varianty

- **2-hodnotová:** Testuje **hranici** a hodnotu **těsně vedle** (v sousední třídě).
- **3-hodnotová:** Testuje hodnotu **těsně před**, **na hranici** a **těsně vedle**.

### Proces

1. Identifikuj třídy (EP).
2. Identifikuj hranice.
3. Aplikuj 2/3-hodnotovou BVA.
4. Navrhni testy.

### Pokrytí

- **100% BVA:** Otestovány všechny hranice dle zvolené varianty.

### Kombinace

- Často se kombinuje s EP pro komplexní pokrytí.

### Omezení

- Primárně pro **uspořádané** třídy (čísla, rozsahy, počty).

---

## Lekce 4: Testování pomocí rozhodovací tabulky

### Co to je

- Technika černé skříňky pro testování **složité logiky** závislé na **kombinaci více podmínek**.

### Struktura

- Tabulka se 4 kvadranty:
  - **Podmínky**
  - **Akce**
  - **Pravidla** (sloupce - kombinace podmínek)
  - **Výsledky akcí** (X/ ).

### Proces

1. Identifikuj podmínky a akce.
2. Vytvoř kombinace podmínek (pravidla, 2^N pro N binárních podmínek).
3. Urči akce pro každé pravidlo.
4. (Minimalizuj tabulku).
5. Navrhni 1 test/pravidlo.

### Pokrytí

- **100%:** Otestováno každé **pravidlo (sloupec)**.

### Výhody

- Systematické, odhaluje chybějící/nekonzistentní pravidla.

### Nevýhody

- Počet pravidel může být velký (exponenciální růst).

---

## Lekce 5: Testování přechodů stavů

### Co to je

- Technika pro modelování a testování systémů, které mají konečný počet stavů a jejichž chování závisí na aktuálním stavu a vstupních událostech.

### Modely

- **Diagram přechodů stavů:** Graficky zobrazuje stavy, přechody (šipky), události/akce/podmínky.
- **Stavová tabulka:** Tabulka, kde řádky = stavy, sloupce = události, buňky = cílový stav/akce.

### Cíl

- Ověřit správnost přechodů mezi stavy, provedené akce a reakce na platné i neplatné události.

### Kritéria pokrytí

- **Pokrytí všech stavů:** Navštívit každý stav.
- **Pokrytí všech platných přechodů:** Projít každou šipku/definovaný přechod.
- Testovat i **neplatné přechody**.

### Testovací případ

- Typicky pokrývá sekvenci několika přechodů.

---

Tento přehled shrnuje klíčové body pro dosud probrané techniky černé skříňky. Doufám, že ti to pomůže s poznámkami!

Můžeme teď přejít k technikám bílé skříňky a začít **Testováním a pokrytím příkazů**?
