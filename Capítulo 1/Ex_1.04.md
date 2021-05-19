### *Exercise 1.4: Learning from Exploration*

**Suppose learning updates occurred after all moves, including exploratory moves. If the step-size parameter is appropriately reduced over time (but not the tendency to explore), then the state values would converge to a different set of probabilities. What (conceptually) are the two sets of probabilities computed when we do, and when we do not, learn from exploratory moves? Assuming that we do continue to make exploratory moves, which set of probabilities might be better to learn? Which would result in more wins?**

---
Resposta 1:

```
Para movimentos exploratórios, o conjunto de probabilidades seguiria a política "não gananciosa", não escolhendo os movimentos com maiores valor, enquanto para movimentos não exploratórios seria o que segue a "gananciosa". Realizando apenas movimentos gananciosos, é possível que o agente foque em movimentos que são muitos bons, já que prioriza os ganhos imediatos, enquanto movimentos não gananciosos também visa maximizar as recompensas no longo prazo. Explorando outros movimentos, o agente pode encontrar novas jogadas promissoras que podem ser as melhores e com isso, maximizar as recompensas. Realizar movimentos exploratórios pode resultar em desempenho melhor, levando em consideração que o resultado da abordagem gananciosa pode ser enviesada, logo, o desempenho do aprendizado com movimentos exploratórios é no mínimo tão ruim quanto que a outra abordagem, já que se uma ação, que foi escolhida na exploração, for melhor que a ganancioasa, seu valor será atualizado. Entretanto, o ideal é equilibrar as abordagens, um momento utilizando movimentos exploratórios e em outro movimentos gananciosos, que busca maximixar o resultado daquela ação.
```
