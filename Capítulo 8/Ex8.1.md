Exercise 8.1 The nonplanning method looks particularly poor in Figure 8.3 because it is
a one-step method; a method using multi-step bootstrapping would do better. Do you
think one of the multi-step bootstrapping methods from Chapter 7 could do as well as
the Dyna method? Explain why or why not.


O Dyna-Q sintetiza todas as experiências anteriores para alguns estados escolhidos de forma aleatória. Já o n-step bootstrapping
pode ser mais lento para convergir, pois atualiza apenas os últimos estados visitados. No entanto, existe um maior desperdício de computação no Dyna-Q,
pois alguns estados aleatórios que não são importantes serão atualizados. Portanto, o Dyna-Q consegue propagar de volta as recompensas
recebidas para estados anteriores na etapa de planejamento, já o n-step propaga para estados visitados anteriormente.