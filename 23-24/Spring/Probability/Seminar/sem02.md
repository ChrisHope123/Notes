* Binominális eloszlás
:(n alatt a k)
:számomra x%-al sikeres kisérleteket elvégzek sokszor és akkor ezt az értéket adja meg

* Geometriai elosztlás: elkezdek érmét dobálni, és ha először fejet kapok akkor megállok.
: P(k-adik után álltam meg ) p<sup>k-1</sup>*(1-p)
: ahol k = 1,2,3..

* Poisson :  λ > 0
: $$ P\left( x \right) = \frac{{e^{ - \lambda } \lambda ^x }}{{x!}} $$


* Hypergeometriai eloszlás
: általánosíttott lottó a tanmese hozzá

* várható érték (diszkrét esetben)
: P(X = xᵢ) = pᵢ
: E(X) = ∑ᵢ pᵢ  xᵢ

* negatív binominális
: k = n, n+1, ...
: (k-1/n-1) * pⁿ * (1-p)<sup> k-n</sup>
: Addig kísérletezünk, amíg meg nem kapjuk a n-edik sikeres próbálkozás
: Az első n-1 helyre betesszük n-1 sikeres kísérletet, majd elhelyezzük a többit sikeresnek illetve sikertelnek ~ valami ilyesmi a tanmese

Feladatok:
1. Adjuk meg annak a valószínŰségi változónak az eloszlását, ami egy hatgyermekes családban a fiúk számát adja
meg. (1/2 esély a fiú és a lány esélye is)
: Binominális eloszlás
2. Tegyük fel, hogy az új internet-elofizet ˝ ok véletlenszer ˝uen választott ˝ 20%-a speciális kedvezményt kap. Mi a valószín ˝usége, hogy 10 ismerosünk közül, akik most fizettek el ˝ o, legalább négyen részesülnek a kedvezményben
    * binominális eloszlás lesz.
    * n = 10, p = 1/5
    * behelyettesítünk
3. Egy tétel áru 1% selejtet tartalmaz. Hány darabot kell találomra kivennünk és megvizsgálnunk, hogy a megvizsgált darabok között legalább 0,95 valószín ˝uséggel selejtes is legyen, ha az egyes kiválasztott darabokat vizsgálatuk után visszatesszük.
: 1/100 valószínűséggel húzunk selejtet
: n a húzások száma
: P(n húzásnál van selejtes is) = 1-(99/100)ⁿ ≥ 0,95
: 0,05 ≥ (99/100)ⁿ
Legkisebb n amire ez igaz: felső egészrész(log<sub>99/100</sub> 0.05)   
5. Jelölje X az ötöslottón kihúzott lottószámok legkisebbikét. Adjuk meg X eloszlását.
: Legyen a legkisebb k .
: P(k a legkisebb lehúzott) = (90-k) alatt (4) / (90) al 5   

6. Egy érmével dobva (tfh. p a fej valószín˝usége), jelölje X az elso azonosakból álló sorozat hosszát. (Azaz pl., ha a ˝ sorozat FFI..., akkor X = 2.) Adjuk meg X eloszlását.
: P( az első k db ) = pᵏ * (1-p) + (1-p)ᵏ * p




megszámlálhatóan végtelen vs megszámlálhatatlanul végtelen
* természetes számok megszámlálhatóan végesek(pl induktív bevezetés stb.)
* valós számok megszámlálhatlanul végtelenek

Állítás: A valós szűmokat nem lehet megszámolni.
Bizonyítás: indirekt tfh. sorozatba rendezzük őket.
Írjuk fel őket tizedestört alakban  és csak a [0,1] intervallumon belülieket. Mátrixot csinálunk belőle - Cantor - féle átlós módszer

Házi: 3mas feladatsorban amik kimaradtak



