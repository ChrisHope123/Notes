relációs algebra
rekordok
  St
N | Gy
Mi | A
Mi | K
Ka | A

szeret → relációs 
π → peojekció → milyen oszlopokat szeretnénk megtartani 
π ₙₑᵥ szeret → az eredeti szeret táblát vegyük → 'vetítjük/projektáljuk a nev oszlopra'
A relációk eredménye halmaz, így az ismőtlédések nem szerepelhetnek benne.
Az eredmény
N 
Mi 
Ka


Milyen gyümölcsöket szeret micimackó?
Ahol név oszlopban micimackó szerepel, azokban a sorokban van az eredmény
Szelekció → logikai feltétel
(szigma)
σ <sub>nev = 'Mi'</sub> szeret


3.ℿ<sub> gy</sub> (2.σ <sub>nev = 'Mi </sub>' (1.Szeret))
egész tábla → micimackós sorok → gyümölcs oszlop

**SQL lekérdezések általános syntax**

SELECT *oszlopok*
from *táblák*
[where * feltétel*]


Megfeletetés relációs algebrával
select → Π
Π alsóindex → oszlopok
σ → where
σ alsóindex → feltétel
tábla {*name*} → from *name*

Összes oszlop kiválasztása a táblából → *

mivel a rekordok halmazok, így vannak halmazműveletink
Azért jó, mert így relációs algebrában és sqlben is tudjuk használni a halmazműveleteket.
Műveletek:
* ∖   MINUS
* ∩   INTERSECCT
* ∪   UNION

σ <sub>N = 'Mi' </sub> 
σ <sub>N ≠ | ≥ | ≤ 'Mi' </sub> ()
σ <sub>N ! 'Mi' </sub> → Not
σ <sub>N ∧ 'Mi' </sub> → And
σ <sub>N V 'Mi' </sub> → Or


**Feladat megoldások**
1. Melyek azok a gyümölcsök, amelyeket Micimackó szeret?
    * Ki kell választani a micimackós sorokat, majd a gyümölcs oszlopot
    * ℿ<sub> gy</sub> (σ <sub>nev = 'Micimackó' </sub> (Szeret))
    * SELECT GYUMOLCS FROM SZERET WHERE NEV = 'Micimackó'; 
2. Melyek azok a gyümölcsök, amelyeket Micimackó nem szeret? (de valaki más igen)
    * Válasszuk ki az összes gyümölcsöt, majd volnjuk ki belőle azon gyümölcsöket amiket micimackó szeret
    * ℿ<sub> gy</sub> (Szeret) ∖ ℿ<sub> gy</sub> (σ <sub>nev = 'Micimackó' </sub> (Szeret))
    * SELECT GYUMOLCS FROM SZERET MINUS SELECT GYUMOLCS FROM SZERET WHERE NEV = 'Micimackó';
3. Kik szeretik az almát?
    * Válasszuk ki azokat a sorokat ahol alma van, majd projektáljunk névre
    * ℿ<sub> n</sub> (σ <sub>gy = 'alma'</sub> (Szeret))
    * SELECT NEV FROM SZERET WHERE GYUMOLCS = 'alma';
4. Kik nem szeretik a körtét? (de valami mást igen)
    * Vegyük azokat, akik szeretik a körtét, majd vonjuk ki a nevek halmazából
    * ℿ<sub> n</sub> (Szeret) ∖ ℿ<sub> n</sub> (σ <sub>gy = 'körte' </sub> (Szeret))
    * SELECT NEV FROM SZERET MINUS SELECT NEV FROM SZERET WHERE GYUMOLCS = 'körte';
5. Kik szeretik vagy az almát vagy a körtét?
    * Válaszzuk ki azon embereket, akik szeretik az almát, majd azon embereket akik szeretik a körtét és uniózzuk össze.
    * Π<sub>n</sub>( σ <sub>gy = 'alma' </sub> (Szeret)) ∩ Π<sub>n</sub>( σ <sub>gy = 'körte' </sub> (Szeret))
    * SELECT NEV FROM SZERET WHERE GYUMOLCS = 'alma' UNION SELECT NEV FROM SZERET WHERE GYUMOLCS = 'körte';
6.  Kik szeretik az almát is és a körtét is?
    * Π<sub>n</sub>( σ <sub>gy = 'alma' </sub> (Szeret)) ∪ Π<sub>n</sub>( σ <sub>gy = 'körte' </sub> (Szeret))
    * SELECT NEV FROM SZERET WHERE GYUMOLCS = 'alma' UNION SELECT NEV FROM SZERET WHERE GYUMOLCS = 'körte';
7. Kik azok, akik szeretik a körtét, de nem szeretik az almát?
    * Válasszuk ki akik szeretik a körtét majd vonjuk ki akik szeretik az almát
    * Π<sub>n</sub>( σ <sub>gy = 'alma' </sub> (Szeret)) ∩ Π<sub>n</sub>( σ <sub>gy = 'körte' </sub> (Szeret))
    * SELECT NEV FROM SZERET WHERE GYUMOLCS = 'körte' INTERSECT SELECT NEV FROM SZERET WHERE GYUMOLCS = 'alma'










