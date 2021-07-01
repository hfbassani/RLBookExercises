### *Exercise 8.3:*

**Careful inspection of Figure 8.5 reveals that the difference between Dyna-Q+ and Dyna-Q narrowed slightly over the first part of the experiment. What is the reason for this?**

---
Resposta 1:

```
O Dyna-Q+ encontra de uma maneira mais rápida a política ótima pela sua maior natureza exploratória, porém mesmo já possuindo a política ótima ele é forçado a continuar explorando, é por esse custo exploratório que a diferença entre Dyna-Q + e Dyna-Q vai se estreitando
```

---
Resposta 2:

```
Durante a primeira parte do experimento, rapidamente o Dyna-Q+ encontra uma boa política por conta dos passos exploratórios reaproveitando a experiência anterior. Porém, o Dyna-Q acaba se aproximando do Dyna-Q+ justamente por conta dos passos aleatórios dados pela política epsilon-greedy. Dessa forma, a melhoria no Dyna-Q se dá pelo passo de aprendizado direto, quando uma ação aleatória é escolhida. Já a pequena piora do Dyna-Q+ ocorre pelo fato de que ainda por cima da política epsilon-greedy, o Dyna-Q+ ainda precisa revisitar ações que não foram visitadas faz tempo por conta do termo k * √𝜏. Perceba que a ordem de decaimento do tempo 𝜏 dessas ações segue a visitação original das ações, isto é, se eu visito os estados S1, S2, S3, então S1 "decairá" primeiro de forma a ter um alto k * √𝜏, logo em seguida S2 e assim por diante. Como o passo de planning acontece mais vezes, mas então o aspecto greedy da política original se transfere e se soma na fase de planejamento, decaindo o Dyna-Q+ em performance um pouco mais do que o Dyna-Q. Se o uso de uma política greedy faz com que a acurácia máxima do agente seja 90%, então com o Dyna-Q+ ela acaba sendo um pouco menor que 90%.
```