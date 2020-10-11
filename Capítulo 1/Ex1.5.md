Exercice 1.5: Can you think of other ways to improve the reinforcement learning player? Can you think of any better way to solve the tic-tac-toe problem as posed?

    Uma maneira de melhorar o aprendizado do Reinforcement Learning player é criando um script com jogadas preferiveis antes de rodar o algoritmo de aprendizado. Como o jogo da velha é um jogo simples, existem jogadas que em um determinado estado do jogo são mais utilizadas por jogadores convencionalmente, uma ideia de como seria o script inicial:
    
    * Mais 02 pontos se a posição for a central;
    * Mais 01 ponto se a posição estiver nos quatro cantos da matriz;
    * Menos 02 pontos, se já houver uma ou mais peças do adversário na mesma linha, coluna ou diagonal onde a posição se encontra;
    * Mais 04 pontos se a posição impedir a vitória do adversário;
    * Mais 04 pontos se a posição levar a uma vitória;
    
    Escolhendo sempre a jogada que da mais pontos, isso pode acelerar o processo de aprendizado total ou pelo menos melhorar o jogo inicial do Reiforcement Learning player.