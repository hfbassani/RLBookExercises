### *Exercise 6.5:*

**In the right graph of the random walk example, the RMS error of the TD method seems to go down and then up again, particularly at high α’s. What could have caused this? Do you think this always occurs, or might it be a function of how the approximate value function was initialized?**

---
Resposta 1:

```
Eu acredito que esteja relacionado a inicialização da função de estado-valor, e é intensificado por α. Se os valores iniciais da função
de estado-valor não tiverem uma inicialização tão boa (por exemplo, os estados que não levam para uma recompensa favoravel possuem estado-valor melhores)
o algoritmo vai demorar para convergir para os valores reais, mas vai convergir eventualmente. Caso contrário (estado-valor com inicialização mais realista)
o algoritmo vai convergir mais rápido para o "ótimo", porém, eventualmente vai tentar novos caminhos e isso vai causar um RMS maior (com α’s menores, o RMS é menor
pois o passo não foi tão "drástico").
```
