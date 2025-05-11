**Opakovací otázky – Kapitola 5: Management testování (20 otázek)**

1.  Který dokument typicky definuje celkovou strategii testování, zdroje, harmonogram a výstupní kritéria pro daný projekt?
    a) Report o defektu
    b) Testovací případ
    c) Plán testování
    d) Test Charter

2.  Tým odhaduje pracnost testování nového modulu. Každý člen týmu má sadu karet s čísly a po diskuzi současně ukáže kartu se svým odhadem. Pokud jsou odhady rozdílné, následuje další diskuze a hlasování. Jaká technika odhadování je zde popsána?
    a) Tříbodový odhad
    b) Wideband Delphi
    c) Metriky založené na historických datech
    d) Plánovací poker

3.  Riziko, že klíčový dodavatel testovacího nástroje ukončí jeho podporu, je příkladem:
    a) Produktového rizika
    b) Projektového rizika
    c) Rizika spojeného s pokrytím kódu
    d) Akceptačního rizika

4.  Co je hlavním cílem **Řízení testování (Test Control)**?
    a) Pouze shromažďovat data o postupu testování
    b) Přijímat nápravná opatření na základě informací z monitoringu, aby se dosáhlo cílů testování
    c) Definovat, které testovací případy budou automatizovány
    d) Archivovat veškerý testware po dokončení projektu

5.  Která z následujících položek je **NEZBYTNÁ** pro kvalitní report o defektu, aby vývojář mohl problém efektivně řešit?
    a) Návrh testera na konkrétní opravu v kódu
    b) Podrobný popis kroků k reprodukci defektu
    c) Osobní názor testera na kvalitu celého modulu
    d) Seznam všech ostatních defektů nalezených ve stejný den

6.  Pokud testovací tým dosáhne 90% pokrytí požadavků testy, ale výstupní kritérium bylo stanoveno na 95%, co by měl manažer testů typicky udělat?
    a) Okamžitě ukončit testování a prohlásit produkt za připravený
    b) Změnit výstupní kritérium na 90%, aby bylo splněno
    c) Analyzovat důvody nesplnění, diskutovat rizika s managementem a navrhnout další kroky (např. další testování, akceptace rizika)
    d) Ignorovat výstupní kritérium, protože je nereálné

7.  Proč je důležité sledovat verzi testovaného objektu a verzi testwaru pomocí konfiguračního managementu?
    a) Aby se zajistilo, že se vždy používá nejstarší stabilní verze
    b) Pro zajištění reprodukovatelnosti testů a správnosti testování vzhledem ke konkrétní verzi
    c) Aby se zjednodušilo reportování defektů
    d) Primárně pro účely fakturace zákazníkovi

8.  Manažer testů připravuje odhad pro testování. Optimistický odhad (a) je 10 člověkodnů, nejpravděpodobnější (m) je 15 člověkodnů a pesimistický (b) je 26 člověkodnů. Jaký je očekávaný odhad (E) pomocí PERT vzorce `E = (a + 4m + b) / 6`?
    a) 15 člověkodnů
    b) 17 člověkodnů
    c) 16 člověkodnů
    d) 18 člověkodnů

9.  Která z následujících metrik nejlépe popisuje kvalitu samotného softwarového produktu?
    a) Počet provedených testovacích případů za den
    b) Procento automatizovaných testů
    c) Hustota defektů (např. počet defektů na KLOC)
    d) Čas strávený plánováním testování

10. Tým identifikoval produktové riziko: "Systém může nesprávně vypočítat složené úročení u VIP klientů, což může vést k finančním ztrátám a poškození reputace." Jaká testovací aktivita by byla vhodným **zmírněním (mitigací)** tohoto rizika?
    a) Ignorovat toto riziko, protože VIP klientů je málo
    b) Detailní testování výpočtu úročení s různými scénáři a hraničními hodnotami, zaměřené na VIP klienty
    c) Přenést odpovědnost za správnost výpočtů na finanční oddělení
    d) Zcela odstranit funkci složeného úročení ze systému

11. Co je typickým příkladem **vstupního kritéria (Entry Criteria)** pro zahájení systémového integračního testování?
    a) Všechny plánované testy byly úspěšně provedeny
    b) Komponenty, které mají být integrovány, prošly úspěšně komponentovým testováním
    c) Souhrnný report z testování byl schválen zákazníkem
    d) Všechny nalezené defekty byly označeny jako "Odložené"

12. Jaký typ reportu by tester měl připravit na konci celého projektu, aby shrnul veškeré testovací aktivity, výsledky, metriky a ponaučení?
    a) Denní report o postupu prací
    b) Plán testování
    c) Souhrnný report z testování (Test Summary Report)
    d) Report o defektu pro každý nenalezený defekt

13. Priorita defektu je typicky určována na základě:
    a) Technické složitosti opravy defektu
    b) Dopadu defektu na byznys a naléhavosti jeho opravy
    c) Počtu řádků kódu ovlivněných defektem
    d) Zkušeností testera, který defekt nahlásil

14. Během monitoringu testování zjistíte, že počet nalezených kritických defektů je výrazně vyšší, než se očekávalo, a testování je blokováno. Co je vhodnou **řídicí akcí (Test Control)**?
    a) Pokračovat v testování podle původního plánu a doufat, že se situace zlepší
    b) Snížit závažnost hlášených defektů, aby metriky vypadaly lépe
    c) Zastavit testování, analyzovat příčiny, eskalovat problém a navrhnout nápravná opatření (např. stabilizace buildu, revize kódu)
    d) Ihned začít s aktivitami dokončení testování

15. Co z následujícího NENÍ typickým cílem konfiguračního managementu v testování?
    a) Zajistit, že je testována správná verze softwaru
    b) Umožnit reprodukovatelnost testů
    c) Sledovat verze testovacích plánů a případů
    d) Přímo odhadovat pracnost testovacích aktivit

16. Váš tým po dokončení prvních 3 sprintů zjistil, že průměrně připraví a provede testy pro jeden Story Point za 4 hodiny. Pro zbývajících 50 Story Pointů v backlogu tedy odhadujete pracnost 200 hodin. Jakou techniku odhadování jste primárně použili?
    a) Metriky založené na historických datech z jiných projektů
    b) Wideband Delphi
    c) Extrapolace na základě dat z běžícího projektu
    d) Tříbodový odhad

17. Definice "Míra, do jaké jsou splněny explicitní a implicitní potřeby zákazníků a uživatelů" nejlépe popisuje:
    a) Testovací strategii
    b) Softwarovou kvalitu
    c) Pokrytí testů
    d) Životní cyklus defektu

18. Která informace o defektu je klíčová pro určení jeho **závažnosti (Severity)**?
    a) Jak rychle musí být defekt opraven z pohledu byznysu
    b) Jaký je technický dopad defektu na funkčnost nebo stabilitu systému
    c) Kolik času zabere vývojáři oprava defektu
    d) Který tester defekt nahlásil

19. Pokud se management rozhodne vydat produkt i přes to, že nebyly splněny všechny definované výstupní kritéria (např. stále existují známé defekty střední priority), jaká strategie reakce na riziko je zde primárně uplatněna?
    a) Vyhnutí se riziku
    b) Zmírnění rizika
    c) Přenesení rizika
    d) Akceptace rizika

20. "Baseline" v konfiguračním managementu slouží jako:
    a) Seznam všech testerů zapojených do projektu
    b) Referenční bod (formálně schválená sada položek), od kterého se sledují další změny
    c) Nejnižší možná úroveň kvality, kterou je produkt povinen splnit
    d) Automatický nástroj pro generování testovacích dat

Přeji hodně štěstí! Jsem zvědavý, jak si s touto komplexní sadou poradíš.
