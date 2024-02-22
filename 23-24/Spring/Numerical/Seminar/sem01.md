1. Gyak

2. feladat
10,85 felírása 2-es számrendszerben

10 2-es számrendszerben "akasztófa módszerrel" → 10 → 1010
.85 2-es számrendszerrel "akasztófa módszer "szorozgatással"" → gyakorlatilag ugyan az, csak kettővel osztás helyett szorzunk, az egész rész kerül balra, majd mod 2, illetve felülről lefele olvasva kell értelmeznmi
.85 szor2 → 1,70, 1.40, 0.8 1.6, 1.2 (5 elem mivel 5ös mantissza)
0.85 → 11011...
tehát 10,85₁₀ → 1010.1|1011₂ → kerekítés szükséges, mivel 1 a levágott rész első karaktere, így felfele kerekítünk
így → 10,85 ₁₀ → 1011.0₂
A tizedespont nincs a helyén, 4-el balra toljuk(a számnak tizedestörtnek kell lennie)
.10110 → egy 4-es eltolás, avagy karakterisztika → +[.10110|4]

Tehát fl(10,85) → +[10110|4]ű

Számoljuk ki a hibáját ennek a kerekítésnek.

A hiba a .85 kerekítéséből adódik.

hiba: |10.85 - fl(10.85)| (avagy a bevitt szám és a kapott eredmény távolsága)
|10.85 - fl(10.85)| ≤ 1/2 * 2⁴ * 2⁻⁵ = 1/4 → 1/4-edes hibát kapunk.

Megjegyzés: Mi történik ha nem normalizált a szám? azaz az első számjegy nem 1.
                     Például fl(0,13) → "kettévágjuk a tizedesvesszőnél"
                     2|13
                     0|26
                     0|52    → 0.00100⋯ ₂ → vigyük helyére a pontot(normalizálás) → -2-es eltolás  → [100|-2] 
                     1|04
                     0|08
                     ⋯

                     Mi történik ha nem férünk bele a karakterisztika hosszunkba?
                     A definíció szerint ilyenkor minden számjegyhez a 0-át rendeljük.



Az első értékes karaktertől kell leszámolni a mantissza hossz + 1-et, azaz itt a 3-mas feladatban 7 számjegyet kell kiszámolni


3, feladat
közelítsük a x-1/6-ot a M(6,-5,5)-ben!
Induljunk ki a következő közelítő értékekből:
a) → 1/6 = 0,16
 
   2 | 16
   0 | 32
   0 | 64  → 0.00100⋯ ₂ → -3-as eltolás → [100 | 3]
   1 | 24
   0 | 48
   0 | 96
   

4. feladat

a,
Ha van kis és nagy karakteresztikájú számok számokat akarunk összeadni, akkor a kisebb karakterisztikájú számot egyeztetjük meg a nagobb szzámnak.
Ilyenkor kis mantissza értéknél és nagy "szám" ranggel meg tudjuk azt csinálni, hogy "kitoljuk" a kisebb számot, így a + b = a és b ‌≠ 0

b, rontsuk el az asszociativitást


5,

adjuk meg az 1 és 8 gépi számot
kettő hatványok megadása egyszerű,

Hogyan vonunk ki gép számoakt egymásból(példatárban fordulhat elő)

