Rozumím, metriky mohou být někdy trochu matoucí, pojďme si je projít ještě jednou "polopatě" s důrazem na jejich účel a typy, které zmiňuje sylabus.

Představ si, že jsi manažer testovacího týmu (nebo i člen týmu) a potřebuješ vědět, **jak si vedete** a **jak kvalitní je to, co testujete**. Metriky jsou jako **palubní deska v autě** – dávají ti důležité informace, abys mohl/a dobře řídit.

## Proč vůbec metriky potřebujeme?

- **Abychom věděli, kde jsme:** Jsme v plánu? Kolik práce je hotovo?
- **Abychom věděli, kam jdeme:** Blížíme se cíli? Bude produkt dost kvalitní?
- **Abychom mohli dělat rozhodnutí:** Máme přidat lidi? Máme testování zastavit? Můžeme produkt vydat?
- **Abychom se mohli zlepšovat:** Co jsme minule udělali dobře a co špatně?

## Základní dělení metrik (jak je sylabus naznačuje):

Budeme se bavit o několika kategoriích, které ti pomohou sledovat různé aspekty.

### 1. Metriky POSTUPU PROJEKTU/ITERACE (Jak nám jde práce na projektu celkově?)

Tyto metriky ti říkají, jestli stíháte termíny, jestli máte dost lidí a peněz, a jestli jsou úkoly hotové.

- **Příklad "polopatě":** Jste parta, co staví dům.
  - **Dokončení úkolů:** "Kolik procent cihel už máme položených z celkového plánu?" (Např. % dokončených testovacích případů z plánu).
  - **Využití zdrojů:** "Kolik hodin jsme na stavbě strávili tento týden oproti plánu? Máme ještě dost peněz na materiál?" (Např. skutečná vs. plánovaná pracnost testerů, náklady na testování).
  - **Náklady na testování:** "Kolik nás stálo ověření, že okna těsní?"

### 2. Metriky POSTUPU TESTOVÁNÍ (Jak nám jde samotné testování?)

Tyto metriky se zaměřují konkrétně na testovací aktivity.

- **Příklad "polopatě":** Stále stavíte dům a teď se soustředíte na kontrolu kvality (testování).
  - **Počet navržených/provedených/automatizovaných testů:** "Kolik různých způsobů kontroly oken jsme vymysleli? Kolik z nich už jsme provedli? Kolik kontrol dělá robot (automat)?"
  - **Doba trvání testovacího cyklu:** "Jak dlouho nám trvalo, než jsme zkontrolovali všechna okna v jednom patře?"
  - **Počet testů, které prošly / selhaly / byly zablokovány:** "Kolik oken bylo v pořádku? Kolik jich netěsnilo (selhání)? Kolik oken jsme nemohli zkontrolovat, protože ještě nebyla osazená (zablokováno)?"

### 3. Metriky KVALITY PRODUKTU (Jak dobrý je ten náš dům/software?)

Toto je klíčové! Tyto metriky přímo vypovídají o tom, jak kvalitní je to, co jste vytvořili.

- **Příklad "polopatě":** Dům je (téměř) hotový.
  - **Počet nalezených defektů:** "Kolik netěsných oken, křivých zdí nebo kapajících kohoutků jsme našli?" (Může se dělit podle závažnosti – "trochu kape" vs. "teče proudem").
  - **Hustota defektů (Defect Density):** "Našli jsme průměrně 2 chyby na každou místnost." (Nebo počet chyb na 1000 řádků kódu, na funkční bod). Pomáhá porovnávat kvalitu různých částí nebo projektů.
  - **Procento zjištěných defektů (Defect Detection Percentage - DDP):** "Při kolaudaci (fáze testování) jsme našli 8 netěsných oken. Po nastěhování (produkce) našli majitelé ještě 2 další. Takže naše DDP při kolaudaci bylo 8/(8+2) = 80 %." (Jak jsme byli dobří v hledání chyb _v té konkrétní fázi_).
  - **Míra selhání (Failure Rate), Střední doba mezi poruchami (MTBF):** "V průměru nám každý třetí den přestane fungovat topení." (Jak často systém selhává v provozu).
  - **Stav otevřených defektů:** "Kolik kapajících kohoutků ještě čeká na opravu?"

### 4. Metriky POKRYTÍ (Co všechno jsme vlastně otestovali?)

Tyto metriky ukazují, jakou část systému nebo požadavků jsme našimi testy "prošlápli".

- **Příklad "polopatě":** Kontrola elektroinstalace v domě.
  - **Pokrytí požadavků testy:** "Naším cílem bylo zkontrolovat, že v každé místnosti funguje světlo a alespoň dvě zásuvky. Podařilo se nám to ověřit ve všech místnostech?" (Např. % požadavků, pro které existuje a prošel test).
  - **Pokrytí kódu (příkazy, větve):** "Prošli naši elektrikáři (testy) každý jednotlivý drát (příkaz) v rozvaděči? Zkontrolovali, co se stane, když zapnou každý jistič (větev)?"
  - **Pokrytí rizik:** "Identifikovali jsme riziko požáru od špatné elektroinstalace. Máme testy, které ověřují, že jsou použity správné materiály a pojistky, abychom toto riziko snížili?"

### 5. Metriky EFEKTIVITY TESTOVÁNÍ (Jak dobře a rychle pracujeme jako testeři?)

Tyto metriky pomáhají zhodnotit, jak efektivní je náš testovací proces.

- **Příklad "polopatě":** Opravy chyb v domě.
  - **Průměrný čas na nalezení/opravu defektu:** "Jak dlouho nám průměrně trvá, než najdeme příčinu kapajícího kohoutku a jak dlouho trvá instalatérovi ho opravit?"
  - **Náklady na nalezení defektu:** "Kolik nás stálo (čas lidí, nástroje) najít jedno netěsnící okno?"

## Důležité "polopatě" pravidlo:

- **Nesbírej metriky jen pro to, abys je měl.** Každá metrika by ti měla pomoci něco pochopit nebo o něčem rozhodnout. Pokud nevíš, k čemu ti metrika je, je zbytečná.
- **Kontext je král.** Metrika sama o sobě nemusí nic znamenat. "10 nalezených chyb" – je to hodně nebo málo? Záleží na velikosti a složitosti systému, fázi testování atd. Metriky je potřeba interpretovat v kontextu.
- **Trendy jsou často důležitější než absolutní čísla.** "Počet otevřených chyb roste každý týden" je varovnější signál než jen informace "Máme 50 otevřených chyb".

Doufám, že toto "polopaté" vysvětlení s příklady bylo srozumitelnější a pomohlo ti lépe si utřídit různé typy metrik a jejich účel.

Je to teď jasnější? Chceš se k některé kategorii ještě vrátit nebo se na něco doptat?
