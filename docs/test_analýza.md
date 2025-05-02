Rozhodně! Tady je ucelený souhrn všeho, co jsme dosud probrali z Kapitoly 4 a začátku Kapitoly 5, připravený pro zkopírování do tvého Markdown souboru (`.md`). Použil jsem Markdown formátování pro přehlednost.

```markdown
# Poznámky ISTQB CTFL 4.0 – Kapitola 4 & 5 (Část 1)

---

## Kapitola 4: Testovací analýza a návrh testů

### 4.1 Přehled technik testování

**Shrnutí pro poznámky:**

- **Kategorie technik:**
  - **Černá skříňka (Black-Box):** Testuje funkčnost **bez znalosti vnitřní struktury**, na základě specifikací (co má systém dělat). _Analogie: Testování kávovaru – vstup/výstup._
  - **Bílá skříňka (White-Box):** Testuje na základě **znalosti vnitřní struktury** (kódu, architektury). Cílem je ověřit vnitřní fungování a měřit pokrytí struktury. _Analogie: Kontrola elektroinstalace elektrikářem._
  - **Založené na zkušenostech (Experience-Based):** Využívá **znalosti a intuici** testerů k nalezení chyb, které jiné techniky nemusí odhalit. _Analogie: Zkušený automechanik diagnostikuje podle zvuku._
- **Kombinace:** V praxi se techniky často **kombinují** pro dosažení nejlepšího pokrytí.

---

### 4.2 Techniky testování černé skříňky

#### 4.2.1 Rozdělení tříd ekvivalence (Equivalence Partitioning - EP)

- **Princip:** Rozdělit možné vstupy/výstupy do **skupin (tříd)**, kde se předpokládá **stejné chování** systému. Cílem je **snížit počet testů** výběrem **jednoho reprezentanta** z každé třídy.
- **Typy tříd:**
  - **Platné (Valid):** Hodnoty, které má systém akceptovat.
  - **Neplatné (Invalid):** Hodnoty, které má systém odmítnout/zpracovat jako chybu.
- **Proces:** Identifikuj vstup -> Identifikuj platné/neplatné třídy -> Navrhni testy (1 hodnota/třída).
- **Testování neplatných tříd:** Každou neplatnou třídu testuj **samostatně** (v jednom testu jen jedna neplatná podmínka), aby se zabránilo maskování chyb.
- **Pokrytí:** 100% EP = testována alespoň 1 hodnota z každé třídy.
- **Příklad (Počet kusů 1-100):**
  - VP1: 1-100 (vyber např. 50)
  - IP1: < 1 (vyber např. 0)
  - IP2: > 100 (vyber např. 101)
  - IP3: Ne-celá čísla (vyber např. 10.5)
  - IP4: Nečíselné (vyber např. "abc")
  - Celkem 5 testů pro 100% EP.

**Shrnutí pro poznámky:**

- **Co to je:** Technika černé skříňky, rozděluje vstupy/výstupy do **skupin (tříd)** se **stejným očekávaným chováním**.
- **Cíl:** **Snížit počet testů** výběrem **jednoho reprezentanta** z každé třídy.
- **Typy:** **Platné** (akceptovat) a **Neplatné** (odmítnout/chyba).
- **Neplatné třídy:** Testuj **samostatně**, aby se nemaskovaly chyby.
- **Omezení:** Nepokrývá specificky **hranice** tříd.

#### 4.2.2 Analýza hraničních hodnot (Boundary Value Analysis - BVA)

- **Princip:** Zaměřuje se na testování **hranic** mezi třídami ekvivalence a hodnot těsně kolem nich, protože zde se často vyskytují chyby. Vyžaduje nejprve EP.
- **Varianty:**
  - **2-hodnotová:** Testuje **hranici** a hodnotu **těsně vedle** (v sousední třídě).
  - **3-hodnotová:** Testuje hodnotu **těsně před**, **na hranici** a **těsně vedle**.
- **Proces:** Identifikuj třídy (EP) -> Identifikuj hranice -> Aplikuj 2/3-hodnotovou BVA -> Navrhni testy.
- **Pokrytí:** 100% BVA = otestovány všechny hranice dle zvolené varianty.
- **Příklad (Počet kusů 1-100):**
  - Hranice: 1, 100.
  - 2-hodnotová BVA: Testuj 0, 1, 100, 101.
  - 3-hodnotová BVA: Testuj 0, 1, 2, 99, 100, 101.
- **Kombinace:** Často se kombinuje s EP.

**Shrnutí pro poznámky:**

- **Co to je:** Technika černé skříňky, testuje **hranice** tříd ekvivalence a hodnoty **těsně kolem** nich.
- **Předpoklad:** Chyby se často vyskytují **na hranicích**. Vyžaduje **EP**.
- **Varianty:** **2-hodnotová** (hranice + vedle) a **3-hodnotová** (před + hranice + vedle).
- **Omezení:** Primárně pro **uspořádané** třídy.

#### 4.2.3 Testování pomocí rozhodovací tabulky

- **Princip:** Systematická technika pro testování **složité logiky** závislé na **kombinaci více podmínek**. Mapuje kombinace podmínek na výsledné akce.
- **Struktura:** Tabulka: Podmínky, Akce, Pravidla (sloupce - kombinace T/F/-), Výsledky akcí (X/ ).
- **Proces:** Identifikuj podmínky a akce -> Vytvoř kombinace podmínek (pravidla, 2^N) -> Urči akce pro každé pravidlo -> (Minimalizuj tabulku pomocí "-") -> Navrhni 1 test/pravidlo.
- **Pokrytí:** 100% = otestováno každé **pravidlo (sloupec)**.
- **Příklad (Sleva v e-shopu):**
  - Podmínky: Nový zákazník? (T/F), Objednávka > 1000? (T/F)
  - Akce: Sleva 10%, Sleva 15%, Žádná sleva.
  - Minimalizovaná tabulka měla 3 pravidla (sloupce), vyžaduje 3 testy.
- **Výhody:** Systematické, odhaluje chybějící/nekonzistentní pravidla.
- **Nevýhody:** Počet pravidel může být velký.

**Shrnutí pro poznámky:**

- **Co to je:** Technika černé skříňky pro testování **složité logiky** závislé na **kombinaci podmínek**.
- **Struktura:** Tabulka: **Podmínky, Akce, Pravidla (sloupce), Výsledky (X/** )\*\*.
- **Proces:** Identifikuj P+A -> Vytvoř pravidla (kombinace) -> Urči Akce -> (Minimalizuj) -> 1 Test/Pravidlo.
- **Pokrytí:** 100% = otestován každý **sloupec (pravidlo)**.

#### 4.2.4 Testování přechodů stavů (State Transition Testing)

- **Princip:** Technika pro modelování a testování systémů s **konečným počtem stavů**, kde chování závisí na **aktuálním stavu** a vstupních **událostech**.
- **Modely:**
  - **Diagram přechodů stavů:** Graficky (stavy, šipky=přechody, popisky=události/akce/[podmínky]).
  - **Stavová tabulka:** Tabulka (řádky=stavy, sloupce=události, buňky=cílový stav/akce). Prázdná buňka = neplatný přechod.
- **Cíl:** Ověřit správnost přechodů mezi stavy, provedené akce, reakce na události.
- **Kritéria pokrytí:** **Pokrytí všech stavů** (slabé), **Pokrytí všech platných přechodů** (běžné), testování **neplatných přechodů**.
- **Testovací případ:** Typicky pokrývá sekvenci několika přechodů.
- **Příklad (Přihlašování):** Stavy (Nepřihlášen, Zadávání, Přihlášen, Zablokován), Události (Zadat jméno, Zadat heslo, Potvrdit...), Akce (Zobrazit chybu...). Testy sledují cesty diagramem.

**Shrnutí pro poznámky:**

- **Co to je:** Technika pro testování systémů s **konečným počtem stavů**. Chování závisí na stavu a událostech.
- **Modely:** **Diagram přechodů stavů** nebo **Stavová tabulka**.
- **Cíl:** Ověřit správnost **přechodů**, **akcí** a reakcí.
- **Pokrytí:** Alespoň **všech platných přechodů** (tím i všech stavů). Testovat i **neplatné**.
- **Test:** Sekvence přechodů.

---

### 4.3 Techniky testování bílé skříňky

#### 4.3.1 Testování a pokrytí příkazů (Statement Testing and Coverage)

- **Princip:** Základní technika bílé skříňky. Cílem je navrhnout testy tak, aby byl **každý spustitelný příkaz** v kódu proveden **alespoň jednou**.
- **Pokrytí:** `(Provedené příkazy / Celkem příkazů) * 100 %`.
- **Omezení:** **Slabé kritérium**, nezaručuje otestování všech větví nebo podmínek.
- **Příklad:** Pro `IF A > B THEN PRINT A ELSE PRINT B ENDIF` stačí 2 testy (jeden pro A>B, druhý pro A<=B) pro 100% pokrytí příkazů.

**Shrnutí pro poznámky:**

- **Co to je:** Základní technika **bílé skříňky**.
- **Cíl:** Provést **každý spustitelný příkaz** alespoň jednou.
- **Pokrytí:** % provedených příkazů.
- **Nevýhody:** **Slabé**, netestuje důkladně větvení/podmínky.

#### 4.3.2 Testování a pokrytí větví (Branch Testing and Coverage)

- **Princip:** Zaměřuje se na **rozhodovací body**. Cílem je navrhnout testy tak, aby byl **každý možný výsledek (větev)** z každého rozhodovacího bodu proveden **alespoň jednou** (např. TRUE i FALSE větev z IF).
- **Pokrytí:** `(Provedené větve / Celkem větví) * 100 %`.
- **Vztah k příkazům:** 100% pokrytí větví **zaručuje** 100% pokrytí příkazů (ne naopak).
- **Příklad:** Pro `IF A > B THEN PRINT A ELSE PRINT B ENDIF` jsou potřeba 2 testy (A>B a A<=B) pro 100% pokrytí větví.
- **Příklad (Bonus):** Funkce s vnořenými IF pro `praxe_roky` a `hodnoceni` měla 4 RB a 8 větví, pokryto 5 testy.
- **Příklad (Doprava):** Funkce s IF/ELSEIF/ELSE pro `vaha_kg` a IF pro `typ_doruceni` měla 3 RB a 6 větví, pokryto 4 testy.
- **Příklad (Login):** Funkce s vnořenými IF pro existenci, heslo, aktivitu, pokusy měla 4 RB a 8 větví, pokryto 5 testy.
- **Příklad (Vstupenka):** Funkce s vnořenými IF pro věk, studenta a den měla 5 RB a 10 větví, pokryto 4 testy.
- **Omezení:** Stále nepokrývá všechny kombinace složených podmínek.

**Shrnutí pro poznámky:**

- **Co to je:** Technika **bílé skříňky** fokusovaná na **rozhodovací body**.
- **Cíl:** Provést **každou větev** (výsledek rozhodnutí, např. TRUE/FALSE) alespoň jednou.
- **Pokrytí:** % provedených větví.
- **Vztah:** 100% pokrytí větví => 100% pokrytí příkazů.
- **Silnější** než pokrytí příkazů.

#### 4.3.3 Přínos (hodnota) testování bílé skříňky

- Důkladnější testování (prověření vnitřní struktury).
- Odhalení specifických defektů kódu (nejen funkčních).
- Časná detekce defektů (levnější oprava).
- Objektivní měření pokrytí (statement, branch...).
- Zvyšování důvěry ve strukturální kvalitu kódu.

**Shrnutí pro poznámky:** Důkladnější testování, odhalení chyb v kódu (i nefunkčních), časná detekce, měřitelné pokrytí, vyšší důvěra.

---

### 4.4 Techniky testování založené na zkušenostech

- **Princip:** Využívají **znalosti, intuici a zkušenosti** testerů. Méně formální, doplňují black/white-box.

#### 4.4.1 Odhadování chyb (Error Guessing)

- **Princip:** Tester "tipuje" (odhaduje), kde by mohly být chyby, na základě znalostí (historie chyb, typické problémy, problematické oblasti) a navrhuje testy k jejich odhalení.
- **Příklad:** Testování speciálních znaků, dlouhých textů, nulových/záporných hodnot tam, kde se nečekají.
- **Výhody:** Efektivní pro zkušené testery.
- **Nevýhody:** Nesystematické, závislé na testerovi, neměří pokrytí.

**Shrnutí pro poznámky:** Tipování chyb na základě zkušeností. Efektivní, ale nesystematické.

#### 4.4.2 Průzkumné testování (Exploratory Testing - ET)

- **Princip:** **Souběžné učení** o systému, **návrh testů** a **provedení testů**. Tester aktivně prozkoumává software.
- **Struktura:** Není náhodné; používá **časové rámce (sessions)**, **listiny testů (Test Charters)** definující cíl/oblast, **zaznamenávání** (Session Sheets) a **diskuze (Debriefing)**.
- **Vhodné pro:** Málo času, nejasné specifikace, rychlé učení, doplněk k skriptovaným testům.
- **Výhody:** Flexibilita, efektivita (pro zkušené), učení.
- **Nevýhody:** Horší reprodukovatelnost/měření pokrytí, závislost na testerovi.

**Shrnutí pro poznámky:** Souběžné učení, návrh a provedení. Strukturované (Sessions, Charters, Logging, Debriefing). Flexibilní, efektivní.

#### 4.4.3 Testování založené na kontrolních seznamech (Checklist-based Testing)

- **Princip:** Tester používá **předpřipravený seznam (checklist)** položek k systematickému ověření. Říká "co" ověřit, ne nutně "jak".
- **Checklist:** Seznam ověřitelných bodů (zkušenosti, standardy, rizika...).
- **Proces:** Projít seznam, ověřit položky, zaznamenat výsledek.
- **Výhody:** Systematičnost, struktura, rychlost, snadná tvorba.
- **Nevýhody:** Riziko povrchnosti, neurčuje "jak", může zastarat.

**Shrnutí pro poznámky:** Systematické ověřování pomocí **předpřipraveného seznamu** položek. Strukturované, ale může být povrchní.

---

### 4.5 Přístupy k testování založené na spolupráci

- **Princip:** Spolupráce **"Tří amigos"** (Byznys, Vývoj, Test) na definici požadavků a testů.

#### 4.5.1 Společné psaní uživatelských scénářů (User Stories)

- **User Story:** Popis funkce z pohledu uživatele (_Jako <role> chci <cíl>, abych <přínos>_). Vzniká diskuzí "Tří amigos".

#### 4.5.2 Akceptační kritéria (Acceptance Criteria - AC)

- **AC:** **Měřitelné podmínky** pro dokončení scénáře. Vznikají ve spolupráci. Jsou to byznys testovací podmínky.
- **Formáty:**
  - **Scenario-oriented (GWT):** Given (kontext) / When (akce) / Then (výsledek).
  - **Rule-oriented (Checklist):** Seznam konkrétních pravidel/kritérií.

#### 4.5.3 Vývoj řízený akceptačními testy (Acceptance Test-Driven Development - ATDD)

- **Princip:** **Akceptační kritéria** (jako spustitelné testy) **řídí vývoj**.
- **Proces:** Diskutuj AC -> Napiš selhávající (automatizovaný) test dle AC -> Napiš kód, aby test prošel -> (Refaktoruj).
- **AC = Testovací případy** na akceptační úrovni.

**Shrnutí pro poznámky (Kolaborativní přístupy a ATDD):**

- **Spolupráce "Tří amigos"** (Byznys+Vývoj+Test) na User Stories a AC.
- **AC:** Měřitelné podmínky dokončení (Formáty: GWT/Scénáře nebo Checklist/Pravidla).
- **ATDD:** AC jako (automatizované) testy řídí vývoj kódu.

---

## Kapitola 5: Management testování (Začátek)

### 5.1 Plánování testování

#### 5.1.1 Účel a obsah plánu testování

- **Účel:** Hlavní dokument pro **strategii, přístup, zdroje, harmonogram**, komunikaci a sledování testování.
- **Obsah:** Co (ne)testovat, Jak (přístup, techniky), Kdy (harmonogram), Kdo (role), Prostředí, Rizika, Kritéria (Pass/Fail, Suspend/Resume), Výstupy.
- **Dynamický:** Aktualizuje se při změnách.

#### 5.1.2 Přínos testerů při plánování iterací a vydání (Agile)

- **Release Planning:** Definice testovatelných AC pro epicy/features, analýza rizik, odhady, strategie.
- **Iteration/Sprint Planning:** Rozpad scénářů na úkoly, testovatelnost, upřesnění AC, rizika, odhady, závislosti.

**Shrnutí pro poznámky (Úvod do Mgmt a Plánování):**

- **Management testování:** Řízení test. procesu (Plánování, Rizika, Monitoring/Řízení, Konfigurace, Defekty).
- **Plán testování:** Klíčový dokument (Co, Jak, Kdy, Kdo, Prostředí, Rizika...). Aktualizovat!
- **Testeři v Agile plánování:** Klíčová role při definici AC, rizik, odhadů, strategie na obou úrovních (Release/Iteration).

---
```

Snad je to takto dostatečně ucelené a přehledné pro tvé potřeby! Prošli jsme toho opravdu hodně.
