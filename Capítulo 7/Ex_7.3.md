### *Exercise 7.3:*

**Why do you think a larger random walk task (19 states instead of 5) was used
in the examples of this chapter? Would a smaller walk have shifted the advantage to a different
value of n? How about the change in left-side outcome from 0 to 1 made in the larger walk? Do
you think that made any difference in the best value of n?**

---
Resposta 1:

```
A tarefa de andar aleatoriamente (random walk) foi feita com 19 estados, ao invés de 5, para permitir um maior acumulo nas recompensas e assim ter uma maior precisão na estimativa n-step TD. Deste modo, um menor número de estados para caminhar o resultado de n tenderia a ser diferente. 
No caso de tornar os valores da esquerda por -1, depois de n-passos teremos que o a gente saberá pelo aprendizado que ele está no estado terminal da esquerda, talvez essa mudança não afete no melhor valor de n, mas apenas aumente a eficiência do aprendizado do agente.
```
