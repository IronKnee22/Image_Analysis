⚠️✅

# 1. Jaké jsou rozdíly mezi analýzou obrazu (počítačovým viděním) na jedné straně a počítačovou grafikou na druhé straně? Uveďte dva příklady, které rozdíly demonstrují.✅
Počítačové vidění se snaží napodobit lidské vidění snímáním obrazu elektronickými prostředky a
porozuměním jejich obsahu počítačovým zpracováním(interpretací).U počítačového vidění je snaha
porozumět libovolné 3D scéně. Počítačové vidění je považováno za součást kybernetiky. Kromě
vlastních vjemů hraje důležitou úlohu také zkušenost.
Např: Počítačové čtení automobilových značek. Vstupem je obraz výstupem je text.
Počítačová grafika se naopak snaží zobrazit člověku informaci z počítače, často s možností
interakce.Snaží se zobrazit libovolnou 3D scénu. Počítačová grafika je samostatná kategorie
grafiky.
Např: počítačová hra – na základě interakce zobrazí určitou scénu(seskládanou jen z jednoduchých
elementů)

# 2. Vysvětlete, co se v analýze obrazů rozumí interpretací. Použijte vyjádření pomocí matematického formalismu. Co je v této souvislosti objekt a k čemu pomáhá jeho zavedení? Co interpretace při analýze obrazů na jednu stranu přináší a čím použití metod omezuje?✅
Interpretaci v analýze obrazu formálně definujeme jako zobrazení, které převádí pozorovaná obrazová data (syntaxi) na model teorie (sémantiku). Objekt je v této souvislosti chápan jako reálná entita, kterou data reprezentují, což pomáhá ukotvit abstraktní teorii v konkrétním světě, ve kterém tato teorie platí. Hlavním přínosem interpretace je, že surovým datům dodává význam a umožňuje porozumění scéně na základě znalostí o světě. Nevýhodou je, že tento přístup omezuje univerzálnost metody, protože interpretace je vždy závislá na kontextu konkrétního světa a jedné teorii může odpovídat více různých světů.

# 3. Proč je porozumění obecným (trojrozměrným) scénám v počítačovém vidění těžké? Uveďte několik důvodů se stručným komentářem. (V přednášce bylo uváděno šest důvodů)✅
3D → 2D přináší ztrátu informace díky vlastnostem perspektivní transformace (matematická abstrakce, dírková komora).

Měřený jas je dán složitým fyzikálním postupem vytváření obrazu. Zář (angl. radiance) (≈ jas) závisí na typu světelných zdrojů, jejich poloze, intenzitě, poloze pozorovatele, lokální geometrii povrchu a odrazivosti povrchu. Obrácená úloha je špatně podmíněna.

Nevyhnutelná přítomnost šumu v každém měření ve skutečném světě.

Příliš mnoho dat Stránka A4, 300 dpi, 8 bit per pixel = 8.5 Mbytes. 
Neprokládané video 512 × 768, RGB (24 bit) = 225 Mbits/sekundu.

Nutnost zahrnout interpretaci
Lokální okno v kontrastu s potřebou globálního pohledu

# 4. Lokální a globální zpracování. • Diskutujte stručně rozdíl mezi lokálním a globálním přístupem v analýze obrazu. Uveďte vý-hody a nevýhody obojího. • Uveďte se stručným komentářem dva příklady lokálních operací. • Uveďte se stručným komentářem dva příklady globálních operací.✅
## Lokální:
Lokálně nejsme schopni vnímat kontext obrazové informace. ten je velmi důležitý. může dojit ke špatné interpretaci. Nutnost zahrnout interpretaci

**Výhody**: Citlivost k lokálním detailům, schopnost zachytit texturu a detaily na mikroskopické úrovni.

**Nevýhody**: Může být citlivý na šum nebo místní variace a může vyžadovat komplexnější
zpracování. 

**např.** lokální průměrování, detekce hran

## Globální:
**Výhody**: Jednoduchý výpočet, vhodný pro celkové zpracování obrazu, nemá problémy s lokálním šumem nebo variacemi.

**Nevýhody**: Může ztratit detaily a informace na mikroskopické úrovni. 

**např.** úprava jasu, inverze obrazu

# 5. Vysvětlete pojem spojitá obrazová funkce f (x, y) nebo f (x, y, t). Vysvětlete, co jsou parametry x, y, t. Uveďte několik příkladů reálných obrazových funkcí sejmutých s pomocí různých fyzikálních principů. Hodnota funkce f tedy bude odpovídat různým fyzikálním veličinám.✅
Obrazová funkce je matematický popis rozložení energie v rovině (dvourozměrný signál), kde parametry x, y představují prostorové souřadnice. Hodnoty obrazové funkce f odpovídají některé fyzikální veličině, např. jasu u obrazu z černobílé TV kamery, teplotě u termovizní kamery nebo hustotě tkáně u rentgenu. Statický obraz je popsán funkcí dvou souřadnic f(x,y). Obrazová funkce tří proměnných se použije, když se plošné obrazy mění v čase t, tj. f(x,y,t), nebo v případě objemových obrazů f(x,y,z) – např. tomograf.

# 6. Co je to kvantování obrazu? Jak a v jakém zařízení se kvantování realizuje? Kolik kvantizačních úrovní zhruba rozliší u monochromatického obrazu člověk? Co je v obraze patrné, když je kvantizačních úrovní méně, než by mělo být?✅
Kvantování je přiřazení určité diskrétní hodnoty jasu danému bodu. Realizuje se na A/D
převodníku. Člověk rozliší zhruba 50 úrovní jasu. Když je v obraze méně kvantizačních úrovní než
je potřeba zaniknu jemné detaily obrazu a vzniknou falešné obrysy.

# 7. Uvažujte digitalizaci dvojrozměrného obrazu. Zde se stejně jako při digitalizaci jednorozměrného signálu stanovuje vzdálenost ekvidistantních vzorků podle Shannonovy věty o vzorkování. Pro dvojrozměrné obrazy je potřebné navíc ke stanovení vzdálenosti mezi vzorky (což se řeší podobně jako u jednorozměrného signálu) vyřešit další záležitost. Jakou? Jak se záležitost typicky řeší a jaké výhody či nevýhody tato řešení mají? Poznamenávám, že se neptám na kvantování.✅
Je potřeba rozhodnout o geometrickém uspořádání vzorků (topologii mřížky). Existují pouze 3 pravidelné mnohoúhelníky, jimiž lze beze zbytku pokrýt rovinu: trojúhelníky, čtverce a šestiúhelníky.

**Čtvercová mřížka (nejčastější)**:
- Výhody: Snadno realizovatelná (odpovídá maticovému zápisu, polím v paměti), standard pro většinu HW (CCD/CMOS, monitory).
- Nevýhody: Měření vzdálenosti (anizotropie): Vzdálenost mezi středy sousedních pixelů není konstantní (vzdálenost po úhlopříčce je 2​-krát větší než po straně).

**Hexagonální mřížka (včelí plástve)**:
- Výhody: Izotropie – všech 6 sousedů je stejně daleko. Má jednoznačnou definici spojitosti (neřeší se 4 vs 8 okolí). Je efektivnější při vzorkování kruhově symetrických signálů (menší hustota vzorků pro stejnou informaci).

- Nevýhody: Chybí přímá podpora v HW, složitější adresování pixelů a implementace algoritmů (např. FFT je na čtvercích mnohem rychlejší díky separabilitě).

# 8. Jaké výhody přináší použití hexagonální mřížky (podobné včelí plástvi) při vzorkování obrazu? Proč se taková mřížka nepoužívá ve většině digitalizačních karet?✅
**Výhody**: Má stejné vzdálenosti pro všechny sousedy jednotlivého bodu v mřížce, větší obrazová stabilita

**Nevýhody**: Většina technologií a obrazových standardů používá čtvercový rastr, vyžaduje složitější hardware, nekompatibilita pro běžné operace např. Fourierovu frekvenční filtraci.

# 9. Relace souvislosti mezi dvěma pixely binárního digitálního obrazu (tj. existuje mezi nimi cesta) definuje rozklad obrazu (tj. množiny) na třídy ekvivalence (tj. oblasti). Jaké tři vlastnosti musí relace splňovat, aby byla ekvivalencí. Ověřte platnost těchto tří vlastností pro relaci souvislosti.✅
## 1. Reflexivita:
- Každý pixel je sám se sebou v souvislosti (existuje cesta od pixelu do sebe sama).
- Reflexivita je obvykle automaticky splněna.

## 2. Symetrie:
- Pokud pixel A je ve vztahu souvislosti s pixelem B, pak i pixel B musí být ve vztahu souvislosti s pixelem A.

## 3. Tranzitivita:
- Pokud jsou pixely A a B ve vztahu souvislosti a pixely B a C jsou ve vztah souvislosti, pak musí být také pixely A a C ve vztahu souvislosti.
- Tranzitivita je klíčová pro vytváření tříd ekvivalence, protože umožňuje spojování sousedících pixelů do stejné třídy na základě spojitosti.

# 10. (a) Definujte (i) oblast a (ii) konvexní oblast ve dvojrozměrném obraze. Nakreslete příklad konvexní a nekonvexní oblasti. (b) Definujte konvexní obal. (c) Pro nekonvexní oblast z bodu (a) zakreslete konvexní obal.✅
**Konvexní** Když vezmeš jakékoliv dva body uvnitř tvaru a spojíš je rovnou čarou (úsečkou), ta čára zůstane celá uvnitř.

**Nekonvexní** Existují dva body uvnitř, které když spojíš, tak ta čára vyleze ven do prázdna. (Třeba u písmene "U" když spojíš oba vrchní konce).

**Konvexní obal** Představ si nekonvexní tvar (třeba hvězdu). Konvexní obal je ten nejmenší možný konvexní tvar, do kterého tu hvězdu můžeš zabalit.
- Jednoduše: Je to tvar, který vznikne, když vyplníš všechny "zálivy" a "promáčkliny".

# 11. Vysvětlete v souvislosti s obrazy význam pojmů (a) prostorové rozlišení; (b) spektrální rozlišení; (c) radiometrické rozlišení a (d) časové rozlišení.✅
- **Prostorové rozlišení**: Týká se schopnosti senzoru rozlišovat mezi blízkými objekty nebo detaily v prostoru (je dáno velikostí pixelu / vzorkovací frekvencí). Vyšší prostorové rozlišení znamená, že senzor zobrazí i menší detaily ostře.

- **Spektrální rozlišení**: Je dáno počtem a šířkou spektrálních pásem (kanálů). Černobílá kamera: 1 široké pásmo (nízké rozlišení). Barevná kamera: 3 pásma (R, G, B).

- **Radiometrické rozlišení**: Souvisí s počtem diskrétních úrovní jasu (tzv. bitová hloubka), které senzor dokáže rozlišit. Vyšší radiometrické rozlišení znamená, že senzor zachytí více jemných odstínů mezi nejtmavší a nejsvětlejší částí obrazu (např. 8 bitů = 256 úrovní).

- **Časové rozlišení**: Týká se frekvence, s jakou systém dokáže opakovaně snímat stejnou scénu (snímková frekvence u videa nebo perioda návratu u družic). Vyšší časové rozlišení umožňuje zachytit rychlé změny v čase a sledovat dynamické jevy.

# 12. Napište definiční vzorec Shannonovy (též informační) entropie. Vysvětlete veličiny ve vzorci. K čemu se Shannonova entropie používá? Uvažujte šedotónový obraz. Uveďte alespoň dvě použití Shannonovy entropie v digitálním zpracování obrazu.✅
𝐻𝑒 = − ∑ 𝑃(𝐾) log2 𝑃(𝐾)𝑘 [bit]

**Používá se při kompresi obrazu**:
- Entropie tvoří limit při bezeztrátové kompresi dat. Data nelze více zhustit než dovoluje jejich entropie, pokud nechceme ztratit informace v datech.

**Segmentace obrazu**:
- V oblasti zpracování obrazu lze Shannonovu entropii použít pro segmentaci obrazu. Nízká entropie může signalizovat homogenní oblasti nebo struktury, což může být využito při identifikaci a oddělení různých objektů nebo regionů v obraze. Vyšší entropie může naznačovat složitější nebo nejistější oblasti v obraze

# 13. I když nic nevíme o interpretaci obrazových dat, můžeme měřit informační obsah obrazu Shannonovou entropií. Uvažujte šedotónový obraz. Ukažte, jak spočítat entropii jasových úrovní obrazy s 2b stupni šedi obrazu o rozměru N × N z histogramu h(i), i = 0, . . . , 2b − 1. Pro jaký histogram bude entropie největší?✅
Počty jednotlivých jasů v histogramu podělíme rozměrem NxN a z vypočtených odhadů pravděpodobností vypočteme odhad entropie.

Entropie bude největší pro rovnoměrné rozložení jasů v histogramu.

# 14. Napište definiční vztah pro Shannovovu entropii. Uvažujte šedotónový obrázek. Spočítejte entropii na základě histogramu jasu hi , i = 0, . . . , 255. Ví se, že předzpracováním obrazu se entropie nezvětší. Co musíme udělat, když přesto potřebujeme obraz s větší entropií?✅
𝐻𝑒 = − ∑ 𝑃(𝐾) log2 𝑃(𝐾)𝑘 [bit]

## Možnosti zvýšení entropie:
**Přidat šum (Noise/Dithering)**: Přičtení náhodného šumu k obrazu zvýší míru "nepořádku" (neurčitosti) v datech, a tím matematicky zvýší entropii.

**Ekvalizace histogramu (Histogram Equalization)**: Toto je specifická výjimka často očekávaná u zkoušky. Cílem této metody je přiblížit histogram rovnoměrnému rozdělení. Rovnoměrné rozdělení má teoreticky maximální možnou entropii. Ačkoliv u diskrétního obrazu nemůžeme informaci "vyrobit", ekvalizace se snaží dostupnou bitovou hloubku využít co nejefektivněji (maximalizovat entropii výstupního obrazu).

# 15. Při pořizování obrazu trojrozměrného (3D) světa kamerou se geometrie zobrazení reprezentuje modelem dírkové kamery (tj. perspektivní projekcí), ve kterém se 3D bod (x, y, z) promítne do obrazové roviny jako (x, y). Nakreslete odpovídající obrázek (stačí o dimenzi menší, tj. plošný). Předpokládejte, že znáte 3D souřadnice (x, y, z), ohniskovou vzdálenost f, tj. vzdálenost obrazové roviny od středu promítání. Odvoďte vztah pro x.✅

![16](imgs/16.png)

Díky podobným trojúhelníkům pro perspektivní zobrazení platí:
![16](imgs/16_1.png)

Odvození přes podobné trojúhelníky:
![16](imgs/16_2.png)

# 16. K čemu slouží optická soustava (především objektiv) u fotoaparátu. Popište roli objektivu neformálně z fyzikálního hlediska.✅
Úkolem objektivu je posbírat rozbíhavé paprsky světla odražené od bodů ve scéně a "zlomit" je tak, aby se znovu sbíhaly (zaostřily) do jednoho bodu na rovině snímače. Tím vytváří věrný obraz scény.

**Zobrazení a zaostřování**
- Objektiv promítá 3D scénu do 2D roviny. Posunem čoček mění rovinu ostrosti tak, aby se paprsky protly přesně na povrchu snímače (nikoliv před ním nebo za ním).

**Sběr světla (Světelnost)**
- Objektiv soustřeďuje (sbírá) světlo z větší plochy na malou plochu snímače. Tím výrazně zvyšuje jas obrazu oproti pouhé dírkové komoře.

**Kontrola expozice (Clona)**
- Clona (umístěná uvnitř objektivu) mechanicky reguluje průměr otvoru, kudy proudí světlo. Tím ovlivňuje expozici a zároveň hloubku ostrosti (kolik toho je ostré před a za zaostřeným bodem).

# 17. Fungování objektivu fotoaparátu se obvykle na praktické úrovni vysvětluje teorií geometrické optiky. Za jakých předpokladů se může být zjednodušený model geometrické optiky použit? Podotýkám, že složitější fyzikální model je model vlnové optiky.✅

Geometrickou optiku (malování čar podle pravítka) můžeme použít tehdy, když ignorujeme vlnovou povahu světla, čočky jsou dostatečně velké a paprsky jdou blízko středu objektivu.

## Kdyby to nestačilo
**Rozměry systému vs. vlnová délka**:
- Základní předpoklad: Vlnová délka světla (λ) je zanedbatelně malá ve srovnání s rozměry optických prvků (čočky, clony) a objektů. Limitně se blíží nule (λ→0).

**Malé úhlové rozměry (Paraxiální aproximace)**:
- Pro použití jednoduchých zobrazovacích rovnic (jako je čočková rovnice) se předpokládá, že paprsky svírají s optickou osou jen malé úhly. Pokud jsou úhly velké, vznikají optické vady (aberace), které jednoduchý model nezohledňuje.

**Homogenita prostředí**:
- Předpokládá se, že prostředí je izotropní a homogenní (nemění se index lomu), takže se světlo šíří po přímkách. K lomu dochází jen na rozhraní prostředí (čočka-vzduch).

**Zanedbání difrakce (ohybu)**:
- Předpokládá se, že nedochází k ohybu světla. Tento předpoklad platí pouze tehdy, pokud jsou rozměry otvoru (clony) MNOHONÁSOBNĚ VĚTŠÍ než vlnová délka světla.

# 18. Srovnejte na konceptuální úrovni z pohledu fotografování vlastnosti dírkové komory a objektivu složeného z čoček.✅
**Dírková komora**: Má teoreticky nekonečnou hloubku ostrosti (nemusí se ostřit), ale extrémně nízkou světelnost. Dírka sbírá jen málo fotonů, proto vyžaduje dlouhé expozice.

**Objektiv (Čočka)**: Sbírá násobně více fotonů (světla) z celé plochy čočky a soustředí je do jednoho bodu, což umožňuje krátké expozice a ostrý obraz. Na rozdíl od dírky musí být zaostřen na konkrétní vzdálenost(má omezenou hloubku ostrosti) – objekty mimo tuto vzdálenost budou neostré.

# 19. Vysvětlete, co je přirozená vinětace. Projevuje se přirozená vinětace více u normálních objektivů nebo u širokoúhlých objektivů? Zdůvodněte (v lepším případě odvoďte), proč k přirozené vinětaci dochází.✅
Je to jev, kdy dochází k poklesu jasu (intenzity osvětlení) směrem k okrajům obrazu. Více se projevuje u širokoúhlých objektivů, protože pracují s většími úhly dopadu světla.

# 20. Vysvětlete, co je to radiální zkreslení objektivu. Jak se v sejmutém obraze projevuje a jak se opravuje?✅
Jde o převládající geometrickou vadu, kdy se měřítko zobrazení mění se vzdáleností od středu obrazu. Rovné linie se v obraze jeví jako zakřivené.

Projevuje se ve dvou hlavních formách:
- Soudkovité (Barrel): Linie se vyboulují směrem ven (typické pro širokoúhlé objektivy/krátká ohniska).
- Poduškovité (Pincushion): Linie se prohýbají směrem dovnitř (typické pro teleobjektivy).

Koriguje se výpočtem (přemapováním pixelů) na základě známých koeficientů zkreslení, které se zjistí kalibrací kamery.

# 21. Vysvětlete pojem pojem Bayerova mřížka u barevných kamer a fotoaparátů? Liší se rozlišení v barvě (na čipu) od počtu pixelů? Pokud ano, jak?✅
Bayerova mřížka je mozaika barevných filtrů umístěná přímo na obrazovém snímači. Umožňuje snímači (který jinak měří jen intenzitu světla) zachytit barevný obraz. Mřížka má podobu vzoru, ve kterém jsou jednotlivé pixely pokryty filtry propouštějícími jen jednu barvu. Tento vzor (RGGB) se skládá z 50 % zelených (G), 25 % červených (R) a 25 % modrých (B) pixelů. Zelené je více, protože lidské oko je na tuto barvu nejcitlivější.

Rozlišení v barvě se liší od počtu pixelů (je nižší). Protože každý pixel fyzicky změří jen jednu barevnou složku (R, G nebo B), zbývající dvě barvy pro daný bod se musí dopočítat (interpolovat) z hodnot okolních pixelů (tzv. demosaicing). Plná barevná informace tedy není změřená v každém bodě, ale je zčásti odhadnutá.

# 22. Vysvětlete pojem hloubka zaostření u optického objektivu. Jaký (obvykle ovladatelný) parametr objektivu umožňuje měnit hloubku zaostření?✅
**Hloubka zaostření (Depth of Focus)**: Týká se obrazového prostoru (uvnitř kamery). Je to tolerance polohy snímače – rozsah, v jakém můžeme posunout snímač podél optické osy, aniž by se obraz stal rozmazaným (rozptylový kroužek nepřesáhne velikost pixelu).

Ovladatelný parametr je clona (clonové číslo). Zvýšení clonového čísla (zmenšení otvoru) zúží kužel světelných paprsků. Tím se zmenší průměr rozptylových kroužků neostrých bodů a zvětší se jak hloubka ostrosti, tak hloubka zaostření.

# 23. Představte si, že snímáme 3D scénu, jejíž elementární ploška odráží jistou záři L do CCD kamery. To se na jejím světlocitlivém čipu odpovídá ozáření E, které je přímo úměrné hodnotě obrazové funkce f (x, y), tj. jasu (přesněji záři). Na jakých vlastnostech elementární plošky a zdrojů světelné energie hodnota f (x, y) pro pevně zvolená x, y závisí?✅
- lokální geometrie
- koeficient odrazivosti albedo
- úhel natočení
- směr pohledu
- vlnová délka dopadajícího světla


# 24. Jaké odrazivostní vlastnosti má lambertovský povrch? K čemu se zjednodušení odrazivostních vlastností daných lambertovským modelem používá? Uveďte alespoň dva příklady použití.✅
je idealizovaný model povrchu, který má několik zjednodušujících předpokladů o odrazivosti.
• Odráží světelnou energii rovnoměrně do všech směrů. Proto je zář (a také jas) ze všech
směrů konstantní. Jeho BRDF je také konstantní.
• Odrazivost je nezávislá na úhlu pohledu
Lambertovský model je pro svou jednoduchost značně oblíbený. Používá se pro výpočty
odrazivosti nebo v počítačové grafice. 3D rekonstrukce fotky pokud je tenhle pixel tmavší víme že je dál od světla

# 25. Co řeší v radiometrii rovnice ozáření? Zkuste úlohu formulovat (asi Vám pomůže, když si nakreslíte obrázek a označíte v něm veličiny) a naznačit myšlenky odvození (vzorce nejsou nezbytně nutné).✅
Rovnice ozáření popisuje základní vztah mezi tím, jak moc září objekt ve skutečnosti (Zář L), a tím, kolik světla nakonec skutečně dopadne na snímač kamery (Ozáření E). Jednoduše řečeno: je to matematický předpis, který nám říká, jak objektiv převede jas scény na jas fotky.

Myšlenka odvození stojí na logickém sledování toku světla: Vycházíme z malé plošky na scéně, která vyzařuje světlo do prostoru. Objektiv kamery z tohoto záření „vykrojí“ jen určitou část – konkrétně kužel světla, který se vejde do otvoru clony (průměr d). Tato zachycená energie se pak přenese a soustředí na odpovídající malou plošku na snímači (pixel).

## Když nebude stačit
Rovnice ozáření (Fundamental Radiometric Equation) popisuje vztah mezi září (Radiance L) povrchu scény a ozářením (Irradiance E), které dopadá na snímač kamery. Říká, že obraz je přímo úměrný jasu scény, ale je ovlivněn nastavením kamery a polohou v obraze.
E=L⋅4π​(fd​)2cos4α

Kde:

    E: Ozáření obrazu [W⋅m−2] (energie dopadající na pixel).

    L: Zář scény [W⋅m−2⋅sr−1] (jas objektu).

    d: Průměr otvoru clony (aperture).

    f: Ohnisková vzdálenost (vzdálenost snímače od čočky).

    α: Úhel paprsku od optické osy (způsobuje přirozenou vinětaci).

Myšlenky odvození (kroky):

    Zdroj: Uvažujeme elementární plošku objektu dO, která vyzařuje energii (má zář L).

    Sběr světla: Spočítáme, kolik energie (tok Φ) dopadne z této plošky na čočku o průměru d. To závisí na prostorovém úhlu, pod kterým ploška "vidí" čočku.

    Přenos: Předpokládáme bezeztrátovou čočku – veškerá energie zachycená čočkou je soustředěna do plošky obrazu dI.

    Geometrie: Z podobnosti trojúhelníků (perspektivní zobrazení) vyjádříme poměr velikosti ploch dO a dI.

    Závěr: Dosazením zjistíme, že dopadající energie na jednotku plochy snímače (E) klesá s druhou mocninou clonového čísla (f/d) a se čtvrtou mocninou úhlu (cos4α).

Popis k obrázku: Optická osa je osa Z, objektiv (čočka) je v počátku.

    dO: Ploška na objektu (zdroj).

    dI: Ploška na snímači (obraz).

    d: Průměr čočky.

    α: Úhel mezi optickou osou a paprskem (určuje polohu pixelu na snímači).

    z: Vzdálenost objektu od čočky.

# 26. Charakterizujte předzpracování obrazu. Co je vstupem a výstupem předzpracování obrazu. K čemu předzpracování obrazu slouží? Uveďte tři příklady použití metod předzpracování.✅
Předzpracování obrazu (tzv. low-level processing) je fáze zpracování, která připravuje data pro následnou automatickou analýzu. Klíčovou charakteristikou je, že vstupem je obraz a výstupem je opět obraz (nikoliv text, graf nebo příznaky).

**Slouží ke dvěma hlavním účelům:**
- Potlačení nežádoucích vlivů vzniklých při snímání (šum, geometrické zkreslení, neostrost).
- Zvýraznění důležitých vlastností pro další zpracování (např. vytažení hran).

**Příklady metod:**
- Filtrace (odstranění) šumu – např. vyhlazování nebo mediánový filtr.
- Úprava jasu a kontrastu – např. ekvalizace histogramu pro lepší využití dynamického rozsahu.
- Zaostření

# 28. Charakterizujte dvojrozměrnou konvoluci. K čemu se dvojrozměrná konvoluce používá v digitálním zpracováním obrazu?✅
Dvourozměrná konvoluce je matematická operace, která kombinuje obrazy s konvoluční maskou tak, aby vznikl
obraz třetí (násobení ve frekvenční oblasti). Používá se jako frekvenčně selektivní filtr přičemž lze
definovat: dolní propust (odstranění šumu, rozmazání) horní propust (zvýraznění hran v obrázku)

# 29. Jakými metodami předzpracování obrazu zvýšíte kontrast šedotónového obrazu pro pozorovatele, máte-li k dispozici právě tento jediný obraz. Uveďte alespoň dvě kvalitativně odlišné metody. Vysvětlete stručně princip těchto metod.
## Histogramová ekvalizace:✅
- Tato metoda se snaží rovnoměrně rozdělit jasové úrovně v histogramu obrazu. Histogram je transformován tak, aby byl co nejvíce uniformní. Tím se zvýší kontrast mezi různými jasovými úrovněmi.

## Adaptivní kontrastová úprava:
- Tato metoda bere v úvahu okolní regiony pixelů a upravuje kontrast lokálně na základě charakteristiky každého regionu. Místo jednotné transformace celého obrazu adaptivní kontrastová úprava analyzuje okolí každého pixelu a upravuje kontrast v souladu s okolními hodnotami.

# 30. Napište definiční vztah pro přímou a inverzní jednorozměrnou Fourierovu transformaci. Vyjádřete neformálně princip a význam Fourierovy transformace.✅

Fourierova transformace je vyjádření časově závislého signálu pomocí harmonických signálů, tj.
funkcí sin a cos, obecně tedy funkce komplexní exponenciály. Slouží pro převod signálů z časové
oblasti do oblasti frekvenční. Signál musí být periodický a splňovat Dirichletovy podmínky. Signál
může být buď ve spojitém či diskrétním čase.

# 31. Jaká je asymptotická výpočetní složitost jednorozměrné Fourierovy transformace.Použijte značení ‘velké O’ v závislosti na délce n vstupního diskrétního signálu (posloupnosti).✅
O(n<sup>2</sup>)

# 32. Vysvětlete, co je dvojrozměrná Fourierova transformace, její rozdíl od jednorozměrné (můžete definičním vzorcem nebo neformálně). Jak se dvojrozměrná Fourierova transformace používá ve zpracování obrazu.✅
Dvourozměrná Fourierova transformace je rozšířením jednorozměrné Fourierovy transformace na dvourozměrné oblasti, jako jsou například matice nebo obrazy. Zatímco jednorozměrná Fourierova transformace pracuje s jednorozměrnými signály, dvojrozměrná Fourierova transformace zpracovává dvourozměrné signály, což umožňuje analýzu prostorové struktury a frekvenčního obsahu dvourozměrných dat.

Používá se zejména k filtraci a zpracování obrazu, kompresi dat nebo analýze obrazových textur.

# 33. Vztah mezi šířkou frekvenčního spektra ve Fourierově transformaci a dobou trvání jednorozměrného signálu je dán (Heisenbergovým) principem nejistoty. Formulujte neformálně princip a vysvětlete jeho význam pro frekvenční analýzu ve zpracování signálů (obrazů).✅
Čím přesněji změřím čas, tím rozmazanější bude informace o frekvenci a naopak

# 34. Fourierova transformace je definována pro periodické signály. Mnohé praktické signály, s nimiž běžně pracujeme, jsou neperiodické. Nazvěte a neformálně vysvětlete dva přístupy, které se zde obvykle používají.✅
**Okenková metoda**: zpracovat signál po malých částech (oknech) a předpokládat, že vně je signál periodický.

**Použití složitějších bázových funkcí**, např. vlnek ve vlnkové (wavelets) transformaci

# 35. Vyjádřete větu o konvoluci, tj. jak je konvoluce vyjádřena ve Fourierově transformaci. Pro jednoduchost uvažujte jednorozměrný případ.✅
f(t)∗g(t) ⟷ F(ω)⋅G(ω)

Věta o konvoluci (Convolution Theorem): Konvoluce dvou funkcí v časové (nebo prostorové) oblasti odpovídá prostému násobení jejich spekter ve frekvenční oblasti (a naopak).

# 36. Jaká je výpočetní složitost diskrétní Fourierovy transformace pro dvojrozměrný obraz o velikosti N × N pokud byste v algoritmu použili přímo definiční vztah? Připomínám, že asymptotický odhad algoritmické složitosti se zapisuje formou O(.), kde se v argumentu v našem případě bude vyskytovat výraz obsahující N . Na multiplikativní a aditivní konstanty se nebude brát zřetel.✅
O(n<sup>4</sup>)

# 37. K urychlení diskrétní Fourierovy transformace byl před více než padesáti lety navržen algoritmus rychlé Fourierovy transformace (FFT). Jaký je jeho princip? Jsou nějaká omezení na velikost vstupního 2D obrazu?✅
Principem je metoda rozděl a panuj. Dlouhý signál se opakovaně půlí na sudé a liché vzorky, dokud nezbydou jen triviální dvojice. Ty se snadno spočítají a pomocí „motýlkového schématu“ poskládají zpět.

Omezení je Mocniny 2 aby se to dalo vždycky rozdělit

# 38. Jaká je algoritmická složitost algoritmu FFT pro dvojrozměrný obraz o velikosti N × N ?✅
O(n<sup>2</sup>) * log N

# 39. Formulujte Shannonovu (též Nyquistovu, Kotelnikovu) větu o vzorkování pro jednodušší případ jednorozměrného signálu. Vysvětlete (stačí neformálně, obrázek pomůže), jak se věta o vzorkování dokazuje (nápověda: frekvenční spektra).✅
Formulace: Abychom mohli signál z digitálních vzorků bezchybně vrátit zpět do analogové podoby, musí být vzorkovací frekvence větší než dvojnásobek nejvyšší frekvence v signálu.

![41](imgs/41.png)

# 40. (a) Televizní signál o 25 snímcích za sekundu je vzorkován do matice 500 × 500 pixelů ve 256 jasových úrovních. Vypočtěte nejmenší vzorkovací frekvenci (v kHz), kterou musí být signál v digitizéru (angl. frame grabber) vzorkován? (b) Jak se jmenuje věta, podle které jste výpočet realizovali? Naznačte myšlenku jejího odvození (stačí úvaha, vzorce nejsou nezbytně nutné).✅
a) Vypočtěte nejmenší vzorkovací frekvenci (v kHz). • 6 250 kHz (Výpočet: 500 pixelů × 500 pixelů × 25 Hz = 6 250 000 Hz = 6 250 kHz. Počet jasových úrovní nemá na vzorkovací frekvenci vliv, jen na datový tok).

b) Jak se jmenuje věta a naznačte myšlenku odvození. 
- Shannon-Kotělnikovův teorém (nebo Nyquist-Shannonova věta). 
- Tento teorém se dokazuje přes frekvenční spektra. Z Fourierovy transformace vyplývá, že vzorkování v čase způsobí, že se spektrum signálu periodicky opakuje na násobcích vzorkovací frekvence fvz​. Aby se tato kopie spekter vzájemně nepřekrývala (nenastal aliasing), musí být vzorkovací frekvence minimálně 2krát vyšší než nejvyšší frekvence obsažená v signálu (fmax​).




# 91. Je eroze binárního obrázku komutativní operací? Proč (vyjděte z jedné z definic eroze)?
Eroze není komutativní operací, protože oba vstupy v ní hrají zcela odlišnou roli.

I když jsou z hlediska počítače A i B matice (tedy obrázky), v morfologii je A velký zkoumaný obraz (scéna), zatímco B je maličký nástroj zvaný strukturní element (nebo maska).

Princip eroze spočívá v otázce: "Vejde se tento malý nástroj (B) celý dovnitř objektu na velkém obrázku (A)?"
- Pokud erodujeme A pomocí B, zjišťujeme, kde všude se malá maska vejde do velkého objektu. Výsledkem je zmenšený objekt.
- Pokud bychom to otočili a erodovali B pomocí A, ptali bychom se: "Vejde se tento obrovský obrázek celý dovnitř té jedné malé masky?" Odpověď je prakticky vždy ne. Výsledkem by byl prázdný obraz.

