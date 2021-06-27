### *Exercise 6.3:*

**From the results shown in the left graph of the random walk example it appears that the first episode results in a change in only V (A). What does this tell you
about what happened on the first episode? Why was only the estimate for this one state changed? By exactly how much was it changed?**
---
Resposta:

```
Como apenas o valor do estado A decresceu, podemos inferir que o agente terminou o episódio no estado terminal da esquerda, ou seja, com recompensa 0.

Pois todos os estados foram inicializados com o mesmo valor V(S) = 0,5, o fator de desconto utilizado foi de γ=1 e A era o estado mais próximo do estado terminal, assim,
apenas este valor foi modificado após o fim do episódio.

No algoritmo TD(0) os estados são atualizados por:
V(St) <- V(St) + α[Rt+1 + γ*V(St+1) - V(St)]

No passo em que o agente se move de A para o estado terminal, temos:
V(A) <- 0,5 + 0,1*[0 + 1*0 - 0,5] = 0,5 - 0,05 => V(A) <- 0,45
```
