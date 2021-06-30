### *Exercise 8.2:*

**Why did the Dyna agent with exploration bonus, Dyna-Q+, perform better in the first phase as well as in the second phase of the blocking and shortcut experiments?**

---
Resposta 1:

```
O algoritmo Dyna Q por ser menos exploratório, na primeira fase, pode ter encontrado um caminho não ótimo para chegar ao estado terminal  e continuou a seguir esse caminho por mais tempo do que no algoritmo Dyna Q+, que possui uma exploração do ambiente maior, consequentemente atingindo mais rapido a política ótima. Já na segunda fase, no primeiro experimento, acontece algo similar a primeira fase, no bloqueio do caminho, os dois algoritmos encontram o caminho ótimo, porém o Dyna Q+ o encontra mais rapidamente. No segundo experimento, na abertura de um novo caminho, o Dyna Q+ encontra a política ótima pela sua natureza mais exploratória, enquanto o Dyna Q continua indo pelo caminho não otimo, justamente por causa da sua natureza pouco exploratória, mesmo utilizando e-greedy. 
```
---
Resposta 2:

```
Dá pra resumir tudo ao fato do Dyna Q+ ser mais propenso a explorar, enquanto o Dyna-Q tende a ficar em um mesmo caminho por mais tempo, logo,
Dyna-Q+ explorou mais possibilidades e chegou ao estado terminal antes (phase 1), enquanto o Dyna-Q provavelmente ficou "preso" em algum caminho
falso. Na segunda fase, o Dyna-Q+ novamente, explorou mais (caminhos que ele não explorava há mt tempo) e encontrou o estado terminal muito antes
do Dyna-Q. 
```
