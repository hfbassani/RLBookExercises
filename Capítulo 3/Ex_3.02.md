### *Exercise 3.2:*

**Is the MDP framework adequate to usefully represent all goal-directed learning tasks? Can you think of any clear exceptions?**

---
Resposta 1:

```
Em Aprendizagem por Reforço (AR)  o problema a ser resolvido é descrito pelo Processo de Decisão de Markov - MDP. Temos que se um problema é bem descrito como MDP, então Aprendizagem por Reforço é uma boa abordagem a se seguir, de fato isso não significa que o modelo necessite ter todos estados de probabilidades 
descritos, mas apenas que eles sejam feitos ou descobertos. Caso o problema em questão não tenha um mapeamento ou se adeque ao MDP, isso indica que não há possibilidade de resultados úteis com AR. Uma das chaves para saber se AR funcionará de forma satisfatória é através da propriedade Markoviana, que o valor do estado atual
é suficiente para ajustar as próximas transições subsequentes com as devidas recompensas pelas ações tomadas. Esse processo pode ter uma falha quando o sistema de recompensas é violado e isso pode acontecer quando o sistema em questão foca em mais de um objetivo tendo que realizar tradeoffs para maximizar as recompensas, considerando
que sistemas de AR consideram focar apenas em um único objetivo. 
```


