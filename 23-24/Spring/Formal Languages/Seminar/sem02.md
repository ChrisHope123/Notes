
##Szabályok

S → A | A + S
A → B | B * A
B → i | (S)

előreolvasunk: i + i * i
* S → A + <u>S</u> → A + <u>A</u>
* A + B * <u>A</u> → A + B * B
* A + B * i → A + i * i
* B + i * i → i + i * i

Tehát S →* i + i * i

*Adjunk grammatikát, amely az L₁ = {aᵐbⁿ | m,n ≥ 0} = {a}\*{b}** nyelvet definiálja
G = ({S,A,B}, {a,b}, P,S), ahol
P: S →A
...

grammophone app 

S  →   ϵ | aS | B 
B  →  bB | ϵ

