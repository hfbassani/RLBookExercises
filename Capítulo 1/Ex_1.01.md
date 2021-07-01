### *Exercise 1.1: Self-Play*

**Suppose, instead of playing against a random opponent, the reinforcement learning algorithm described above played against itself, with both sides learning. What do you think would happen in this case? Would it learn a different policy for selecting moves?**

---
Resposta 1:

```
O algoritmo aprenderia com ele mesmo maneiras de vencer o jogo, através da experiência adquirida nas suas partidas. Sua política de movimento será diferente da de um humano, pois o algoritmo não teve nenhum contato(jogando contra ou por um modelo) com técnicas utilizadas por um humano, possuindo assim um maneira única de jogar, e podendo até existir momentos na partida que o algoritmo faça jogadas contraintuitivas para um humano, pois ele aprendeu que essa é a melhor jogada nessa situação para obter a vitória no final da partida.
```

---
Resposta 2:

```
Neste caso os algoritmos iriam valorizar os estados de maneiras diferentes. Imagine o jogo Tic Toc onde o jogador A sempre começa jogando. Dessa forma o Jogador B nunca viu o tabuleiro vazio e portando nao saberia qual posição escolher quando visse pela primeria vez o tabuleiro vazio. Os jogadores apesar de usarem o mesmo algoritmo de aprendizagem por reforço poderiam aprender politicas diferentes pois cada jogador teria suas próprias experiências.
```

---
Resposta 3:

```
No mesmo problema de um jogo da velha, com o alpha mantido constante e um epsilon não nulo como a probabilidade de uma jogada exploratória, eventualmente ambos jogarão de forma quase ótima a menos de um epsilon. Isso porque, quando ambos convergirem, ainda assim em epsilon porcento das vezes o agente jogará uma jogada aleatória. Se ambos jogarem de forma gulosa a partir desse momento, ambos jogarão de forma ótima. Se o alpha não for constante ou não houverem jogos o suficiente, é possível que os agentes acabem convergindo para um comportamento subótimo, um mínimo local.

Já se considerarmos problemas além do de jogo da velha, e se é a nossa intenção que o agente possa enfrentar oponentes diversos, a possibilibade de corvergência para um comportamento subótimo é maior. A Deepmind usou um esquema de torneio com uma população de agentes tanto para o Alpha Zero quanto para o Alpha Star para enfrentar esse problema, no primeiro usando o ELO dos agentes para pareamento, e no segundo usando o próprio sistema de classificação de StarCraft II para pareamento. De outra forma, um par de oponentes pode convergir numa estratégia subótima que só leva em conta o adversário, onde um oponente pode se tornar dominante, limitando o tamanho das partidas. Isso só é mais evidente em jogos mais complicados, como xadrez, shogi ou GO.
```