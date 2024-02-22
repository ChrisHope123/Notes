relatrív gyakoriság: n kisérlet, ebből k alkalommal következik be kedvező esemény ., A viszgált esemény relatív gyakorsisága ilyenkor k/n

ha n → ∞ mellett a relatív gyakoriságnak van egy határértéke, akkor ez lesz az esemény valószínűsége.

A valószínűség értéke ∈ (0,1)

A biztos esemény lehetősége 1, a lehetetlen esemény valószínűsége 0

Ha veszek eseményeket amik páronként egymást kizárják, akkor igaz, hogy az összegük valószínűsége az ugyan az mint az ő valószínéségének összege, azaz P(A₁ + A₂ + ⋯) = P(A₁) + P(A₂) + ⋯

Feltételes valószínűség: Tudom hogy B bekövetkezik, mennyi a valószínűsége, hogy ezen feltétel mellett  A is bekövetkezik.

P(A|B) = P(AB) / P(B) (Területes magyarázat → B egy "biztos" esemény, ehhez viszonyítjuk az A eseméynt)

1.1
Hányféleképpen lehet 8 bástyát letenni egy sakktáblára, hogy ne üssék egymást?
1 → Semelyik kettő bástya sem kerülhet azonos sorba és oszlopba.
2 → Haladjunk soronként:
                                           1 sor → 8 lehetőség
                                           2 sor → 7 lehetőség
                                           ⋯
                                           8 sor → 1 lehetőség
Ez alapján 8! a válasz

1.2
Mi a valószínűsége, hogy egy véletlenszerűen kiválasztott 6 jegyű szám jegyei mind különbözoek?
1 → Összes : 9 * 10^5
2 → kedvező 9 * 9 * 8 * 7 * 6 * 5
3 → ebből osztással számolandó

1.3. Feladat. Ha egy magyarkártya-csomagból (32 lap: piros, zöld, makk, tök) visszatevéssel húzunk három lapot, akkor mi
annak a valószínűsége, hogy
a) pontosan egy piros színű lapot húztunk?
1 → minden húzásnál 1/4 valószínűséggel lesz piros.
2 → 3 helyen lehet piros → 1/4 * (3/4)^2 * 3

b) legalább egy piros színű lapot húztunk?

komplementer esemény(nempiros nempiros nempiros) → (3/4)^3
így a valószínűség 1 -  (3/4)^3

1.5
. ⋆ n dobozba véletlenszer˝uen helyezünk el n golyót úgy, hogy bármennyi golyó kerülhet az egyes dobozokba.
a) Mi a valószín˝usége, hogy minden dobozba kerül golyó?
b) Annak mi a valószín˝usége, hogy pontosan egy doboz marad üresen?

a
Összes : → minden golyó választ magának dobozt → n ^ n
Kedvező → n! →

b
Öszes → minden golyó választ magának dobozt → n ^n
Kedvező n * (n-1) * (n a 2) * n-2 
