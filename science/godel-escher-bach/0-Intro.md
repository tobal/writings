# Bevezetés - Zeneo-logikai áldozat

Nem is olyan rég olvastam el először a Gödel Escher Bach - Egybefont Gondolatok Birodalma c. könyvet D. R. Hofstadter-től, és azóta is próbálom feldolgozni. Akárhányszor megkérdezik tőlem, hogy miről szól, sosem tudom egy kerek egész mondattal, érthetően elmondani. Többel sem. Ez valószínűleg azt jelenti, hogy én magam sem értem. Ugyanakkor a könyv, bár majdnem 40 éve íródott, olyan témát feszeget, amiről manapság sem tudunk sokkal többet, mint akkor, és engem személy szerint a legmesszebbmenőkig érdekel. A könyv ugyanis nem más, mint az öntudat működésével kapcsolatos legfontosabb általánosságokra adott számos izomorfizmus bemutatása.

Ezért elhatároztam, hogy szeretném megérteni a könyvet. Ezt pedig legkönnyebben úgy érhetem el, ha figyelmesen újra elolvasom, és jegyzetet készítek minden fejezetről.  Ha pedig már készítek egy ilyen jegyzetet, miért ne tegyem azt közkinccsé, akár a saját gondolataimmal kiegészítve? Úgyhogy egy kis bemelegítésnek fogadjátok szeretettel a bevezető fejezet jegyzetét.

A bevezetés egy Bach-ról szóló anekdotával nyit, amikor Frigyes király meghívta az udvarába, hogy kipróbálja az új zongoráit (bár akkor még nem így hívták őket). Bach zseniális improvizációkat adott elő a király által adott zenei témára, majd később megfelelően kidolgozva azokat Zenei Áldozat címen tette közzé. Ennek kapcsán szó esik a kánonokról és fúgákról is, ahol már most felüti a fejét néhány később részletesen kifejtett téma: a rekurzió, a jelentés és a kódolás.

A kánon nem más, mint egy adott zenei téma (dallam) több szólamban való megszólaltatása, időben eltolva egymáshoz képest. Ez máris egyfajta rekurzió, de a könyv témáival való izomorfizmusok sora ezzel nem áll meg. Az izomorfizmus jelentését is részletesebben fogja tárgyalni a könyv, itt elég annyit megjegyezni róla, hogy két dolog között akkor áll fent izomorfizmus, ha valamilyen módon megfeleltethetőek egymásnak. Például amikor egy kánonban több szólam együttes összhangzatát halljuk, azt tekinthetjük egyfajta dekódolásnak, amit az agyunk végez (tehát a kánon összhangzatának érzékelése izomorf egy kódolt üzenet visszafejtésével). A kód ebben az esetben a dallam egy adott hangja, ami a dallam más hangjaival egyszerre megszólalva egy harmonikus összhangzatot képez, ami nem más, mint a dekódolt “üzenet”. A kódok többszintű jelentésének témája is felbukkan, ugyanis egy hang zenei jelentése más és más attól függően, hogy milyen más hangokkal szólal meg egyidőben.

A könyv ezután rátér egy másik ilyen általánosságra: a furcsa hurkokra. A furcsa hurkok az egész könyvet végigkísérik majd, általánosan megfogalmazva arról a jelenségről van szó, amikor egy hierarchikus rendszerben a szintek között lefelé vagy felfelé lépkedve egyszer csak ugyanarra a szintre jutunk, ahonnan elindultunk (elvileg az öntudat is ilyen végtelenül ismétlődő gondolatok furcsa hurkaiból születik). Egy ilyen általános megfogalmazás alapján nem igazán lehet megérteni, hogy mi is ez, ezért a könyv rögtön hoz is egy példát: Bach a Zenei Áldozatban megkomponált egy zenei furcsa hurkot, egy örökké emelkedő kánont, amiben egyre magasabb és magasabb hangnemben ismétli ugyanazt a témát (ezt hívják modulációnak), mindaddig, amíg el nem jut ugyanabba a hangnembe, ahonnan elindult. Így az egész a végtelenségig folytatható, és azt az illúziót kelti, hogy a hangmagasság egyre csak emelkedik. Ha nem hiszed, hogy ez lehetséges, hallgasd meg ezt:

[![Shepard tone video][shepard-yt-image]][shepard-video]

A könyv ezután Escher műveiben mutatja be ugyanezt a jelenséget. A Vízesés című műve például egy ötlépcsős furcsa hurkot ábrázol:

![Escher waterfall][escher-waterfall]

Escher rajzaiban, hasonlóan Bach zeneműveihez, kifejezésre jutnak azok a témák, amikkel a könyv behatóan foglalkozik. A fejezetben a szerző Gödelnek is külön alfejezetet szentel, aki egy matematikus volt, és a Nem Teljességi Tétele miatt érdekes. A bevezető a tétel nagyon rövid bemutatását is tartalmazza.

Az egész történet az Epimenidész paradoxonnal kezdődik, ami alapvetően arra mutat rá, hogy nem minden mondatról lehet eldönteni, hogy igaz-e vagy hamis. Ha ugyanis azt írom, hogy “ez a mondat hamis”, akkor akár igaznak, akár hamisnak próbálom titulálni, a mondat ellentmond ennek, így ez paradoxonhoz vezet. A matematikában rengeteg ehhez hasonló paradoxon van, amiknek kiküszöbölésére rengeteg különfélel elméletet, különféle matematikát dolgoztak ki. Például a halmazelméletben jelen van a Russell-paradoxon, ami az önfelfaló halmazokkal kapcsolatos: döntsük el, hogy tartalmazza-e önmagát az a halmaz, amelyikre igaz az, hogy tartalmazza az összes olyan halmazt, ami nem tartalmazza önmagát (a halmazelméletben minden további nélkül meghatározhatunk ilyen halmazt). A szerző szavaival élve: tessék kipróbálni!

Ehhez hasonló paradoxonoktól hemzseg a matematika, ilyen például a Kleene-Rosser paradoxon is. Az összes ilyen paradoxont az okozza, hogy megengedjük az önhivatkozást. A direkt vagy indirekt önhivatkozással ugyanis egy furcsa hurok jön létre, ami önellentmondáshoz vezethet. A fent leírt Epimenidész paradoxon is azért jöhet létre, mert megengedjük, hogy egy mondat önmagára hivatkozzon. A matematikában ezeket a paradoxonokat az önhivatkozás “megtiltásával” küszöbölték ki, például a típuselméletben.

Amit Gödel bebizonyított az az, hogy nem hozható létre olyan matematika, amiben minden igaz állítást kifejezhetünk, és paradoxonok sincsenek benne. És ami az extra poén, hogy mindennek a bizonyítására egy furcsa hurkot használt (amihez először kitalálta, hogyan írhat olyan matematikai állítást, ami nem számokról, hanem egy másik matematikai állításról szól, így lehetővé téve az önhivatkozást). Ez a bizonyítás később részletesen is be lesz mutatva a könyvben.

Aztán egy látszólagos témaváltással a fejezet áttér a számítógépek kialakulására és a mesterséges intelligenciára. Lamentál kicsit az intelligencia mibenlétén, és felteszi a kérdést: vajon létrehozhatunk-e intelligens gépet? Ez a kérdés azért fontos, mert ez a fokmérője annak, hogy megértettük-e, hogy hogyan működik a saját tudatunk. Ha viszont a saját tudatunkkal akarjuk megérteni a saját tudatunkat, az kicsit olyan, mintha a saját hajunknál fogva akarnánk felemelni magunkat. Ráadásul ha úgy van ahogy sejtjük, vagyis a tudatban létező furcsa hurkokból ered az öntudat és ezzel együtt az intelligencia, akkor megkérdőjeleződik, hogy képesek lehetünk-e valaha gondolkodó gépet létrehozni, elvégre a számítástechnika a matematikán alapul, ami pedig (Gödel tétele szerint) nem tud mit kezdeni a furcsa hurkokkal. A könyv ezt a témát járja körül, a jegyzetem további részében ezt fogom bemutatni.

[shepard-yt-image]: http://img.youtube.com/vi/BzNzgsAE4F0/0.jpg
[shepard-video]: https://www.youtube.com/watch?v=BzNzgsAE4F0
[escher-waterfall]: https://upload.wikimedia.org/wikipedia/en/e/e8/Escher_Waterfall.jpg