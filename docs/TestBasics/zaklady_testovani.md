**Lekce 1: Kapitola 1 - Základy testování (Úvod) a Kapitola 1.1 - Co je to testování?**

**Cíl:** Po této lekci byste měli být schopni:

1.  Identifikovat typické cíle testování (K1).
2.  Odlišit testování od ladění (debugging) (K2).

**Vysvětlení:**

### 1 Úvod do Základů testování

Tato kapitola položí základy pro všechno, co následuje. Řekneme si, co to testování vlastně je, proč je důležité, jaké má principy, jaké jsou základní činnosti a role.

### 1.1 Co je to testování?

Možná to zní jako jednoduchá otázka, ale definice testování je širší, než si mnoho lidí myslí.

- **Není to jen klikání:** Testování **není** jen spouštění softwaru a náhodné zkoušení, jestli něco spadne. Je to **systematický proces**.
- **Co to tedy je?** Testování softwaru je sada činností, jejichž cílem je **hodnotit kvalitu** softwarových pracovních produktů (nejen kódu, ale i požadavků, návrhů...) a **identifikovat defekty** (chyby).
- **Testovaný objekt:** Cokoli, co testujeme (komponenta, modul, systém, dokumentace).
- **Ověření (Verification) vs. Validace (Validation):**

- **Ověření (Verification):** "Stavíme produkt správně?" Kontrolujeme, zda software splňuje **specifikované požadavky** (např. design, standardy kódování, funkční specifikace).
- **Validace (Validation):** "Stavíme správný produkt?" Kontrolujeme, zda software splňuje **potřeby uživatelů a dalších zainteresovaných stran** v jeho provozním prostředí. Splňuje účel, pro který byl vytvořen?
- Testování zahrnuje **obojí** – ověřujeme, zda dělá věci správně, a validujeme, zda dělá správné věci.
- **Statické vs. Dynamické testování:**

- **Statické testování:** Testování **bez spuštění kódu**. Zahrnuje revize dokumentů (požadavky, návrhy, kód) a statickou analýzu kódu (pomocí nástrojů). Probereme v Kapitole 3.
- **Dynamické testování:** Testování **spuštěním kódu**. Zahrnuje provedení testovacích případů a sledování chování systému. Tomu jsme se věnovali v Kapitole 4 (techniky).
- **Intelektuální činnost:** Testování vyžaduje analytické myšlení, kritické myšlení, kreativitu, znalosti domény a technické dovednosti.

#### 1.1.1 Typické cíle testování

Proč vlastně testujeme? Cíle se mohou lišit v závislosti na kontextu projektu, úrovni testování a dalších faktorech, ale typické cíle zahrnují:

1.  **Hodnocení pracovních produktů:** Posouzení kvality požadavků, uživatelských scénářů, návrhů, kódu atd.
2.  **Vyvolání selhání a nalezení defektů:** Toto je často vnímáno jako hlavní cíl – aktivně hledat chyby, aby mohly být opraveny.
3.  **Zajištění požadovaného pokrytí testovaného objektu:** Mít jistotu, že jsme otestovali všechny důležité části nebo funkce.
4.  **Snížení úrovně rizika plynoucí z nedostatečné kvality softwaru:** Odhalením a umožněním opravy chyb snižujeme pravděpodobnost, že software selže v produkci a způsobí problémy.
5.  **Ověření, zda byly splněny stanovené požadavky (Verification):** Kontrola shody se specifikací.
6.  **Ověření, že testovaný objekt vyhovuje smluvním, právním a regulatorním požadavkům:** Např. GDPR, bezpečnostní normy.
7.  **Poskytnutí informací zainteresovaným stranám:** Aby mohly učinit kvalifikovaná rozhodnutí (např. o vydání produktu, o dalším postupu).
8.  **Vytvoření důvěry v danou úroveň kvality testovaného objektu:** Ukázat, že systém funguje podle očekávání a je spolehlivý.
9.  **Kontrola, zda je testovaný objekt kompletní a funguje dle očekávání všech zainteresovaných stran (Validation).**

#### 1.1.2 Testování a ladění (Debugging)

Toto je velmi důležité rozlišení, které se často plete!

- **Testování (Testing):**

- **Cíl:** Najít defekty, vyvolat selhání, posoudit kvalitu.
- **Kdo:** Primárně testeři (ale i vývojáři, uživatelé...).
- **Činnost:** Navrhování a provádění testů, analýza výsledků, reportování defektů. Testování **ukazuje přítomnost defektů**.
- **Ladění (Debugging):**

* **Cíl:** Najít **příčinu** selhání (tedy konkrétní defekt v kódu nebo návrhu), analyzovat ji a **opravit** ji.
* **Kdo:** Primárně vývojáři.
* **Činnost:** Analýza kódu, sledování provádění, používání ladicích nástrojů, oprava kódu. Ladění **odstraňuje defekty**.

**Jak to souvisí:**
Testování může vyvolat selhání. Pokud k selhání dojde, tester nahlásí problém (report o defektu). Vývojář pak vezme tento report a začne proces ladění, aby našel a opravil defekt, který selhání způsobil. Poté následuje **konfirmační testování** (provádí tester), aby se ověřilo, že oprava byla úspěšná.

**Shrnutí pro poznámky (Co je testování?, Cíle, Testování vs. Ladění):**

- **Testování:** Systematický proces **hodnocení kvality** a **identifikace defektů** v softwarových pracovních produktech. Zahrnuje **Ověření** (Verification - děláme věci správně?) a **Validaci** (Validation - děláme správné věci?). Může být **Statické** (bez spuštění) nebo **Dynamické** (se spuštěním).
- **Typické cíle testování (K1 - zapamatovat si některé):** Najít defekty, snížit riziko, ověřit požadavky, poskytnout info, vybudovat důvěru, posoudit kvalitu, zajistit pokrytí.
- **Testování vs. Ladění (K2 - odlišit):**
  - **Testování:** Hledá defekty (vyvolává selhání). Provádí tester.
  - **Ladění (Debugging):** Hledá příčinu selhání (defekt) a opravuje ji. Provádí vývojář.
  - Proces: Testování -> Selhání -> Report defektu -> Ladění (oprava) -> Konfirmační testování.

Výborně, pojďme na to.

**Lekce 22: Kapitola 1.2 - Proč je testování nezbytné?**

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Ilustrovat na příkladech, proč je testování nezbytné (K2).
- Vybavit si vztah mezi testováním a zajištěním kvality (QA) (K1).
- Rozlišit mezi kořenovou příčinou, chybou, defektem a selháním (K2).

**Vysvětlení:**

### 1.2.1 Ilustrace nezbytnosti testování

Už jsme si naznačili, že software je všude kolem nás a jeho selhání může mít různé následky. Testování je nezbytné, protože:

- **Minimalizuje rizika:** Software, který nefunguje správně, může vést k:
  - **Finančním ztrátám:** Chyba v e-shopu může způsobit ztrátu objednávek; chyba v bankovním systému může vést k nesprávným transakcím.
  - **Ztrátě času a zdrojů:** Oprava chyb na produkci je mnohem dražší než jejich odhalení a oprava během vývoje. Uživatelé mohou ztrácet čas kvůli nefunkčnímu softwaru.
  - **Poškození reputace:** Firma, která vydává chybový software, rychle ztratí důvěru zákazníků.
  - **Právním následkům:** V některých odvětvích (např. zdravotnictví, finance, letectví) mohou chyby vést k porušení zákonů a regulací, což může mít za následek pokuty nebo jiné sankce.
  - **Zranění nebo smrti:** U kritických systémů (např. řízení letového provozu, lékařské přístroje, autonomní vozidla) může selhání softwaru mít fatální následky.
- **Zvyšuje kvalitu produktu:** Testování pomáhá odhalovat a odstraňovat defekty, což vede k vyšší spolehlivosti, použitelnosti a celkové kvalitě softwaru. Uživatelé jsou spokojenější s produktem, který funguje podle očekávání.
- **Pomáhá splnit požadavky:** Ověřuje, zda software odpovídá specifikacím, smluvním závazkům a regulatorním požadavkům.
- **Poskytuje důvěru:** Úspěšné testování dává zainteresovaným stranám (managementu, zákazníkům) větší důvěru, že produkt je připraven k nasazení a bude fungovat spolehlivě.

**Příklady z reálného světa (ilustrativní):**

- **Therac-25 (lékařský přístroj pro radioterapii):** Softwarová chyba způsobila, že pacienti dostali mnohonásobně vyšší dávky záření, což vedlo k několika úmrtím a zraněním. Důkladné testování mohlo tuto tragédii odvrátit.
- **Ariane 5 (raketa):** Chyba v softwaru při převodu dat způsobila sebedestrukci rakety krátce po startu, což vedlo ke ztrátě nákladu v hodnotě stovek milionů dolarů.
- **Knight Capital Group (finanční firma):** Chyba v nově nasazeném obchodním softwaru způsobila během 45 minut ztrátu přes 400 milionů dolarů a téměř bankrot firmy.

Tyto příklady ukazují, že investice do kvalitního testování se často mnohonásobně vrátí prevencí mnohem větších škod.

### 1.2.2 Testování a zajištění kvality (Quality Assurance - QA)\*\*

Je důležité rozlišovat mezi testováním a zajištěním kvality (QA), i když jsou úzce spjaty.

- **Testování (Testing):** Jak už víme, je to sada aktivit zaměřená na **hodnocení kvality produktu a hledání defektů**. Je to spíše **reaktivní** a **produktově orientovaná** činnost (i když včasné testování má i preventivní aspekty). Je součástí Řízení kvality (QC).
- **Řízení kvality (Quality Control - QC):** Zahrnuje různé aktivity (včetně testování) zaměřené na **splnění požadavků na kvalitu**. Je to o kontrole a ověřování.
- **Zajištění kvality (Quality Assurance - QA):** Je to mnohem širší koncept. QA se zaměřuje na **procesy a systém** vývoje softwaru s cílem **předcházet vzniku defektů** a zajistit, že procesy vedou k produkci kvalitního softwaru. Je to **proaktivní** a **procesně orientovaná** činnost. QA se snaží "zabudovat kvalitu do procesu".
  - QA zahrnuje aktivity jako definování standardů a procesů, audity, školení, výběr nástrojů, zlepšování procesů atd.
  - Dobré QA by mělo vést k tomu, že testování odhalí méně defektů, protože jich méně vznikne.

**Vztah:** Testování je jednou z klíčových aktivit v rámci Řízení kvality (QC), a QC i QA společně přispívají k celkové kvalitě. QA nastavuje rámec a procesy, QC (včetně testování) kontroluje, zda je produkt v souladu s požadavky.

### 1.2.3 Chyba, defekt, selhání a kořenová příčina

Tyto termíny se často zaměňují, ale mají specifické významy:

1.  **Chyba (Error / Mistake):**
    - **Lidská akce**, která produkuje nesprávný výsledek.
    - _Příklad:_ Programátor udělá překlep v kódu, analytik špatně pochopí požadavek zákazníka, tester špatně navrhne testovací případ.
2.  **Defekt (Defect / Bug / Fault):**
    - **Nedokonalost nebo nedostatek** v pracovním produktu (např. v kódu, dokumentaci, návrhu), který je **důsledkem chyby**.
    - Pokud je defekt v kódu spuštěn, může (ale nemusí) způsobit selhání.
    - _Příklad:_ Překlep programátora (chyba) vede k tomu, že v kódu je špatná podmínka (defekt). Špatně pochopený požadavek (chyba) vede k chybějící funkcionalitě ve specifikaci (defekt).
3.  **Selhání (Failure):**
    - **Projev defektu** při spuštění softwaru. Je to **neschopnost systému provést požadovanou funkci** v rámci specifikovaných limitů. Systém se nechová tak, jak by měl.
    - _Příklad:_ Špatná podmínka v kódu (defekt) způsobí, že se při určitém vstupu špatně vypočítá cena (selhání). Chybějící funkcionalita ve specifikaci (defekt) vede k tomu, že uživatel nemůže provést očekávanou akci (selhání).
    - **Ne každý defekt způsobí selhání!** Některé defekty mohou být v kódu, který se nikdy nespustí, nebo se projeví jen za velmi specifických okolností.
4.  **Kořenová příčina (Root Cause):**
    - **Původní důvod nebo zdroj chyby**, která vedla k defektu. Identifikace a odstranění kořenové příčiny je klíčové pro prevenci opakování podobných chyb v budoucnu.
    - _Příklad:_ Programátor udělal překlep (chyba), protože byl pod velkým časovým tlakem a unavený (kořenová příčina). Analytik špatně pochopil požadavek (chyba), protože nebyla provedena dostatečná komunikace se zákazníkem a chyběly jasné procesy pro ověření požadavků (kořenová příčina).

**Vztah:** Lidská **Chyba** -> vede k **Defektu** (v kódu/dokumentu) -> který se může projevit jako **Selhání** (při spuštění) -> a to vše má nějakou **Kořenovou příčinu**. Testování se snaží odhalit selhání (a někdy přímo defekty), ladění hledá defekty a analýza kořenových příčin pomáhá zlepšovat procesy.

**Shrnutí pro poznámky (Proč je testování nezbytné?, QA, Chyba/Defekt/Selhání):**

- **Nezbytnost testování (K2 - ilustrovat):** Minimalizuje rizika (finanční ztráty, ztráta času/reputace, právní následky, zranění/smrt), zvyšuje kvalitu, pomáhá splnit požadavky, poskytuje důvěru.
- **Testování vs. QA (K1 - vybavit si vztah):**
  - **Testování:** Činnost hodnocení kvality produktu a hledání defektů (součást QC).
  - **QA (Zajištění kvality):** Širší, procesně orientovaný přístup k prevenci defektů a zajištění kvality procesů.
- **Chyba, Defekt, Selhání, Kořenová příčina (K2 - rozlišit):**
  - **Chyba (Error):** Lidská akce vedoucí k nesprávnému výsledku.
  - **Defekt (Bug/Fault):** Nedokonalost v produktu (kód, dokument) způsobená chybou.
  - **Selhání (Failure):** Projev defektu při spuštění (systém se nechová, jak má).
  - **Kořenová příčina (Root Cause):** Původní důvod vzniku chyby.
  - Řetězec: Kořenová příčina -> Chyba -> Defekt -> (může způsobit) Selhání.
