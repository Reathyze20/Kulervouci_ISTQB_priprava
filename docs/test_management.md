# Kapitola 5: Management testování

Vítejte v sekci věnované managementu testování!

## Poznámky ISTQB CTFL 4.0 – Kapitola 5

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

Paráda! Odhady jsou častým úkolem (a někdy i strašákem) v projektovém řízení, včetně testování.

**Lekce 15: Kapitola 5.1.4 - Techniky pro odhadování pracnosti testování**

**Cíl:** Po této lekci bys měl/a být schopen/a použít techniky odhadování pro výpočet pracnosti potřebné při testování (K3).

**Vysvětlení:**

**Co je odhad pracnosti testování?**

Je to předpověď (nikoli závazek!) množství práce (obvykle vyjádřené v člověkohodinách, člověkodnech apod.), která bude pravděpodobně potřeba k provedení definovaných testovacích aktivit a dosažení cílů testování. Odhady jsou klíčové pro:

- **Plánování:** Určení délky trvání, potřebných zdrojů (lidí), nákladů.
- **Řízení:** Porovnávání skutečné pracnosti s plánem a identifikaci odchylek.
- **Komunikaci:** Poskytnutí informací managementu a dalším stranám.

**Faktory ovlivňující odhad:**

Odhady ovlivňuje mnoho faktorů, například:

- **Produktové faktory:** Složitost domény, požadovaná kvalita, velikost produktu, rizika produktu.
- **Procesní faktory:** Zvolený SDLC model, vyspělost testovacího procesu, dostupné nástroje, tlak na termíny.
- **Lidské faktory:** Zkušenosti a dovednosti týmu (nejen testerů, ale i vývojářů, analytiků...), komunikace v týmu.

**Techniky odhadování (Sylabus zmiňuje čtyři):**

1.  **Odhad na základě metrik (Metrics-based approach):**

- **Princip:** Využívá historická data a "standardizované" metriky z předchozích, podobných projektů v dané organizaci.
- **Příklad:** Víme, že v minulých projektech byla pracnost testování typicky 40 % pracnosti vývoje. Pokud je odhad vývoje pro nový projekt 500 člověkodnů, odhadneme pracnost testování na 0.4 _ 500 = 200 člověkodnů. Nebo víme, že návrh a provedení testů pro jeden "středně složitý" funkční požadavek trvá průměrně 4 hodiny. Pokud máme 50 takových požadavků, odhad je 50 _ 4 = 200 člověkohodin.
- **Výhody:** Pokud jsou historická data relevantní a kvalitní, může být poměrně přesný.
- **Nevýhody:** Vyžaduje existenci a spolehlivost historických dat z _podobných_ projektů.

2.  **Odhad na základě expertízy (Expert-based approach):**

- **Princip:** Využívá znalosti a zkušenosti expertů (např. zkušených testerů, manažerů testů, vývojářů, byznys analytiků) na danou oblast nebo technologii. Experti odhadnou pracnost na základě svého úsudku.
- **Techniky využívající expertní odhad:**
  - **Wideband Delphi:** Iterativní technika. Skupina expertů provede **nezávislé anonymní odhady**. Odhady se shromáždí, ukáží (stále anonymně, často rozsah nebo průměr), experti o nich **diskutují** (zejména o důvodech pro extrémní hodnoty) a pak provedou **další kolo anonymních odhadů**. Proces se opakuje, dokud se odhady nesblíží (nedosáhne se konsenzu) nebo dokud není další kolo neproduktivní. Cílem je snížit vliv dominantních jedinců a využít kolektivní moudrosti.
  - **Plánovací poker (Planning Poker):** Často používané v agilu. Každý člen týmu (expert) má sadu karet s čísly (často Fibonacciho řada: 1, 2, 3, 5, 8, 13...) reprezentujícími relativní velikost nebo pracnost (např. Story Points). Pro každou odhadovanou položku (např. uživatelský scénář) všichni **současně ukáží kartu** se svým odhadem. Pokud jsou odhady podobné, použije se dohodnutá hodnota (např. průměr, medián). Pokud jsou odhady velmi rozdílné, následuje **diskuze** (zejména lidí s nejnižším a nejvyšším odhadem), proč si to myslí, a pak se hlasuje znovu. Opakuje se do dosažení konsenzu.
- **Výhody:** Rychlé, využívá hluboké znalosti expertů, nevyžaduje detailní historická data.
- **Nevýhody:** Subjektivní, závislé na kvalitě expertů, riziko zkreslení (bias), Wideband Delphi může být časově náročnější.

3.  **(Implicitně zmíněno u metrik) Extrapolace:**

- **Princip:** Používá se v průběhu projektu. Změří se skutečná pracnost na začátku projektu (např. v prvních iteracích) a na základě těchto dat se **předpovídá (extrapoluje)** budoucí pracnost pro zbytek projektu.
- **Příklad:** Po 3 sprintech víme, že průměrná pracnost testování na jeden Story Point je 2 hodiny. Pokud ve zbytku backlogu máme 100 Story Pointů, extrapolovaný odhad je 100 \* 2 = 200 hodin.
- **Výhody:** Využívá reálná data z běžícího projektu.
- **Nevýhody:** Vyžaduje, aby budoucí práce byla podobná té již provedené. Přesnost roste až v průběhu projektu.

4.  **(Implicitně zmíněno u expertízy) Tříbodový odhad (Three-Point Estimation):**

- **Princip:** Pro snížení nejistoty expert odhadne tři hodnoty pro daný úkol:
  - **a:** Optimistický odhad (nejlepší možný případ).
  - **m:** Nejpravděpodobnější odhad (reálný odhad).
  - **b:** Pesimistický odhad (nejhorší možný případ, vč. rizik).
- **Výpočet výsledného odhadu (E - Expected):** Často se používá vážený průměr (PERT): `E = (a + 4m + b) / 6`. Dává větší váhu nejpravděpodobnějšímu odhadu.
- **Výpočet směrodatné odchylky (SD - Standard Deviation):** Ukazuje míru nejistoty odhadu: `SD = (b - a) / 6`. Vyšší SD = vyšší nejistota.
- **Příklad:** a=6h, m=9h, b=18h. Výsledný odhad E = (6 + 4\*9 + 18) / 6 = (6 + 36 + 18) / 6 = 60 / 6 = **10 hodin**. Směrodatná odchylka SD = (18 - 6) / 6 = 12 / 6 = **2 hodiny**. Odhad je tedy 10 ± 2 hodiny (tj. pravděpodobně mezi 8 a 12 hodinami).
- **Výhody:** Zohledňuje nejistotu, poskytuje realističtější odhad než jediný bodový odhad.
- **Nevýhody:** Vyžaduje odhad tří hodnot, výpočet je trochu složitější.

**Důležité:** Odhady by se měly v průběhu projektu **pravidelně revidovat** a upravovat na základě nových informací a skutečné pracnosti.

**Shrnutí pro poznámky (Techniky odhadování):**

- **Účel odhadu:** Předpověď práce (člověkohodiny/dny) pro plánování, řízení, komunikaci.
- **Techniky:**
  1.  **Metriky:** Využití **historických dat** a poměrů z podobných projektů. Vyžaduje kvalitní data.
  2.  **Expertíza:** Využití **znalostí expertů**.
  - **Wideband Delphi:** Anonymní kola odhadů -> diskuze -> opakování do konsenzu.
  - **Planning Poker (Agile):** Současné ukázání karet (čísla/Story Points) -> diskuze při rozdílech -> opakování do konsenzu.
  3.  **Extrapolace:** Odhad budoucí práce na základě **dosavadních skutečných dat** z běžícího projektu.
  4.  **Tříbodový odhad:** Expert odhadne **Optimistický (a), Nejpravděpodobnější (m), Pesimistický (b)**. Výsledek `E = (a + 4m + b) / 6`, Nejistota `SD = (b - a) / 6`.
- **Revize:** Odhady pravidelně **revidovat** a upravovat.

Zvládl/a jsi vstřebat tyto techniky? Tříbodový odhad a plánovací poker/Delphi jsou K3, takže je potřeba je umět nejen popsat, ale i aplikovat. Zkusíme otázky?

## Kapitola 5.2: Management rizik

Management rizik je klíčovou součástí plánování a řízení testování. Pomáhá nám zaměřit úsilí tam, kde je to nejvíce potřeba.

**Lekce 16: Kapitola 5.2 - Management rizik (Úvod, Definice, Typy)**

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Identifikovat úroveň rizika pomocí pravděpodobnosti a dopadu (K1).
- Odlišit mezi projektovým a produktovým rizikem (K2).

**Vysvětlení:**

**Co je Management rizik?**

Je to systematický proces **identifikace, analýzy, plánování reakcí a monitorování rizik** spojených s projektem nebo produktem. Cílem není rizika zcela eliminovat (což často ani není možné), ale **porozumět jim a aktivně je řídit** tak, aby se maximalizovala pravděpodobnost dosažení cílů a minimalizovaly negativní dopady.

V kontextu testování nám management rizik pomáhá:

- **Zaměřit úsilí:** Rozhodnout, které části systému testovat důkladněji (ty rizikovější).
- **Prioritizovat testy:** Testovat nejdříve oblasti s nejvyššími riziky.
- **Vybrat vhodné techniky:** Použít robustnější techniky pro rizikovější oblasti.
- **Určit rozsah testování:** Rozhodnout, jak moc do hloubky testovat.
- **Plánovat zálohy:** Mít připravené scénáře, co dělat, když se riziko naplní.

**Přístup k testování založený na rizicích (Risk-based Testing):** Právě využití analýzy rizik pro řízení testovacích aktivit (co testovat, kdy, jak, jak moc) se nazývá risk-based testing.

**5.2.1 Definice rizika a jeho atributy**

- **Co je riziko?** Možná **negativní událost**, hrozba nebo situace, jejíž výskyt by měl nepříznivý dopad na dosažení cílů projektu nebo na kvalitu produktu.
- **Základní atributy rizika:** Každé riziko charakterizujeme dvěma hlavními faktory:
  1.  **Pravděpodobnost (Likelihood):** Jaká je šance (často vyjádřená slovně - např. Nízká, Střední, Vysoká - nebo procenty či škálou 0-1), že riziková událost **nastane**.
  2.  **Dopad (Impact):** Jak závažné by byly **následky**, kdyby riziková událost nastala (opět často slovně - Nízký, Střední, Vysoký, Kritický - nebo finančním vyjádřením škody apod.).
- **Úroveň rizika (Risk Level):** Kombinací pravděpodobnosti a dopadu určujeme celkovou **úroveň (míru) rizika**. Typicky se používá jednoduché pravidlo:
  - `Úroveň rizika = Pravděpodobnost * Dopad`
  - _Příklad:_ Pokud máme škálu 1-3 pro pravděpodobnost (1=Nízká, 3=Vysoká) a 1-3 pro dopad (1=Nízký, 3=Vysoký), riziko s P=3 a D=3 má úroveň 9 (Velmi vysoká), zatímco riziko s P=1 a D=1 má úroveň 1 (Velmi nízká). Někdy se používají i matice rizik pro vizualizaci.
- **Význam úrovně rizika:** Čím vyšší je úroveň rizika, tím větší pozornost bychom mu měli věnovat a tím silnější by měla být opatření pro jeho zmírnění.

**5.2.2 Projektová a produktová rizika**

Při testování rozlišujeme dva hlavní typy rizik:

1.  **Projektová rizika (Project Risks):**

- Týkají se **managementu a řízení samotného projektu**. Ohrožují **schopnost projektu dosáhnout svých cílů** (dodat včas, v rámci rozpočtu, v požadovaném rozsahu).
- Jsou to často "externí" faktory z pohledu testera, i když mohou testování silně ovlivnit.
- **Příklady:**
  - **Organizační:** Zpoždění v dodávkách (od vývoje, od třetích stran), nedostatek zdrojů (lidí, peněz), špatné odhady, změna priorit projektu.
  - **Lidské:** Nedostatek kvalifikovaných lidí, konflikty v týmu, špatná komunikace, nemoc klíčových osob.
  - **Technické:** Problémy s testovacím prostředím, špatná podpora nástrojů, změny technologie během projektu.
  - **Dodavatelské:** Selhání nebo zpoždění dodávky od externího dodavatele, jeho bankrot.
- **Dopad:** Primárně na harmonogram, rozpočet, zdroje a rozsah projektu.

2.  **Produktová rizika (Product Risks / Quality Risks):**

- Týkají se **kvality samotného produktu** (softwaru nebo systému). Ohrožují **schopnost produktu splnit očekávání a potřeby** uživatelů a zainteresovaných stran.
- Jsou to "vnitřní" rizika spojená s tím, co software dělá nebo nedělá. Právě na tato rizika se **testování zaměřuje především**.
- Souvisí s **kvalitativními charakteristikami** (dle ISO 25010, viz Kap. 2.2.2): funkční správnost, výkonnostní efektivita, kompatibilita, použitelnost, spolehlivost, bezpečnost (security), udržovatelnost, přenositelnost, bezpečnost (safety).
- **Příklady:**
  - Software neimplementuje požadovanou funkci správně (Funkční správnost).
  - Software je příliš pomalý při vysoké zátěži (Výkonnostní efektivita).
  - Software nefunguje správně v novém prohlížeči (Kompatibilita).
  - Uživatelé se v softwaru ztrácejí a nedokáží ho efektivně používat (Použitelnost).
  - Software často padá nebo zamrzá (Spolehlivost).
  - Neoprávněný uživatel může získat přístup k citlivým datům (Bezpečnost - security).
  - Oprava chyby v jedné části způsobí problémy jinde (Udržovatelnost).
  - Vstup citlivý na bezpečnost není správně validován (Bezpečnost - safety/security).
- **Dopad:** Primárně na spokojenost uživatelů, reputaci firmy, finanční ztráty, právní postihy, v extrémních případech i na zdraví nebo životy.

**Důležité:** Oba typy rizik se mohou navzájem ovlivňovat (např. projektové riziko "nedostatek času" může vést k produktovému riziku "nedostatečné otestování bezpečnosti"). Management testování musí brát v úvahu oba typy.

**Shrnutí pro poznámky (Úvod do Rizik, Typy):**

- **Management rizik:** Proces identifikace, analýzy, reakce a monitorování rizik.
- **Risk-based Testing:** Využití rizik pro řízení testování (co, kdy, jak, jak moc).
- **Riziko:** Možná negativní událost s nepříznivým dopadem.
- **Atributy:**
  - **Pravděpodobnost (Likelihood):** Šance, že nastane.
  - **Dopad (Impact):** Závažnost následků.
  - **Úroveň rizika = Pravděpodobnost \* Dopad** (vyšší úroveň = vyšší priorita).
- **Typy rizik:**
  - **Projektová:** Ohrožují **řízení projektu** (termíny, rozpočet, zdroje). Příklady: zpoždění, nedostatek lidí, problémy s prostředím, selhání dodavatele.
  - **Produktová (Kvality):** Ohrožují **kvalitu produktu**. Příklady: funkční chyby, nízký výkon, špatná použitelnost, nespolehlivost, bezpečnostní díry. **Na tato rizika se testování primárně zaměřuje.**

Skvěle!

**Lekce 17: Kapitola 5.2.3 - Jak analýza produktových rizik ovlivňuje hloubku a rozsah testování & Kapitola 5.2.4 - Opatření v reakci na produktová rizika**

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Vysvětlit, jak může analýza produktových rizik ovlivnit hloubku a rozsah testování (K2).
- Vysvětlit, jaká opatření lze přijmout v reakci na analyzovaná produktová rizika (K2).

**Vysvětlení:**

Když jsme identifikovali a ohodnotili produktová rizika (určili jejich pravděpodobnost a dopad => úroveň rizika), tyto informace nám slouží jako **klíčový vstup pro plánování testování**. Cílem je **zaměřit naše omezené testovací zdroje** (čas, lidi, peníze) tam, kde je to nejvíce potřeba – na oblasti s nejvyššími riziky. Tomu se říká **Risk-based Testing (testování založené na rizicích)**.

**5.2.3 Jak analýza produktových rizik ovlivňuje hloubku a rozsah testování**

Analýza produktových rizik přímo ovlivňuje rozhodnutí o tom:

1.  **Co testovat (Rozsah):**

    - **Prioritizace funkcí/oblastí:** Funkce nebo části systému s vyšší úrovní rizika budou mít vyšší prioritu pro testování a budou testovány důkladněji. Naopak, funkce s velmi nízkým rizikem mohou být testovány méně, nebo v extrémních případech (při nedostatku zdrojů) vůbec.
    - **Výběr úrovní a typů testů:** Pro rizikovější oblasti můžeme zvolit více úrovní testování (např. nejen systémové, ale i důkladné integrační) nebo více typů testů (např. pro rizikovou funkci související s výkonem naplánujeme specifické výkonnostní testy).

2.  **Jak důkladně testovat (Hloubka/Podrobnost):**

    - **Výběr testovacích technik:** Pro vysoce rizikové oblasti můžeme použít formálnější a robustnější testovací techniky (např. Rozhodovací tabulky, Testování přechodů stavů), zatímco pro méně rizikové můžeme použít jednodušší techniky (např. EP, BVA, nebo se více spolehnout na experience-based).
    - **Definice kritérií pokrytí:** Pro rizikovější kód můžeme stanovit přísnější kritéria pokrytí (např. 100% pokrytí větví vs. 80% pokrytí příkazů pro méně kritický kód). Pro rizikovější funkční oblasti můžeme požadovat pokrytí všech identifikovaných pravidel v rozhodovací tabulce.
    - **Množství a detailnost testovacích případů:** Pro oblasti s vyšším rizikem budeme pravděpodobně navrhovat více testovacích případů a ty budou detailnější, pokrývající více scénářů (včetně negativních a okrajových).
    - **Potřeba dat:** Pro rizikovější scénáře můžeme potřebovat komplexnější a realističtější testovací data.

3.  **Kdy testovat:**

    - Rizikovější oblasti by se měly testovat **co nejdříve** (shift-left), aby se potenciální problémy odhalily včas.

4.  **Kým testovat:**
    - Na testování vysoce rizikových oblastí můžeme nasadit **zkušenější testery** nebo testery se specifickými dovednostmi. Může být také vyžadována vyšší úroveň **nezávislosti testování**.

**Příklad:** Pokud identifikujeme, že platební modul v e-shopu má velmi vysoké produktové riziko (vysoká pravděpodobnost chyby a kritický dopad – ztráta peněz, reputace), budeme ho testovat velmi důkladně. Použijeme detailní techniky (rozhodovací tabulky pro různé typy plateb a slev, BVA pro částky), naplánujeme více negativních testů, zajistíme pokrytí všech hlavních scénářů, a možná i specifické bezpečnostní a výkonnostní testy. Testování začne brzy a budou ho provádět zkušení testeři. Naopak, testování informační stránky "O nás" bude mít pravděpodobně mnohem nižší prioritu a hloubku.

**5.2.4 Opatření v reakci na produktová rizika (Risk Treatment / Risk Mitigation)**

Když jsme rizika identifikovali a ohodnotili, musíme se rozhodnout, co s nimi uděláme. Pro každé riziko můžeme zvolit jednu z následujících strategií reakce (někdy i kombinaci):

1.  **Zmírnění rizika (Risk Mitigation):**

    - **Co to je:** Podniknutí kroků ke **snížení pravděpodobnosti** výskytu rizika nebo **snížení jeho dopadu**, pokud nastane.
    - **Jak (v kontextu testování):** Právě **testování** je primárním způsobem zmírňování produktových rizik! Tím, že navrhneme a provedeme testy zaměřené na rizikové oblasti, snažíme se odhalit a umožnit opravu defektů, které by mohly vést k naplnění rizika.
    - **Konkrétní testovací opatření (jak už bylo naznačeno výše):**
      - Přidělení **zkušenějších testerů** na rizikové oblasti.
      - Zvýšení **nezávislosti testování** (např. dedikovaný tým).
      - Provedení **revizí a statické analýzy** požadavků a kódu.
      - Použití **robustnějších testovacích technik** a dosažení **vyššího pokrytí**.
      - Implementace **specifických typů testů** (výkonnostní, bezpečnostní...).
      - **Dynamické testování** s větším důrazem na dané riziko.
      - Častější testování.

2.  **Přenesení rizika (Risk Transfer / Risk Sharing):**

    - **Co to je:** Přesunutí části nebo celého dopadu rizika na třetí stranu.
    - **Příklad:** Pojištění proti ztrátě dat, outsourcing specializovaného testování (např. penetrační testy) na firmu, která na sebe vezme odpovědnost za kvalitu provedení.

3.  **Vyhnutí se riziku (Risk Avoidance):**

    - **Co to je:** Eliminace aktivity nebo podmínky, která riziko způsobuje.
    - **Příklad:** Pokud je implementace určité funkce příliš riziková a není absolutně kritická, může se management rozhodnout tuto funkci z produktu zcela **odstranit** nebo odložit.

4.  **Akceptace rizika (Risk Acceptance / Risk Retention):**

    - **Co to je:** Vědomé rozhodnutí nedělat nic aktivního pro zmírnění rizika (nebo náklady na zmírnění jsou vyšší než potenciální dopad).
    - **Příklad:** Pro funkci s velmi nízkou pravděpodobností chyby a zanedbatelným dopadem se může tým rozhodnout provést jen minimální testování nebo riziko akceptovat bez dalších testů (např. pokud na důkladné testování nejsou zdroje). Riziko by mělo být zdokumentováno.

5.  **Záložní plán (Contingency Plan):**
    - **Co to je:** Připravený plán akcí pro případ, že se riziko naplní (nastane problém), aby se minimalizoval dopad.
    - **Příklad:** Mít připravený postup pro rychlé vrácení k předchozí stabilní verzi softwaru (rollback), pokud nové nasazení způsobí kritické problémy. Mít definovaný komunikační plán pro zákazníky v případě výpadku.

Výběr strategie závisí na úrovni rizika, nákladech na opatření a celkových cílech projektu.

**Shrnutí pro poznámky (Analýza rizik & Opatření):**

- **Vliv analýzy rizik na testování (Risk-based Testing):**
  - **Prioritizuje** oblasti/funkce k testování.
  - Ovlivňuje **hloubku a důkladnost** testování (výběr technik, pokrytí, množství testů).
  - Pomáhá rozhodnout o **načasování** testů (rizikové dříve).
  - Pomáhá přiřadit **zkušenější testery** na rizikové oblasti.
- **Opatření v reakci na produktová rizika:**
  - **Zmírnění (Mitigation):** Snížení P nebo D. **Primární reakce pomocí TESTOVÁNÍ** (více/lepší testy, zkušenější lidé, vyšší pokrytí...).
  - **Přenesení (Transfer):** Přenést dopad na třetí stranu (pojištění, outsourcing).
  - **Vyhnutí (Avoidance):** Odstranit příčinu rizika (např. neimplementovat rizikovou funkci).
  - **Akceptace (Acceptance):** Vědomě nedělat nic (pokud je riziko malé nebo náklady na zmírnění vysoké). Zdokumentovat!
  - **Záložní plán (Contingency):** Co dělat, když se riziko naplní (minimalizace následků).

Zvládl/a jsi tento blok o vlivu rizik na testování a možnostech reakce? Připraven/a na otázky?

Perfektní! Pojďme se podívat na to, jak se testování sleduje, řídí a uzavírá.

**Lekce 18: Kapitola 5.3 - Monitoring, řízení a dokončení testování**

**Cíl:** Po této lekci bys měl/a být schopen/a:

- Vybavit si metriky využívané při testování (K1).
- Shrnout účel a obsah reportů z testování a uvědomit si, pro koho jsou určeny (K2).
- Ilustrovat na příkladech komunikaci stavu testování (K2).

**Vysvětlení:**

**Co je Monitoring testování?**

- Je to **průběžná aktivita shromažďování dat a informací** o testovacích činnostech.
- **Cíl:** Sledovat aktuální stav testování, porovnávat ho s plánem (např. plánem testování, harmonogramem) a identifikovat případné odchylky nebo problémy.
- **Co se monitoruje?** Například:
  - Postup oproti harmonogramu.
  - Využití zdrojů (lidí, prostředí).
  - Stav defektů (nalezené, opravené, otevřené).
  - Dosažené pokrytí (požadavků, kódu, rizik).
  - Stav plnění vstupních/výstupních kritérií.
  - Blokátory a problémy.

**Co je Řízení testování (Test Control)?**

- Je to aktivita, která **využívá informace z monitoringu** k tomu, aby se **přijímala nápravná opatření**, pokud testování nejde podle plánu nebo pokud se objeví nové skutečnosti.
- **Cíl:** Udržet testování na správné cestě k dosažení jeho cílů. Je to reaktivní i proaktivní činnost.
- **Příklady řídicích akcí:**
  - **Přehodnocení priorit testů:** Pokud se objeví nové kritické riziko nebo se zpozdí dodávka klíčové funkce.
  - **Změna testovací strategie/přístupu:** Pokud se ukáže, že původní přístup není efektivní.
  - **Přidělení více zdrojů:** Pokud je testování ve skluzu.
  - **Úprava harmonogramu:** Pokud jsou objektivní důvody pro zpoždění.
  - **Revize vstupních/výstupních kritérií:** V případě zásadních změn v projektu (ale opatrně, viz dříve).
  - **Eskalace problémů:** Pokud tým nemůže problém vyřešit sám (např. nestabilní prostředí, které musí opravit jiný tým).

**Co jsou Činnosti dokončení testování (Test Completion Activities)?**

- Jsou to aktivity, které se provádějí, když se testovací fáze (např. úroveň testování, iterace, celý projekt) chýlí ke konci nebo je formálně ukončena (např. splněním výstupních kritérií).
- **Cíl:** Formálně uzavřít testovací aktivity, shromáždit zkušenosti, archivovat testware a připravit finální reporty.
- **Příklady činností dokončení:**
  - **Kontrola splnění výstupních kritérií:** Ověření, že všechny definované podmínky byly splněny.
  - **Shromažďování a archivace testwaru:** Uložení testovacích plánů, případů, skriptů, dat, výsledků, reportů pro budoucí použití (např. regresní testy, audit).
  - **Předání testwaru údržbovému týmu:** Pokud bude produkt dále udržován.
  - **Získání zpětné vazby a ponaučení (Lessons Learned):** Analýza toho, co šlo dobře a co špatně, s cílem zlepšit testovací proces v budoucnu. Často formou retrospektivy.
  - **Vytvoření souhrnného reportu z testování (Test Summary Report):** Viz níže.

**5.3.1 Metriky používané při testování**

- **Co jsou metriky:** Kvantitativní (číselné) nebo kvalitativní (popisné) míry, které pomáhají sledovat a hodnotit různé aspekty testovacího procesu a produktu. Jsou klíčové pro monitoring a řízení.
- **Typy metrik (příklady):**
  - **Metriky postupu projektu/iterace:**
    - Dokončení úkolů (např. % dokončených testovacích případů z plánu).
    - Využití zdrojů (např. skutečná vs. plánovaná pracnost).
    - Náklady na testování.
  - **Metriky postupu testování:**
    - Počet navržených/provedených/automatizovaných testovacích případů.
    - Doba trvání testovacího cyklu.
    - Počet testů, které prošly / selhaly / byly zablokovány.
  - **Metriky kvality produktu:**
    - Počet nalezených defektů (celkem, dle závažnosti, dle modulu).
    - Hustota defektů (Defect Density - např. počet defektů na 1000 řádků kódu nebo na funkční bod).
    - Procento zjištěných defektů (Defect Detection Percentage - DDP - poměr defektů nalezených v dané fázi k celkovému počtu defektů nalezených ve všech fázích, včetně produkce).
    - Míra selhání (Failure Rate), Střední doba mezi poruchami (MTBF - Mean Time Between Failures).
    - Stav otevřených defektů.
  - **Metriky pokrytí:**
    - Pokrytí požadavků testy.
    - Pokrytí kódu (příkazy, větve).
    - Pokrytí rizik.
  - **Metriky efektivity testování:**
    - Průměrný čas na nalezení/opravu defektu.
    - Náklady na nalezení defektu.

Výběr metrik závisí na cílech testování, potřebách projektu a dostupnosti dat. Nemá smysl sbírat metriky, které nikdo nepoužívá.

**5.3.2 Účel, obsah a cílové skupiny reportů z testování**

- **Účel reportování:** **Komunikovat** informace o postupu, stavu a výsledcích testování různým zainteresovaným stranám. Reporty jsou klíčovým výstupem z monitoringu a dokončovacích aktivit.
- **Typy reportů:**
  - **Report o postupu prací při testování (Test Progress Report / Test Status Report):**
    - **Účel:** Poskytuje pravidelné (např. denní, týdenní) informace o aktuálním stavu testovacích aktivit během provádění testů.
    - **Obsah:**
      - Testovací období, kterého se report týká.
      - Postup oproti plánu (např. počet provedených testů, nalezené defekty).
      - Nové nebo změněné metriky.
      - Překážky a blokátory a jejich řešení.
      - Nová nebo změněná rizika.
      - Plán testování na následující období.
    - **Cílová skupina:** Testovací tým, manažer testů, projektový manažer, někdy i vývojáři.
  - **Souhrnný report z testování (Test Summary Report / Test Completion Report):**
    - **Účel:** Poskytuje celkové shrnutí a vyhodnocení testovacích aktivit po dokončení určité testovací fáze (úrovně, iterace, projektu).
    - **Obsah:**
      - Shrnutí provedených testů.
      - Vyhodnocení oproti původnímu plánu (cíle, výstupní kritéria).
      - Odchylky od plánu (harmonogram, pracnost, rozsah).
      - Překážky, které se vyskytly, a jak byly řešeny.
      - Souhrnné metriky (pokrytí, stav defektů, kvalita produktu).
      - Neošetřená rizika.
      - Nevyřešené defekty.
      - Ponaučení (Lessons Learned).
      - Doporučení pro další kroky (např. zda je produkt připraven k nasazení).
    - **Cílová skupina:** Management projektu, zákazník, produktový vlastník, další zainteresované strany, které potřebují rozhodnout o dalším osudu produktu.

**Důležité:** Forma a detailnost reportů se liší podle cílové skupiny. Management bude zajímat obecnější přehled a klíčové metriky, zatímco testovací tým může potřebovat detailnější informace.

**5.3.3 Komunikování stavu testování**

- Efektivní komunikace stavu testování je klíčová pro úspěch projektu.
- **Způsoby komunikace:**
  - **Formální reporty:** (viz výše) Progress a Summary reports.
  - **Dashboardy:** Grafické přehledy klíčových metrik (např. v CI/CD nástrojích, test management nástrojích, projektových nástrojích jako Jira). Mohou zobrazovat grafy burn-down (zbývající práce), trendy defektů, pokrytí atd. Jsou dobré pro rychlý přehled.
  - **Pravidelné schůzky:** Denní stand-upy (agile), týdenní status meetingy.
  - **Neformální komunikace:** E-maily, chaty, osobní rozhovory (zejména v rámci týmu).
  - **Online dokumentace:** Wiki, sdílené dokumenty.
- **Přizpůsobení cílové skupině:** Různé skupiny potřebují různé informace a jinou úroveň detailu. Je důležité komunikovat relevantní informace srozumitelnou formou.

**Shrnutí pro poznámky (Monitoring, Řízení, Dokončení, Reporty):**

- **Monitoring:** **Průběžné sledování** testovacích aktivit a porovnávání s plánem.
- **Řízení (Control):** **Přijímání nápravných opatření** na základě monitoringu.
- **Dokončení:** Formální uzavření fáze (kontrola kritérií, archivace, lessons learned, souhrnný report).
- **Metriky:** Kvantitativní/kvalitativní míry (postup projektu/testování, kvalita produktu, pokrytí, efektivita).
- **Reporty:**
  - **Progress Report (Stavový):** Pravidelně, aktuální stav, postup, blokátory, plán. Pro tým, PM.
  - **Summary Report (Souhrnný):** Po dokončení fáze, celkové vyhodnocení, metriky, ponaučení, doporučení. Pro management, zákazníka.
- **Komunikace stavu:** Formální reporty, Dashboardy, Schůzky, Neformální. **Přizpůsobit cílové skupině.**

Uf, to bylo hodně informací o řízení! Jsi připraven/a na otázky k tomuto bloku?
