### *Exercise 2.6: Mysterious Spikes*

**The results shown in Figure 2.3 should be quite reliable because they are averages over 2000 individual, randomly chosen 10-armed bandit tasks. Why, then, are there oscillations and spikes in the early part of the curve for the optimistic method? In other words, what might make this method perform particularly better or worse, on average, on particular early steps?**

---
Resposta 1:

```
O método otimista tem ou pode ter picos na fase inicial porque o agente busca usar mais a exploitação do que a exploração. 
Ou seja, a tendência é que ele busque ações que possam ter boas recompensas imediatas 
em vez de explorar várias ações diferentes procurando formar uma "opinião" sobre determinada ação.
```

---
Resposta 2:

```
Por ter um inicio "otimista" todas as ações tem recompensas igualmente boas (pelo menos no caso da figura 2.3), o que significa que o agente vai explorar todas elas de forma igualitária pelo menos uma vez (a ideia é justamente incentivar a exploração), e isso vai acontecer justamente no inicio, logo, o agente vai escolher alguma ação que não leve a uma boa recompensa final (uma ação não otima)o que vai causar aqueles "spikes" no gráfico, porém, eventualmente, ele vai voltar a convergir para o ótimo.
```
