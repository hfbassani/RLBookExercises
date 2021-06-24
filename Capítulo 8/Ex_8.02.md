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
Porque essa exploração é realizada com base em um registro para cada par estado-ação das etapas de tempo decorridas desde a última tentativa do par em uma interação real com o ambiente. Então quando o ambiente se move o Dina-q+ tenta por meio da exploração esse par de ação tentado a muito tempo sem sucesso e acaba por encontrar  a saida. Onde o Dyna-q não explora e acaba por se prender a politica anterior e ter que atualiza-la toda novamente.
```