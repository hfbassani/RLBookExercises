### *Exercise 6.2:*

**This is an exercise to help develop your intuition about why TD methods are often more ecient than Monte Carlo methods. Consider the driving home example and how it is addressed by TD and Monte Carlo methods. Can you imagine a scenario in which a TD update would be better on average than a Monte Carlo update? Give an example scenario—a description of past experience and a current state—in which you would expect the TD update to be better. Here’s a hint: Suppose you have lots of experience driving home from work. Then you move to a new building and a new parking lot (but you still enter the highway at the same place). Now you are starting to learn predictions for the new building. Can you see why TD updates are likely to be much better, at least initially, in this case? Might the same sort of thing happen in the original scenario?**

---
Resposta 1:

```
O método TD pode usar predições do inicio ao fim de experiências passadas. Já o método MC precisa criar predições. Dessa forma, é provável que as predições de MC sejam diferentes da realidade e por isso, o método TD é melhor nesse caso
```
