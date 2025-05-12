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

**Lekce 1: Kapitola 1.3 - Principy testování**

**Cíl:** Po této lekci bys měl/a být schopen/a vysvětlit sedm principů testování (K2).

**Vysvětlení:**

Existuje sedm základních principů, které by měl každý tester znát a řídit se jimi. Pomáhají nám testovat chytřeji a efektivněji.

**Sedm principů testování:**

1.  **Princip 1: Testování prokazuje přítomnost defektů, nikoli jejich nepřítomnost.**

    - **Vysvětlení:** Testováním můžeme najít chyby. Pokud testy projdou, znamená to, že jsme _v těchto konkrétních scénářích_ žádné chyby nenašli. **Neznamená to ale, že v softwaru žádné další chyby nejsou.** Nikdy nemůžeme s absolutní jistotou říci, že software je 100% bezchybný (ledaže by byl extrémně jednoduchý).
    - **Důsledek:** I když všechny testy projdou, stále existuje riziko, že na produkci se nějaký defekt objeví. Testování snižuje toto riziko, ale neeliminuje ho.

2.  **Princip 2: Vyčerpávající (kompletní) testování není možné.**

    - **Vysvětlení:** Otestovat všechny možné kombinace vstupů, cest kódem, stavů systému a prostředí je u většiny reálných systémů prakticky nemožné. Počet kombinací by byl astronomický a testování by trvalo nekonečně dlouho.
    - **Důsledek:** Místo snahy o nemožné (otestovat vše) se musíme zaměřit na **efektivní testování** – použít techniky analýzy rizik (Kap. 5.2), testovací techniky (Kap. 4) a prioritizaci, abychom otestovali to nejdůležitější a nejrizikovější s omezenými zdroji.

3.  **Princip 3: Včasné testování šetří čas a peníze.**

    - **Vysvětlení:** Čím dříve v životním cyklu vývoje softwaru (SDLC) je defekt nalezen a opraven, tím levnější a jednodušší je jeho oprava. Defekt nalezený v požadavcích stojí na opravu mnohem méně než defekt nalezený až na produkci (kde může způsobit velké škody a jeho oprava je komplexnější).
    - **Důsledek:** Testovací aktivity (včetně statického testování jako revize) by měly začít co nejdříve. Toto souvisí s principem "shift-left".

4.  **Princip 4: Shlukování defektů (Defect clustering).**

    - **Vysvětlení:** Zkušenost ukazuje, že malý počet modulů nebo komponent v systému obvykle obsahuje většinu nalezených defektů. Defekty mají tendenci se "shlukovat" v určitých oblastech.
    - **Důsledek:** Pokud v nějakém modulu najdeme hodně chyb, je pravděpodobné, že tam ještě další budou. Měli bychom na tyto oblasti zaměřit větší testovací úsilí. Tento princip je základem pro risk-based testing. Může to být způsobeno složitostí modulu, novou technologií, méně zkušenými vývojáři atd.

5.  **Princip 5: Testy se opotřebovávají (Beware of the pesticide paradox).**

    - **Vysvětlení:** Pokud budete neustále opakovat stejné testovací případy, jejich schopnost nacházet nové defekty se časem sníží. Je to jako s pesticidy – pokud používáte stále stejný, škůdci si na něj časem vytvoří rezistenci. Software se mění, a i když staré testy mohou stále nacházet regrese, nové chyby už neodhalí.
    - **Důsledek:** Testovací případy je potřeba pravidelně **revidovat a aktualizovat**. Měly by se přidávat nové testy, které pokrývají nové nebo změněné funkce a reagují na nové typy rizik. (Výjimkou mohou být regresní testy, kde je opakování žádoucí).

6.  **Princip 6: Testování je závislé na kontextu.**

    - **Vysvětlení:** Neexistuje jeden univerzální způsob testování, který by byl vhodný pro všechny projekty. Přístup k testování, použité techniky, hloubka a rozsah se musí lišit v závislosti na **kontextu** daného systému a projektu.
    - **Příklady kontextu:** Kritičnost systému (software pro řízení letového provozu se testuje jinak než jednoduchá webová stránka), použitá technologie, typ projektu (agilní vs. waterfall), rizika, časové a finanční omezení, regulatorní požadavky.

7.  **Princip 7: Klam nepřítomnosti chyb (Absence-of-errors fallacy).**
    - **Vysvětlení:** Je klamné si myslet, že pokud software projde všemi testy a nenajdeme žádné chyby, je automaticky úspěšný a kvalitní. Pokud systém sice nemá chyby, ale nesplňuje skutečné potřeby uživatelů, je nepoužitelný nebo horší než konkurence, pak i "bezchybný" software je neúspěšný.
    - **Důsledek:** Nestačí jen ověřovat (Verification - zda dělá věci správně), ale je nutné i validovat (Validation - zda dělá správné věci a splňuje potřeby). I software, který nepadá, může být špatný, pokud je k ničemu.

**Shrnutí pro poznámky (7 Principů testování - K2 vysvětlit):**

1.  **Testování prokazuje přítomnost defektů, ne nepřítomnost:** Najdeme chyby, ale nikdy 100% jistota, že žádné další nejsou.
2.  **Vyčerpávající testování není možné:** Nelze otestovat vše. Nutná prioritizace a výběr.
3.  **Včasné testování šetří čas a peníze:** Chyby nalezené brzy jsou levnější na opravu.
4.  **Shlukování defektů:** Většina chyb bývá v malém počtu modulů.
5.  **Testy se opotřebovávají (Pesticide Paradox):** Stejné testy časem přestanou nacházet nové chyby. Nutná aktualizace.
6.  **Testování je závislé na kontextu:** Přístup se liší dle projektu, rizik, technologie...
7.  **Klam nepřítomnosti chyb:** I bezchybný software může být nepoužitelný, pokud nesplňuje potřeby uživatelů (nutná i validace).

Výborně, jdeme na to.

**Lekce 24: Kapitola 1.4 - Testovací činnosti, testware a role v testování**

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Vysvětlit různé testovací činnosti a související úkoly (K2).
- Vysvětlit vliv kontextu na proces testování (K2).
- Rozlišit mezi různými druhy testwaru podporujícími testovací činnosti (K2).
- Vysvětlit hodnotu udržování trasovatelnosti (K2).
- Porovnat různé role v testování (K2).

**Vysvětlení:**

**1.4.1 Testovací činnosti a úkoly (Test Activities and Tasks)**

I když se testovací proces může lišit v závislosti na kontextu (viz další bod), obvykle zahrnuje několik hlavních skupin činností. Sylabus (a norma ISO/IEC/IEEE 29119-2) je popisuje následovně. Tyto činnosti jsme si už lehce naznačili v Kapitole 5 (Management testování), ale zde se na ně podíváme z obecnějšího pohledu základů.

1.  **Plánování testování (Test Planning):**

    - **Co to je:** Definování cílů testování a přístupu k jejich dosažení v rámci omezení daných kontextem.
    - **Úkoly:** Definování rozsahu, rizik, zdrojů, harmonogramu, vstupních/výstupních kritérií, strategie. Výstupem je **Plán testování**.

2.  **Monitoring a řízení testování (Test Monitoring and Control):**

    - **Co to je:** Průběžné sledování postupu testování oproti plánu (monitoring) a přijímání nápravných opatření (řízení), pokud se objeví odchylky.
    - **Úkoly:** Sběr metrik, reportování stavu, vyhodnocování výstupních kritérií, řízení rizik, rozhodování.

3.  **Testovací analýza (Test Analysis):**

    - **Co to je:** Analýza **testovací báze** (požadavky, návrhy, specifikace, kód, rizika...) s cílem identifikovat, **CO** se má testovat.
    - **Úkoly:** Identifikace testovatelných vlastností, definování **testovacích podmínek** (položek nebo událostí, které by mohly být ověřeny jedním nebo více testovacími případy), přiřazení priorit, hodnocení testovatelnosti testovací báze.

4.  **Návrh testů (Test Design):**

    - **Co to je:** Specifikace, **JAK** se má testovat. Převádí obecné testovací podmínky na konkrétní, vysokoúrovňové (high-level) testovací případy.
    - **Úkoly:** Návrh testovacích případů, identifikace potřebných testovacích dat, návrh testovacího prostředí, identifikace potřebných nástrojů. Používají se zde testovací techniky (Kap. 4).

5.  **Implementace testů (Test Implementation):**

    - **Co to je:** Příprava všeho potřebného pro **provedení** testů.
    - **Úkoly:** Vytvoření konkrétních testovacích dat, sestavení testovacího prostředí, vytvoření a verifikace testovacích skriptů (manuálních i automatizovaných), uspořádání testovacích případů do **testovacích procedur (test scripts)** a ty pak do **testovacích sad (test suites)**, vytvoření harmonogramu provádění testů.

6.  **Provedení testů (Test Execution):**

    - **Co to je:** Spouštění testovacích sad podle harmonogramu.
    - **Úkoly:** Provedení testů (manuálně nebo pomocí nástrojů), porovnání **skutečných výsledků** s **očekávanými výsledky**, zaznamenávání výsledků (prošel/selhal/zablokován), reportování defektů při selhání, logování.

7.  **Dokončení testování (Test Completion):**
    - **Co to je:** Aktivity prováděné na konci testovací fáze nebo projektu.
    - **Úkoly:** Kontrola splnění výstupních kritérií, archivace testwaru, ponaučení (lessons learned), vytvoření **souhrnného reportu z testování**.

**Důležité:** Tyto činnosti nejsou striktně sekvenční, často se provádějí iterativně a paralelně. Například analýza a návrh pro jednu funkci mohou probíhat, zatímco se provádějí testy pro jinou, již dokončenou funkci.

**1.4.2 Vliv kontextu na proces testování**

Jak už jsme zmínili u Principu 6, testování je silně závislé na kontextu. To znamená, že **neexistuje jeden univerzální testovací proces**. Faktory kontextu ovlivňují, jaké činnosti se budou provádět, jak detailně, kým a kdy.

**Faktory kontextu zahrnují (příklady):**

- **Model životního cyklu vývoje softwaru (SDLC):** V agilním vývoji bude proces jiný (kratší iterace, častější zpětná vazba, více automatizace) než ve waterfall modelu (dlouhé fáze, formálnější dokumentace).
- **Rizika spojená s produktem a projektem:** Vysoce rizikové systémy vyžadují důkladnější a formálnější testování.
- **Požadavky (funkční i nefunkční):** Složitost a typ požadavků ovlivní výběr technik a hloubku testování.
- **Dovednosti a zkušenosti týmu:** Dostupnost zkušených testerů a vývojářů.
- **Časové a rozpočtové omezení:** Často nutí k prioritizaci a kompromisům.
- **Použité nástroje a technologie.**
- **Regulatorní požadavky a standardy.**
- **Organizační kultura a procesy.**

Například pro jednoduchou webovou stránku může být testovací proces méně formální a kratší, zatímco pro software v lékařském zařízení bude vyžadovat detailní dokumentaci, vysoké pokrytí a striktní dodržování standardů.

**1.4.3 Testware**

- **Co to je:** Testware jsou **všechny pracovní produkty (artefakty)**, které vznikají během testovacího procesu a jsou používány při testování.
- **Příklady testwaru (už jsme je potkali v různých činnostech):**
  - **Plánovací dokumenty:** Plán testování, strategie testování.
  - **Specifikační dokumenty pro testy:** Testovací podmínky, testovací případy, testovací procedury (skripty), testovací sady (suites), testovací listiny (charters).
  - **Testovací data:** Vstupní data pro testy, očekávané výsledky.
  - **Konfigurace testovacího prostředí:** Popis a nastavení prostředí.
  - **Nástroje a jejich skripty:** Automatizované testovací skripty, výkonnostní skripty.
  - **Výsledky a reporty:** Logy z provedení testů, reporty o defektech, reporty o postupu, souhrnné reporty.
- **Důležitost:** Kvalitní a dobře spravovaný testware je klíčem k efektivnímu a opakovatelnému testování. Měl by být pod **konfiguračním managementem** (Kap. 5.4).

**1.4.4 Hodnota udržování trasovatelnosti (Traceability)**

- **Co to je trasovatelnost:** Schopnost **propojit a sledovat vztahy** mezi různými pracovními produkty. V kontextu testování je nejdůležitější **obousměrná trasovatelnost** mezi:
  - **Testovací bází** (požadavky, uživatelské scénáře, rizika, komponenty návrhu...)
  - **Testovacími podmínkami**
  - **Testovacími případy**
  - **Provedením testů (výsledky)**
  - **Defekty**
- **Proč je důležitá (hodnota):**
  1.  **Analýza pokrytí:** Umožňuje zjistit, které požadavky jsou pokryty testy, a které ne. Kolik testů testuje dané riziko?
  2.  **Analýza dopadu změn (Impact Analysis):** Pokud se změní požadavek, trasovatelnost nám pomůže identifikovat, které testy je potřeba upravit, zopakovat nebo přidat.
  3.  **Auditovatelnost a shoda:** Pomáhá doložit, že všechny požadavky byly otestovány (důležité pro regulované prostředí).
  4.  **Pochopení vztahů:** Usnadňuje pochopení, proč byl daný test navržen (k jakému požadavku/riziku se váže).
  5.  **Reportování:** Umožňuje reportovat stav testování ve vztahu k požadavkům nebo rizikům (např. kolik % požadavků je otestováno a prošlo).
  6.  **Řízení rizik:** Pomáhá zajistit, že rizika s vyšší prioritou jsou pokryta adekvátními testy.

Udržování trasovatelnosti může být náročné, ale její přínosy často převáží. Nástroje pro test management a requirements management mohou tuto činnost výrazně usnadnit.

**1.4.5 Role v testování**

Sylabus rozlišuje dvě hlavní role (ale v praxi jich může být více a názvy se mohou lišit):

1.  **Manažer testování (Test Manager) / Vedoucí tester (Test Lead):**

    - **Odpovědnost:** Celkové řízení testovacího procesu, plánování, zdroje, rozpočet, strategie, komunikace s managementem a ostatními stranami.
    - **Typické činnosti:** Vytváření plánu testování, definování strategie, koordinace týmu, monitoring a řízení, reportování, management rizik a defektů, výběr nástrojů, zajištění zdrojů.
    - V agilním prostředí mohou být některé tyto zodpovědnosti distribuovány v rámci celého týmu.

2.  **Tester / Testovací analytik (Test Analyst) / Technický tester (Technical Tester):**
    - **Odpovědnost:** Provádění konkrétních testovacích činností.
    - **Typické činnosti:** Revize testovací báze, analýza a návrh testů, příprava testovacích dat a prostředí, implementace testů (včetně automatizace), provedení testů, reportování defektů, dokumentace výsledků.
    - Rozdíl mezi analytikem a technickým testerem může být v zaměření – analytik se více soustředí na _co_ testovat a návrh z pohledu byznysu/funkčnosti, technický tester na _jak_ testovat, automatizaci, nefunkční testy. V základním sylabu se tyto role často slučují.

**Důležité:** Nezávislost testerů (viz Kap. 1.5.3) může ovlivnit efektivitu. Role mohou být také kombinovány nebo vykonávány různými lidmi v různých fázích.

**Shrnutí pro poznámky (Testovací činnosti, Testware, Role):**

- **Testovací činnosti (K2 - vysvětlit):**
  1.  Plánování
  2.  Monitoring a Řízení
  3.  Analýza (CO testovat -> testovací podmínky)
  4.  Návrh (JAK testovat -> high-level test. případy)
  5.  Implementace (příprava pro provedení -> test. data, prostředí, skripty, sady)
  6.  Provedení (spuštění, porovnání výsledků, reportování defektů)
  7.  Dokončení (archivace, lessons learned, souhrnný report)
  - _Nejsou striktně sekvenční, často iterativní/paralelní._
- **Vliv kontextu na proces (K2 - vysvětlit):** SDLC, rizika, požadavky, tým, zdroje, nástroje, regulace – to vše ovlivňuje, jak se testuje.
- **Testware (K2 - rozlišit druhy):** Všechny pracovní produkty testování (plány, případy, data, skripty, prostředí, reporty...). Spravovat pomocí KM.
- **Trasovatelnost (K2 - vysvětlit hodnotu):** Propojení mezi test. bází, testy, výsledky, defekty. Pomáhá s pokrytím, analýzou dopadu změn, auditem.
- **Role v testování (K2 - porovnat):**
  - **Manažer testování:** Plánování, strategie, řízení, zdroje, komunikace.
  - **Tester:** Analýza, návrh, implementace, provedení, reportování defektů.

Uf, to byla opět obsáhlá lekce! Zahrnuje jádro testovacího procesu. Jsi připraven/a na otázky?
