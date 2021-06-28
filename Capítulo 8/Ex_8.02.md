### *Exercise 8.2:*

**Why did the Dyna agent with exploration bonus, Dyna-Q+, perform better in the first phase as well as in the second phase of the blocking and shortcut experiments?**

---
Resposta 1:

```
O algoritmo Dyna Q por ser menos exploratório, na primeira fase, pode ter encontrado um caminho não ótimo para chegar ao estado terminal  e continuou a seguir esse caminho por mais tempo do que no algoritmo Dyna Q+, que possui uma exploração do ambiente maior, consequentemente atingindo mais rapido a política ótima. Já na segunda fase, no primeiro experimento, acontece algo similar a primeira fase, no bloqueio do caminho, os dois algoritmos encontram o caminho ótimo, porém o Dyna Q+ o encontra mais rapidamente. No segundo experimento, na abertura de um novo caminho, o Dyna Q+ encontra a política ótima pela sua natureza mais exploratória, enquanto o Dyna Q continua indo pelo caminho não otimo, justamente por causa da sua natureza pouco exploratória, mesmo utilizando e-greedy. 
```

Resposta 2:

```
O bônus de recompensa dado ao Dyna Q + é um dos fatores que fazem ele ter uma recompensa maior e com isso o algoritmo tende a procurar por caminhos não ótimos que não foram visitados e levam até o estado terminal, como consequência pela exploração de novos caminhos a recompensa é aumentada. Nesse caso essa exploração é uma vantagem, pois quando há o bloqueio do que era o caminho anterior, o Dyna-Q que tinha grande otimismo no caminho anterior vai continuar errando, enquanto que o Dyna-Q+ irá explorar melhor o ambiente.
```