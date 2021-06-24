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
Sem a interação do agente com jogadas de oponentes humanos, o agente iria aprender a modificar e alcançar o objetivo (Vitória) por meio de jogadas próprias. Sendo assim, o aprendizado estaria enviesado a políticas e escolhas de ações restritas ao comportamento do agente com o ambiente modificado pelo próprio agente. Portanto, as ações estando ligadas a ele mesmo iriam por muitas vezes parecer sem sentido. Desta forma, fica claro que  suas políticas de escolhas são diferentes de uma escolha humana.
```
