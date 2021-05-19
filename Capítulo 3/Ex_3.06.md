### *Exercise 3.6:*

**Suppose you treated pole-balancing as an episodic task but also used
discounting, with all rewards zero except for 1 upon failure. What then would the
return be at each time? How does this return differ from that in the discounted, continuing
formulation of this task?**

---
Resposta 1:

```
Seria o mesmo: -−γ elevado a k, onde k estaria em um intervalo de tempo

Em uma tarefa contínua, o gamma serve  para que o retorno não seja infinito, não exploda. Já na tarefa episódica, isso não acontece, dessa forma, o uso do gamma pode ser considerado inútil
```

---
Resposta 2:

```
Quando o agente se movimenta e o bastão não cai então recebe 0 de recompensa e 
quando o bastão cai recebe -1 de recompensa. Dessa forma analisando a formula do Ganho teremos:

G = R1 + yR2 + y²R3 + y3R4 + ... + y^(K+1)RK
como o episodio termina quando o bastao e quando nao cai recebe recompensa 0 então:
G = 0 + y0 + y²0 + y0 + ... + y^(K+1)-1
De modo que só iria importar o estado final daquele episodio
```