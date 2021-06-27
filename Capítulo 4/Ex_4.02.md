### *Exercise 4.2:*

**In Example 4.1, suppose a new state 15 is added to the gridworld just below state 13, and its actions, left, up, right, and down, take the agent to states 12, 13, 14, and 15, respectively. Assume that the transitions from the original states are unchanged. What, then, is vπ(15) for the equiprobable random policy? Now suppose the dynamics of state 13 are also changed, such that action down from state 13 takes the agent to the new state 15. What is vπ(15) for the equiprobable random policy in this case?**

---
Resposta 1:

```
Para esta politica equiprovavel o vπ(15) é um estado inexplorado e inalcançavel pois se para este primeiro ponto o vπ(15) não pode ser alcançado pelo estado 13 então, o vπ(15) não pode ser computado. Com a alteração do estado 13 agora com a ação down indo ao 15 então este estado torna-se mais um dos estados conhecido do agente. E assim sua politica poderá ser calculada.
```
