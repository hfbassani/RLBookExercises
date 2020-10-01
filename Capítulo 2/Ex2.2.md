Exercise 2.2: Bandit example Consider a k-armed bandit problem with k = 4 actions, denoted 1, 2, 3, and 4. Consider applying to this problem a bandit algorithm using "-greedy action selection, sample-average action-value estimates, and initial estimates of Q1(a) = 0, for all a. Suppose the initial sequence of actions and rewards is A1 = 1, R1 = -1,A2 = 2,R2 = 1,A3 = 2,R3 = -2,A4 = 2,R4 = 2,A5 = 3,R5 = 0. On some of these time steps the ε case may have occurred, causing an action to be selected at random. On which time steps did this definitely occur? On which time steps could this possibly have occurred?

    Foram executadas 5 ações, o que provoca 5 estados (s1, s2, s3, s4, s5), para cada time step temos as seguintes qualidades das ações (Q), considerando a equanção Action-Value, apenas ações com Q diferente de 0:
            A1  A2    A3  A4  A5
        - 1: 0, 0,    0,  0,  0
        - 2: 1, 0,    0,  0,  0
        - 3: 1, 1,    0,  0,  0
        - 4: 1, 1.5,  0,  0,  0
        - 5: 1, 1.67, 0,  0,  0

    Analisando cada momento individualmente, no que diz respeito a ação ε:
        - 1: Inicialmente todos os Qs são 0, a escolha da ação a1 pode ter sido escolhida ε ou 1 - ε.
        - 2: A ação a2 foi escolhida aqui, só pode ter sido aleatoriamente, visto que Q(A1) é o maior valor.
        - 3: Aqui, as ações a1 e a2 possuem Q iguais, e novamente a ação a2 foi escolhida, o que pode ter sido escolhido ε ou 1 - ε.
        - 4: Q(a2) é o maior valor, 1.5, pode ter sido a escolha gulosa (maior valor) ou aleátoria também (todas as ações têm a mesma probabilidade de serem escolhidas).
        - 5: Nesse caso, Q(a2) é o maior valor, 1.67, e foi escolhida a ação a3, o que demostra que foi aleatória, pois a ação gulosa, a2, não foi escolhida.

    Portanto, nos time steps 2 e 5, as ações foram escolhidas de forma aleátoria (ε), enquanto que no restante pode ter sido ε ou 1 - ε.