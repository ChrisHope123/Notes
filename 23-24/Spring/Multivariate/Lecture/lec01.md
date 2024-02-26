1. Adja meg a normált tér fogálmát!

* Legyen X ̸= ∅ egy lineáris tér R-felett és ∥.∥ : X → R olyan függvény (ún. norma), amelyre minden x, y ∈ X és λ ∈ R esetén igaz, hogy
    * ∥x∥ ≥ 0 és ∥x∥ = 0 ⇐⇒ x = 0,
    * ∥λx∥ = |λ| ∥x∥ (abszolút homogén),
    * ∥x + y∥ ≤ ∥x∥ + ∥y∥ (szubadditív).
* Ekkor az (X, ∥.∥) együttest normált térnek nevezzük. Ugyanakkor azt mondjuk, hogy ∥x∥ az x ∈ X elem normája.

2. Adjon meg három különböző normát az ℝ*ⁿ* lineáris téren!

* *Az ℝ*ⁿ* lineáris téren több norma is értelmezhető. A legfontosabbak a következők:
    
    * Euklideszi norma: $$  \| x \|_{2} := \left( {\sum_{k=1}^{n} x_{k}^{2}} \right)^{\frac{1}{2}} = \sqrt{x_{1}^{2} + x_{2}^{2} + \cdots + x_{n}^{2}} $$ 
    <br>

    * $$ \left\| x \right\|_{1} := \sum_{k=1}^{n} \left| x_{k} \right| = \left| x_{1} \right| + \left| x_{2} \right| + \cdots + \left| x_{n} \right| $$
    <br>

    * $$\left\| x \right\|_{\infty} := \max\left\{ \left| x_{k} \right|  | k = 1,2,3, ... ,n \right \} = \max \left\{ \left| x_{1} \right|, \left| x_{2} \right|, \ldots, \left| x_{n} \right| \right\} $$ 


3. Adja meg a környezet fogalmát az ℝ*ⁿ* euklideszi térben!
* Egy a ∈ ℝ*ⁿ* pont r (> 0) sugarú környezetén a
$$ K_{r}(a) := \left\{ x \in \mathbb{R}^{n} \mid \left\| x - a \right\| < r \right\}
$$ halmazt értjük.
n = 1 esetén Kr(a) az a pontra szimmetrikus (a − r, a + r) nyílt intervallum. Ha n = 2, akkor Kr(a) az a pont körüli r sugarú nyílt körlap, n = 3 esetén pedig az a pont körüli r sugarú nyílt gömb. A „nyílt gömb” elnevezést használjuk akkor is, ha n > 3.

4. Adja meg a torlódási pont fogalmát az ℝ*ⁿ* euklideszi térben!
* Tegyük fel, hogy A az ℝ*ⁿ* euklideszi térnek egy nem üres részhalmaza. 
* Ekkor a ∈ ℝ*ⁿ* az A halmaz torlódási pontja (jelekkel a ∈ A′ ), ha ∀K(a): K(a) ∩ A végtelen halmaz, azaz az a pont minden környezete végtelen sok A-beli pontot tartalmaz.

5. Adja meg a belső pont fogalmát az ℝ*ⁿ* euklideszi térben!
* Tegyük fel, hogy A az ℝ*ⁿ* euklideszi térnek egy nem üres részhalmaza.  
* Ekkor:a ∈ A az A halmaz belső pontja (jelekkel a ∈ int A), ha ∃K(a): K(a) ⊂ A,

6. Mikor mondjuk, hogy egy sorozat konvergens az ℝ*ⁿ* euklideszi térben?
Legyen 1 ≤ n ∈ N. Azt mondjuk, hogy az Rⁿ euklideszi tér (xₖ) : N → Rⁿ  sorozata konvergens, ha
$$ \exists A \in \mathbb{R}^{n}, \forall \epsilon > 0, \exists k_{0} \in \mathbb{N}, \forall k > k_{0}: \left\| x_{k} - A \right\| < \epsilon.
 $$
7. Milyen kapcsolat van egy sorozat konvergenciája és a hátárértéktől való távolsága között?  


8. Milyen kapcsolat van egy sorozat konvergenciája és a koordinátasorozatainak konvergenciája között?
Legyen n ∈ N⁺. Egy Rⁿ -beli sorozat akkor és csak akkor konvergens, ha a sorozat minden koordinátasorozata konvergens, és a határértéke a határvektor megfelelő koordinátája, azaz $$\mathbb{R}^{n} \ni x_{k} = (x^{(1)}_k, x^{(2)}_k, \ldots, x^{(n)}_k) \rightarrow A = (A^{(1)}, A^{(2)}, \ldots, A^{(n)}), \quad \text{ha } k \rightarrow +\infty $$ pontosan akkor igaz, ha minden i = 1, 2, . . . , n koordinátára $$ x^{(i)}_k \rightarrow A^{(i)}, \quad \text{ha } k \rightarrow +\infty. $$

9. Mit állít a Cauchy-féle konvergenciakritérium az ℝ*ⁿ* euklideszi térbeli sorozatokra?
Legyen n ∈ N⁺. Az Rⁿ euklideszi tér (xₖ) sorozata akkor és csak akkor konvergens, ha (xₖ) Cauchy-sorozat, azaz $$ \forall \epsilon > 0, \exists k_{0} \in \mathbb{N}, \forall k, l > k_{0} : \left\| x_{k} - x_{l} \right\| < \epsilon.
$$

10. Mit állít a Bolzano-Weierstrass-féle kiválasztási tétel az ℝ*ⁿ* euklideszi térre?
Az Rⁿ(n ∈ N⁺) euklideszi térben minden korlátos sorozatnak van konvergens részsorozata.
