In the comparison shown in Figure 2.2, which method will perform best in
the long run in terms of cumulative reward and probability of selecting the best action?
How much better will it be? Express your answer quantitatively.


R = Quando o "e-greedy" é médio o algoritmo pode escolher uma maquina muito ruim e por azar a recompensa dela for muito alta, dessa forma iria demorar mais para o algoritmo perceber que aquela maquina é de fato ruim. Com "e-greedy" é muito pequeno acontece algo pior pois com o raciocinio de sempre escolher a melhor ação o algoritmo pode achar uma maquina que lhe dar 3 como recompensa enquanto que a maioria das outras lhe dão -1. Porem pode existir uma maquina que lhe der 10 como média. A grande questão é escolher o valor certo da explotação/exploração