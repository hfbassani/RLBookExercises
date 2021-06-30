### *Exercise 5.2:*

**Suppose every-visit MC was used instead of first-visit MC on the blackjack task. Would you expect the results to be very di↵erent? Why or why not?**

---
Resposta 1:

```
Se eu entendi direito, a politica do player diz que deve-se parar assim que atingir 20 (ou 21), e ele está sempre considerando o "Ace" com
o valor 11 (caso não estoure). Nesse caso, o estado "final" seria atingir 20 ou 21 (se eu entendi direito), logo, o game acaba sempre com 2 cartas
(2 caras de valor 10, 1 cara de valor 10 e um ace de valor 11, ou 2 aces de valor 11 [derrota]). Ou seja, a única forma de aplicar o "every-visit"
seria mudar o valor do ace de 11 para 1, garantindo assim que o jogo durasse mais, e que mais aces apareçam (o que é bastante improvavel, por ser
uma carta mais rara). Dessa forma, é provavel que o player perca mais no inicio (devido a "naturals" do inimigo, que obviamente vai considerar
o ace com valor 11), mas eventualmente vai convergir para uma politica boa.
```