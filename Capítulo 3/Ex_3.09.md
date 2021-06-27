### *Exercise 3.9:*

**Suppose y = 0.9 and the reward sequence is R1 = 2 followed by an infinite sequence of 7s. What are G1 and G0?**

---
Resposta 1:

```
Temos que: R1 = 2, y = 0,9 e Rk = 7, para k > 1.

G1 = R2 + y*G2 = R2 + y*R3 + y²*R4 + ... = 7*(1+0,9+0,9²+0,9³+...) = 7*[1/(1-0,9)] = 70

G0 = R1 + y*G1 = 2 + 0,9*70 = 65

```
