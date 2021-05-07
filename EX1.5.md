Other Improvements Can you think of other ways to improve the reinforce-
ment learning player? Can you think of any better way to solve the tic-tac-toe problem
as posed?

R =  Se o jogador estava se adaptando com o tempo, as atualizações antigas poderiam
acelerar a melhoria. Alterar a taxa de exploração / aprendizagem com base na variação
nas ações do oponente. Se o oponente está sempre fazendo os mesmos movimentos e você 
está ganhando com ele, então o e-greedy com 10% de exploração só vai fazer 
você perder os jogos. Mesmo que o jogo da velha seja um jogo solucionável, 
isso pode não resultar no melhor resultado com um oponente abaixo do ideal.