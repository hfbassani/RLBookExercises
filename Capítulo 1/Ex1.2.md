Exercise 1.2: Symmetries Many tic-tac-toe positions appear di↵erent but are really
the same because of symmetries. How might we amend the learning process described
above to take advantage of this? In what ways would this change improve the learning
process? Now think again. Suppose the opponent did not take advantage of symmetries.
In that case, should we? Is it true, then, that symmetrically equivalent positions should
necessarily have the same value?

Se o oponente com quem o algoritmo está jogando toma as mesmas ações para posições que são simétricas, então
é uma vantagem verificar há simetrias nas jogadas para assim, o algoritmo aprender com mais eficiência. Porém, se 
o jogador tomar ações diferentes para posições simétricas, então não valeria a pena verificar se há simetria, pois as ações
do oponente seriam diferentes daquelas que estávamos esperando. Dito isso, o valor de posições simétricas é igual para casos em que
o oponente toma as mesmas ações simétricas e diferente em casos que o oponente não toma a mesma ação simétrica.