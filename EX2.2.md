Bandit example Consider a k -armed bandit problem with k = 4 actions,
denoted 1, 2, 3, and 4. Consider applying to this problem a bandit algorithm using
"-greedy action selection, sample-average action-value estimates, and initial estimates
of Q 1 (a) = 0, for all a. Suppose the initial sequence of actions and rewards is A 1 = 1,R 1 = 1, A 2 = 2, R 2 = 1, A 3 = 2, R 3 = 2, A 4 = 2, R 4 = 2, A 5 = 3, R 5 = 0. On some of these time steps the " case may have occurred, causing an action to be selected at random. On which time steps did this definitely occur? On which time steps could this
possibly have occurred?

R = 

Valoração dos estados S1 = 0, S2 = 0, S3 = 0, S4 = 0 ----> Ação tomada = 1
No primeiro passo é possivel que tenha sido uma ação 'e' afinal todos os estados tinha valoração igual a zero

Valoração dos estados S1 = -1, S2 = 0, S3 = 0, S4 = 0 ----> Ação tomada = 2
No segundo passo é possivel que tenha sido uma ação 'e' pois  a melhor ação poderia ser S2, S3 ou S4

Valoração dos estados S1 = -1, S2 = 1, S3 = 0, S4 = 0 ----> Ação tomada = 2
No terceiro passo é possivel que tenha sido uma ação 'e' pois  a melhor ação é 2

Valoração dos estados S1 = -1, S2 = -0,5, S3 = 0, S4 = 0 ----> Ação tomada = 2
No quarto passo é usado uma ação 'e' pois  a melhor ação poderia ser 3 ou 4

Valoração dos estados S1 = -1, S2 = 1/3, S3 = 0, S4 = 0 ----> Ação tomada = 3
No quinto passo é usado uma ação 'e' pois  a melhor ação é 2