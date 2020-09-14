Exercise 2.2: Bandit example Consider a k-armed bandit problem with k = 4 actions,
denoted 1, 2, 3, and 4. Consider applying to this problem a bandit algorithm using
"-greedy action selection, sample-average action-value estimates, and initial estimates
of Q1(a) = 0, for all a. Suppose the initial sequence of actions and rewards is A1 = 1,
R1 = 1, A2 = 2, R2 = 1, A3 = 2, R3 = 2, A4 = 2, R4 = 2, A5 = 3, R5 = 0. On some
of these time steps the " case may have occurred, causing an action to be selected at
random. On which time steps did this definitely occur? On which time steps could this
possibly have occurred?

Primeira iteração = não temos certeza se a ação 1 foi escolhida aleatoriamente ou se foi por padrão (Ex: Se Q1(a) = 0 para todos os a, então a primeira ação deve ser escolhida)
Segunda iteração = Foi exploração, já que a greedy action era a primeira ação
Terceira iteração = Empate entre a primeira e segunda ação. Não temos certeza se foi uma escolha aleatória entre as duas ou se foi por padrão (Ex: Entre um empate, escolher a mais recente)
Quarta iteração = Greedy action
Quinta iteração = Foi exploração, já que a greedy action era a segunda ação
