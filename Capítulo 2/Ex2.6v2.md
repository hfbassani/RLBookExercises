Exercise 2.6: Mysterious Spikes The results shown in Figure 2.3 should be quite reliable because they are averages over 2000 individual, randomly chosen 10-armed bandit tasks.
Why, then, are there oscillations and spikes in the early part of the curve for the optimistic method? 
In other words, what might make this method perform particularly better or worse, on average, on particular early steps?



As oscilações podem acontecer dado que o agente considera que ações ruins são boas e ao longo das iterações vai realizando
ações gulosas (exploitation) e pode encontrar uma ação com valores de recompensa altos. Outra característica interessante
é a curva de porcentagem das ações ótimas que cresce de forma mais lenta no Optimistic greedy, pois as ações ruins são
executadas como se fossem boas e vão recebendo menores recompensas até que sejam consideradas ruins. Essa exploração inicial
pode trazer menores recompensas, porém, se as ações ruins receberem recompensas muito pequenas, o agente pode aprender rapidamente
a diferenciar ações ruins e convergir rapidamente em seguida.