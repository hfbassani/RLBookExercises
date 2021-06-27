### *Exercise 5.5:*

**Consider an MDP with a single nonterminal state and a single action that transitions back to the nonterminal state with probability p and transitions to the terminal state
with probability 1-p. Let the reward be +1 on all transitions, and let  = 1. Suppose you observe one episode that lasts 10 steps, with a return of 10. What are the first-visit 
and every-visit estimators of the value of the nonterminal state?**
---
Resposta:

```
Denotando por s=X0 o estado não-terminal e T=10.

Para o caso first-visit o valor do estado não-terminal só será atualizado na primeira visita, ou seja:
V(s=X0) = γG + R10 = 1*0 + 1 => V(X0) = 1
Nas iterações seguintes o algoritmo já terá passado por X0 e seu valor não será atualizado.

Para o caso every-visit o valor é atualizado pela média de G a cada iteração, assim:
em t=T-1=9: G <- γG + R10 = 1 => V(s=X0) = avg(G) = 1
t=8: G <- γG + R9 = 1+1 = 2 => V(s=X0) = avg(G) = (1+2)/2 = 1,5
...
t=0: G <- γG + R9 = 9+1 = 10 => V(s=X0) = avg(G) = (10+9+8+...+1)/10 => V(X0) = 5,5
```
