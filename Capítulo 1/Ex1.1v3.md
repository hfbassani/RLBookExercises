Exercise 1.1: Self-Play Suppose,instead of playing against
a random opponent, the reinforcement learning algorithm described
above played against itself, with both sides learning. What do you think would happen
in this case? Would it learn a different policy for selecting moves?



Considerando o jogo Tic-Tac-Toe, ambos os oponentes aprenderiam a jogar de forma
perfeita caso o alpha nao fosse reduzido ao longo do tempo. Porém, a politica de cada jogador seria diferente. Caso ambos estivessem com alpha não decrescente ao longo das iterações, seria possível garantir que cada jogador não
iria convergir para ações que ganhariam sempre do mesmo oponente. Pois o oponente também está em constante aprendizado, realizando ações não gulosas e mudando lentamente a sua forma de jogar.
Já com alpha reduzindo ao longo do tempo em ambos os jogadores, ambos tenderiam a serem jogadores imperfeitos, pois com a taxa de aprendizado reduzindo, o aprendizado seria limitado. Por fim, caso houvesse a redução do alpha em apenas um
dos jogadores, o jogador sem a redução tenderia a ter uma politica ótima e melhor que a do outro jogador.