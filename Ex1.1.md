Self-Play Suppose, instead of playing against a random opponent, the
reinforcement learning algorithm described above played against itself, with both sides
learning. What do you think would happen in this case? Would it learn a diferent policy
for selecting moves?

R = Neste caso os algoritmos iriam valirizar os estados de maneiras diferentes. Imagine o jogo Tic Toc onde o jogador A sempre começa jogando. Dessa forma o Jogador B nunca viu o tabuleiro vazio e portando nao saberia qual posição escolher quando visse pela primeria vez o tabuleiro vazio. Os jogadores apesarem de usar o mesmo algoritmo de aprendizagem por reforço poderiam aprender politicas diferentes pois cada jogador teria suas próprias experiências.

