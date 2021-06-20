### *Exercise 6.2:*

**This is an exercise to help develop your intuition about why TD methods are often more eficient than Monte Carlo methods. Consider the driving home example and how it is addressed by TD and Monte Carlo methods. Can you imagine a scenario in which a TD update would be better on average than a Monte Carlo update? Give an example scenario—a description of past experience and a current state—in which you would expect the TD update to be better. Here’s a hint: Suppose you have lots of experience driving home from work. Then you move to a new building and a new parking lot (but you still enter the highway at the same place). Now you are starting to learn predictions for the new building. Can you see why TD updates are likely to be much better, at least initially, in this case? Might the same sort of thing happen in the original scenario?**

---
Resposta 1:

```
Como resultado das experiências anteriores é possível que o cálculo do tempo restante é preciso, o método TD tem uma vantagem, pelo menos inicial, sobre o método Monte Carlo por conseguir fazer mudanças ao ponto de um passo e sem a demora de ter que terminar o episódio, característica de Monte Carlo, essa atualização que TD proporciona faz com que se tenha uma prévia de como está a qualidade no momento atual e é possível fazer uma projeção de como ficará.
```
