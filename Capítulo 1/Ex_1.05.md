### *Exercice 1.5: Other Improvements*

**Can you think of other ways to improve the reinforcement learning player? Can you think of any better way to solve the tic-tac-toe problem as posed?**

---
Resposta 1:

```
Uma maneira de melhorar o aprendizado do Reinforcement Learning player é criando um script com jogadas preferiveis antes de rodar o algoritmo de aprendizado. Como o jogo da velha é um jogo simples, existem jogadas que em um determinado estado do jogo são mais utilizadas por jogadores convencionalmente, uma ideia de como seria o script inicial:

* Mais 02 pontos se a posição for a central;
* Mais 01 ponto se a posição estiver nos quatro cantos da matriz;
* Menos 02 pontos, se já houver uma ou mais peças do adversário na mesma linha, coluna ou diagonal onde a posição se encontra;
* Mais 04 pontos se a posição impedir a vitória do adversário;
* Mais 04 pontos se a posição levar a uma vitória;

Escolhendo sempre a jogada que da mais pontos, isso pode acelerar o processo de aprendizado total ou pelo menos melhorar o jogo inicial do Reiforcement Learning player
```

---
Resposta 2:

```
Se o jogador estava se adaptando com o tempo, as atualizações antigas poderiam acelerar a melhoria. Alterar a taxa de exploração / aprendizagem com base na variação nas ações do oponente. Se o oponente está sempre fazendo os mesmos movimentos e você está ganhando com ele, então o e-greedy com 10% de exploração só vai fazer você perder os jogos. Mesmo que o jogo da velha seja um jogo solucionável, isso pode não resultar no melhor resultado com um oponente abaixo do ideal.
```

---
Resposta 3:

```
Uma melhoria que acho que pode ser significativa é fazer o agente "perceber" que está sendo enviesado, por exemplo, quando o inimigo faz as mesmas jogadas pela quinta vez seguida (assim como o inimigo) e ganha novamente, acredito que nesses casos o aprendizado poderia "forçar" o agente a fazer uma jogada epsilon greedy com 100% de certeza (100% de certeza que não fará a "melhor" jogada). Isso já melhoraria bastante o aprendizado, pois priorizaria a exploração e de certa forma, impediria um enviesamento.
```
