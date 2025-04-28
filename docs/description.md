# Příprava na certifikaci ISTQB CTFL 4.0

---

## Analýza důležitosti témat a plán přípravy

Než se pustíme do samotné látky, provedl/a jsem analýzu struktury zkoušky ISTQB CTFL 4.0, abychom mohli naši přípravu zacílit co nejefektivněji. Zkouška se skládá ze 40 otázek a různé kapitoly sylabu mají u zkoušky různou váhu, co se týče počtu otázek a jejich náročnosti (tzv. K-úrovně: K1 - zapamatovat si, K2 - porozumět, K3 - použít).

### Rozložení otázek dle kapitol:

- **Základy testování**: ~8 otázek (K1, K2)
- **Testování v průběhu životního cyklu vývoje softwaru**: ~7 otázek (K1, K2)
- **Statické testování**: ~4 otázky (K1, K2)
- **Testovací analýza a návrh testů**: ~12 otázek (K1, K2, K3)
- **Management testování**: ~7 otázek (K1, K2, K3)
- **Testovací nástroje**: ~2 otázky (K1, K2)

### Závěr:

Jednoznačně největší důraz klade zkouška na **Kapitolu 4: Testovací analýza a návrh testů**. Obsahuje nejvíce otázek (téměř třetinu zkoušky) a zahrnuje otázky na úrovni K3, které vyžadují praktickou aplikaci naučených technik. Hned za ní následuje **Kapitola 5**, která také obsahuje K3 otázky.

Navrhuji tedy začít naši přípravu právě **Kapitolou 4: Testovací analýza a návrh testů**.

---

## Lekce 1: Kapitola 4.1 - Přehled technik testování

### Cíl:

Po této lekci bys měl/a být schopen/a rozlišit mezi třemi hlavními kategoriemi testovacích technik:

- **Techniky černé skříňky**
- **Techniky bílé skříňky**
- **Techniky založené na zkušenostech** (K2)

---

### Vysvětlení:

Představ si, že máš otestovat nějaký software. Můžeš k tomu přistupovat různě. Buď budeš zkoušet náhodně, co tě napadne, nebo použiješ nějaký systematický přístup. A právě k tomu slouží testovací techniky. Jsou to postupy nebo metody, které nám pomáhají:

- Systematicky vybrat, co testovat.
- Rozhodnout, jaké testovací případy navrhnout.
- Zajistit, že jsme pokryli důležité aspekty testovaného softwaru.
- Zefektivnit testování a najít více chyb s menším úsilím.

Existuje mnoho různých technik, ale pro začátek je dělíme do tří hlavních kategorií:

#### 1. Techniky černé skříňky (Black-Box Techniques)

- **Co to je**: Nezajímá nás, jak software funguje uvnitř. Díváme se na něj jako na "černou skříňku" – vidíme jen vstupy a výstupy.
- **Na základě čeho testujeme**: Požadavky, specifikace nebo jiný popis toho, co má software dělat.
- **Cíl**: Ověřit, zda se software chová podle specifikace.
- **Příklady technik**: Rozdělení tříd ekvivalence (EP), Analýza hraničních hodnot (BVA), Testování pomocí rozhodovací tabulky, Testování přechodů stavů.
- **Analogie**: Testuješ kávovar. Víš, že když vhodíš minci a zmáčkneš tlačítko "Espresso", má vypadnout kelímek s espressem. Nezajímá tě, jaké procesy probíhají uvnitř.

#### 2. Techniky bílé skříňky (White-Box Techniques)

- **Co to je**: Známe vnitřní strukturu softwaru – vidíme "dovnitř".
- **Na základě čeho testujeme**: Analýza kódu nebo vnitřní struktury.
- **Cíl**: Ověřit, zda vnitřní struktura funguje správně, a změřit, jak důkladně jsme kód otestovali.
- **Příklady technik**: Testování příkazů (Statement testing), Testování větví (Branch testing).
- **Analogie**: Jsi elektrikář a kontroluješ elektroinstalaci v domě. Nestačí ti jen zapnout světlo, musíš se podívat na samotné dráty, spoje a jističe.

#### 3. Techniky založené na zkušenostech (Experience-Based Techniques)

- **Co to je**: Využívají znalosti, zkušenosti a intuici testerů, vývojářů, uživatelů a dalších zainteresovaných stran.
- **Na základě čeho testujeme**: Předchozí zkušenosti s podobnými systémy, znalosti o typických chybách, selský rozum.
- **Cíl**: Najít defekty, které by formálnější techniky mohly minout.
- **Příklady technik**: Odhadování chyb (Error guessing), Průzkumné testování (Exploratory testing), Testování založené na kontrolních seznamech (Checklist-based testing).
- **Analogie**: Zkušený automechanik slyší podezřelý zvuk motoru a díky svým zkušenostem hned tuší, na kterou součástku se má zaměřit.

---

### Důležité:

Tyto kategorie se nevylučují! V praxi se techniky často kombinují, aby bylo testování co nejefektivnější a pokrylo software z různých úhlů pohledu.

---

## Kontrolní otázky (Lekce 1):

1. Která z následujících kategorií testovacích technik se primárně zaměřuje na ověření funkčnosti softwaru na základě jeho specifikací, aniž by brala v úvahu vnitřní strukturu kódu?

- a) Techniky bílé skříňky
- b) Techniky založené na zkušenostech
- c) Techniky černé skříňky
- d) Techniky statické analýzy

2. Tester analyzuje zdrojový kód modulu, aby navrhl testovací případy, které zajistí, že všechny podmíněné skoky (IF-THEN-ELSE) budou provedeny jak pro pravdivou (TRUE), tak pro nepravdivou (FALSE) větev. Jakou kategorii technik tester primárně používá?

- a) Techniky založené na zkušenostech
- b) Techniky černé skříňky
- c) Techniky bílé skříňky
- d) Techniky založené na riziku

3. Při testování nové funkce online bankovnictví se tester rozhodne vyzkoušet zadání extrémně vysoké částky pro převod, protože si vzpomíná, že v předchozím projektu podobná akce způsobila pád systému. O jaký přístup se jedná?

- a) Primárně technika bílé skříňky
- b) Primárně technika černé skříňky
- c) Technika založená na zkušenostech (Odhadování chyb)
- d) Pouze technika testování přechodů stavů

---

Dej mi vědět, jak si s otázkami poradíš, nebo pokud máš jakékoli dotazy k vysvětlenému tématu!
