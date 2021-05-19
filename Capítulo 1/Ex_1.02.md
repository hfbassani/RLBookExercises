### *Exercise 1.2: Symmetries*

**Many tic-tac-toe positions appear different but are really the same because of symmetries. How might we amend the learning process described above to take advantage of this? In what ways would this change improve the learning process? Now think again. Suppose the opponent did not take advantage of symmetries. In that case, should we? Is it true, then, that symmetrically equivalent positions should necessarily have the same value?**

---
Resposta 1:

```
Se o oponente com quem o algoritmo está jogando toma as mesmas ações para posições que são simétricas, então é uma vantagem verificar há simetrias nas jogadas para assim, o algoritmo aprender com mais eficiência. Porém, se  o jogador tomar ações diferentes para posições simétricas, então não valeria a pena verificar se há simetria, pois as ações do oponente seriam diferentes daquelas que estávamos esperando. Dito isso, o valor de posições simétricas é igual para casos em que o oponente toma as mesmas ações simétricas e diferente em casos que o oponente não toma a mesma ação simétrica.
```

---
Resposta 2:

```
Para o jogo da velha é possível usar 4 eixos de simetria para basicamente dividir o numero de estados por 4. Isso aumentaria drasticamente a velocidade / reduziria a memória necessária. Se o oponente não aproveitasse as simetrias, isso poderia resultar em um pior desempenho geral, por exemplo, se o oponente sempre jogasse certo, exceto em 1 canto, então usar simetrias significaria que você nunca tiraria vantagem dessa informação. Isso significa que posições simetricamente equivalentes nem sempre têm o mesmo valor em um jogo multijogador
```
