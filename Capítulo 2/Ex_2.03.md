### *Exercise 2.3:*

**In the comparison shown in Figure 2.2, which method will perform best in the long run in terms of cumupative reward and probability of selecting the best acton? How much better will it be? Express your answer quantitatively.**

---
Resposta 1:

```
Em questão de longo prazo o método que utiliza ϵ = 0.1 terá um desempenho pior que o ϵ = 0.01 assim como em termos de recompensa cumulativa e probabilidade cumulativa. Primeiramente, em termos de recompensa, pode-se demonstrar matematicamente 
que ϵ = 0.1 terá como resultado 0.9 * 1.55 = 1.395, o valor de 1.55 surge da máquina com maior probabilidade gaussiana média, no caso a terceira do exemplo, no caso de ϵ = 0.01 o resultado será 0.99 * 1.55 = 1.5345. O acúmulo de probabilidade tem que ϵ = 0.1 irá selecionar
a melhor ação com a probabilidade de 90% e ϵ = 0.01 irá selecionar a melhor ação com probabilidade de 99%.

```

