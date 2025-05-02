# Kapitola 5: Management testování

Vítejte v sekci věnované managementu testování!

## Lekce 5: Úvod do Managementu testování a Plánování testování (Kap. 5 a 5.1)

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Chápat obecný účel managementu testování.
- Ilustrovat na příkladech účel a obsah plánu testování (K2).
- Určit, jakou přidanou hodnotou má přítomnost testerů pro plánování iterací a plánování vydání (K1).

---

### Co je Management testování?

**Management testování** zahrnuje všechny aktivity spojené s řízením a kontrolou testovacího procesu během celého životního cyklu projektu. Nejde jen o samotné testování, ale o komplexní proces zahrnující:

- **Plánování:** Co, jak, kdy, kým bude testováno?
- **Organizaci:** Sestavení týmu, přidělení rolí.
- **Sledování (Monitoring):** Jak postupujeme oproti plánu?
- **Řízení (Control):** Jak reagujeme na odchylky a problémy?
- **Reportování:** Komunikace stavu a výsledků.

Cílem je zajistit, aby testování bylo **efektivní**, **účinné** a přispívalo k celkovým cílům projektu (dodání kvalitního softwaru včas a v rámci rozpočtu).

**Hlavní oblasti managementu testování (probereme v Kapitole 5):**

1.  **Plánování testování** (Kap. 5.1)
2.  **Management rizik** (Kap. 5.2)
3.  **Monitoring, řízení a dokončení testování** (Kap. 5.3)
4.  **Konfigurační management** (Kap. 5.4)
5.  **Management defektů** (Kap. 5.5)

Začneme plánováním.

---

## Kapitola 5.1: Plánování testování

### 5.1.1 Účel a obsah plánu testování

**Účel Plánu Testování:**

Plán testování je **klíčový dokument**, který definuje **strategii a přístup** k testování. Slouží jako:

- **Průvodce:** Definuje cíle, rozsah, zdroje, harmonogram a zodpovědnosti.
- **Komunikační nástroj:** Sdílí informace o testování s týmem a zainteresovanými stranami.
- **Základ pro monitoring:** Umožňuje sledovat postup testování oproti plánu.
- **Dokumentace:** Potvrzuje soulad testování s politikami a standardy.

**Kdo ho vytváří:** Obvykle manažer testování nebo vedoucí tester, ve spolupráci s týmem a stakeholdery.

**Typický obsah plánu testování (dle IEEE 29119-3, může se lišit):**

- **Identifikátor plánu:** Jedinečné označení.
- **Úvod:** Kontext projektu, cíle testování.
- **Testované položky (Test Items):** Co se bude testovat (moduly, funkce, systém...). Odkazy na testovací bázi.
- **Testované vlastnosti/funkce (Features to be Tested):** Které aspekty/požadavky se budou testovat.
- **Vlastnosti/funkce, které se testovat nebudou (Features not to be Tested):** Co je mimo rozsah a proč.
- **Přístup k testování (Approach):** Celková strategie, úrovně, typy testování, hlavní techniky.
- **Kritéria úspěšnosti položky (Item Pass/Fail Criteria):** Jak se rozhodne o úspěchu/selhání testu položky.
- **Kritéria pozastavení a obnovení (Suspension Criteria and Resumption Requirements):** Kdy testování pozastavit a kdy obnovit.
- **Výstupy z testování (Test Deliverables):** Jaké dokumenty a artefakty vzniknou (plány, případy, reporty...).
- **Testovací úlohy (Testing Tasks):** Kdo co udělá (příprava, provedení, reporting...).
- **Potřeby prostředí (Environmental Needs):** Hardware, software, nástroje, data, konfigurace...
- **Zodpovědnosti (Responsibilities):** Kdo je za co zodpovědný.
- **Personální zajištění a školení (Staffing and Training Needs):** Kdo bude testovat a jaké školení potřebuje.
- **Harmonogram (Schedule):** Milníky, závislosti, termíny.
- **Rizika a záložní plány (Risks and Contingencies):** Potenciální hrozby a reakce na ně (viz Kap. 5.2).
- **Schválení (Approvals):** Kdo musí plán schválit.

**Důležité:** Plán testování je **živý dokument** a měl by být **aktualizován** při významných změnách.

### 5.1.2 Přínos testerů při plánování iterací a vydání (Agile)

V agilních přístupech mají testeři klíčovou roli v různých úrovních plánování:

**Plánování vydání (Release Planning - dlouhodobější pohled):**

- Pomáhají definovat **testovatelná akceptační kritéria** pro větší celky (epicy, features).
- Podílí se na **analýze rizik** na úrovni produktu/vydání.
- Přispívají k **odhadům pracnosti** pro testovací aktivity v rámci vydání.
- Pomáhají definovat **celkovou strategii testování** napříč iteracemi.

**Plánování iterace/sprintu (Iteration/Sprint Planning - krátkodobý pohled):**

- Podílí se na **rozpadu uživatelských scénářů** na konkrétní (testovací) úkoly.
- Pomáhají **identifikovat testovatelnost** scénářů.
- Upřesňují **akceptační kritéria** pro scénáře v iteraci.
- Provádějí **detailnější analýzu rizik** pro scénáře v iteraci.
- Provádějí **odhady pracnosti** pro testovací úkoly v iteraci.
- Pomáhají identifikovat **závislosti** mezi úkoly.

---

**Shrnutí pro poznámky (Úvod do Mgmt a Plánování):**

- **Management testování:** Řízení a kontrola test. procesu (Plánování, Rizika, Monitoring/Řízení, Konfigurace, Defekty).
- **Plán testování:**
- **Účel:** Hlavní dokument (strategie, přístup, zdroje, harmonogram, komunikace).
- **Obsah:** Co (ne)testovat, Jak (přístup), Kdy (harmonogram), Kdo (role), Prostředí, Rizika, Kritéria, Výstupy.
- **Dynamický:** Aktualizovat dle potřeby.
- **Role testerů v Agilním plánování:**
- **Release Planning:** AC pro epicy, rizika, odhady, strategie.
- **Iteration/Sprint Planning:** Rozpad scénářů, testovatelnost, AC, rizika, odhady, závislosti.

---

### 5.1.3 Vstupní a výstupní kritéria (Entry and Exit Criteria)

Při plánování testování (a řízení jakékoli jiné aktivity) je důležité definovat, **kdy můžeme s danou aktivitou (nebo její fází) začít** a **kdy ji můžeme považovat za dokončenou**. K tomu slouží vstupní a výstupní kritéria.

**Vstupní kritéria (Entry Criteria):**

- **Co to je:** Definují **předpoklady**, které **musí být splněny, ABY mohla daná testovací aktivita** (např. úroveň testování jako systémové testování, nebo provedení specifické sady testů) **ZAČÍT**.
- **Účel:** Zajistit, že máme vše potřebné připraveno a že začátek testování má smysl a je efektivní. Pokud vstupní kritéria nejsou splněna, začátek testování by byl pravděpodobně obtížný, nákladný, neefektivní nebo dokonce nemožný.
- **Příklady vstupních kritérií:**
- **Dostupnost zdrojů:** Jsou k dispozici testeři, nástroje, finance?
- **Připravenost testovacího prostředí:** Je prostředí nainstalováno, nakonfigurováno, stabilní? Jsou dostupná testovací data?
- **Připravenost testovací báze:** Jsou požadavky schválené a dostatečně kvalitní? Jsou uživatelské scénáře jasné?
- **Připravenost testwaru:** Jsou testovací případy navržené a zrevidované? Jsou připraveny testovací skripty?
- **Připravenost testovaného objektu:** Je kód dodaný (build), nainstalovaný v testovacím prostředí? Prošel základními "smoke testy" (ověření, že se systém vůbec spustí a základní funkce fungují)?

**Výstupní kritéria (Exit Criteria):**

- **Co to je:** Definují **podmínky**, které **musí být splněny, ABY mohla být daná testovací aktivita UKONČENA** a považována za dokončenou.
- **Účel:** Objektivně určit, kdy jsme dosáhli stanovených cílů testování a můžeme danou fázi ukončit (např. předat výsledky, začít další fázi). Pomáhají rozhodnout, zda je testovaný software připraven pro další krok (např. nasazení, další úroveň testování).
- **Často spojována s "Definition of Done" (DoD):** V agilním prostředí jsou výstupní kritéria často klíčovou součástí Definition of Done pro uživatelský scénář, sprint nebo release.
- **Příklady výstupních kritérií:**
- **Pokrytí:** Bylo dosaženo požadované úrovně pokrytí (např. 100% pokrytí požadavků testy, 95% pokrytí větví pro kritické moduly)?
- **Výsledky testů:** Byly provedeny všechny plánované testy? Jaký je poměr úspěšných a neúspěšných testů?
- **Defekty:** Kolik je otevřených defektů? Jaká je jejich závažnost a priorita? Byl dosažen plánovaný počet nebo hustota defektů (defects density)? Jsou všechny kritické defekty opraveny a ověřeny?
- **Důvěra:** Je dosaženo dostatečné úrovně důvěry v kvalitu produktu (může být subjektivní, ale často založeno na ostatních kritériích)?
- **Termíny a rozpočet:** Byly dodrženy plánované termíny a rozpočet (i když samotné vyčerpání rozpočtu/času nemusí být nutně platným důvodem pro ukončení, pokud nejsou splněna kritéria kvality, viz níže)?

**Důležité aspekty:**

- **Definice v plánu:** Vstupní i výstupní kritéria by měla být jasně definována už ve fázi **plánování testování** a uvedena v plánu testování.
- **Měřitelnost:** Kritérium by mělo být pokud možno objektivně měřitelné.
- **Realističnost:** Měla by být dosažitelná v rámci projektu.
- **Kontext:** Liší se projekt od projektu, pro různé úrovně testování mohou být definována odlišná kritéria.
- **Riziko při nesplnění:** Pokud se rozhodne ukončit testování i přes nesplnění výstupních kritérií (např. kvůli tlaku na termín), mělo by být jasně zdokumentováno **akceptované riziko**.

---

**Shrnutí pro poznámky (Plánování - Pokračování):**

- **Vstupní kritéria (Entry Criteria):**
- **Co:** Předpoklady pro **zahájení** testovací aktivity.
- **Účel:** Zajistit připravenost, efektivitu.
- **Příklady:** Zdroje, prostředí, test. báze, testware, test. objekt (vč. smoke testů).
- **Výstupní kritéria (Exit Criteria):**
- **Co:** Podmínky pro **dokončení** testovací aktivity.
- **Účel:** Objektivně určit dokončení, připravenost pro další krok. Často součást **DoD**.
- **Příklady:** Pokrytí, výsledky testů, stav defektů, důvěra, (harmonogram/rozpočet).
- **Společné:** Definice v **plánu**, **měřitelnost**, **kontext**, nesplnění výstupních kritérií = **dokumentovat riziko**.
