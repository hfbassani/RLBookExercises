### *Exercise 4.2:*

**In Example 4.1, suppose a new state 15 is added to the gridworld just below state 13, and its actions, left, up, right, and down, take the agent to states 12, 13, 14,
and 15, respectively. Assume that the transitions from the original states are unchanged. What, then, is vπ(15) for the equiprobable random policy? Now suppose the dynamics of
state 13 are also changed, such that action down from state 13 takes the agent to the new state 15. What is vπ(15) for the equiprobable random policy in this case?**

---
Resposta 1:

```
Para o caso em que as transições originais se mantém, podemos calcular o valor do estado 15 a partir dos valores dos estados adjacentes, uma vez que eles não se alteram:

Sabemos que:
- vπ(12) = -22
- vπ(13) = -20
- vπ(14) = -14

Tomando γ = 0,9, temos:

vπ(15) = Eπ[Rt+1 + γvπ(St+1) | St = s] = 0,25*(-1-0,9*22)+0,25*(-1-0,9*20)+0,25*(-1-0,9*14)+0,25*(-1-0,9*vπ(15))
=> vπ(15) = -17,55

Já para o segundo caso, os valores dos demais estados também são alterados durante o processo de convergência:

```
