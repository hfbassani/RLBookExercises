Exercise 2.3: In the comparison shown in Figure 2.2, which method will perform best in the long run in terms of cumupative reward and probability of selecting the best acton? How much better will it be? Express your answer quantitatively.

    O método ε = 0.01 performa melhor ao longo do tempo, mesmo ε = 0.1 convergindo mais rápido, porém conforme o número de tentantivas cresce, ε = 0.01 tem desempenho superior. Isso ocorre porque, ambos convergem para um valor de recompensa ótimo quando o número de tentantivas tende ao infinito. Porém, como ε = 0.01 utiliza ações gulosas (greedy) em cerca de 99% das vezes, enquanto que o outro por 90%, serão escolhidas mais vezes a ação que maximize a recompensa, ou seja, o fator aleatório, será menor para ε = 0.01.
    Simulando quantitativamente o q*(a), ou seja, a recompensa ótima para cada ação, temos:
        Para ε = 0.01 --> 0.99 * 1.5 = 1.485
        Para ε = 0.1 --> 0.9 * 1.5 = 1.35
    Percebe-se que com ε = 0.01, é esperado uma recomensa maior.
    Ps.: Levei em consideração que a recompensa esperada para 1 - ε, ações aleatórias é 0, visto que, são desconhecidas e aleatórias.