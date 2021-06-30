### *Exercise 5.8:*

**The results with Example 5.5 and shown in Figure 5.4 used a first-visit MC method. Suppose that instead an every-visit MC method was used on the same problem. Would the variance of the estimator still be infinite? Why or why not?**

---
Resposta 1:

```
Ainda seria infinito, porque em ambos os casos (single e every visit) só se sabe a recompensa no final do episódio, e seria sempre 1 (só o estado final da recompensa).
Logo, a média seria também 1, j*y / j = 1 (y é o valor de gama, que nesse caso é 1), e a variancia continuaria sendo infinita, independente de qual método está sendo empregado.
```
