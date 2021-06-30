### *Exercise 3.2:*

**Is the MDP framework adequate to usefully represent all goal-directed learning tasks? Can you think of any clear exceptions?**

---
Resposta 1:

```
Um caso onde eu acredito que não seja adequado a utilização o MDP é quando nos deparamos com um conjunto de estados e/ou conjunto de ações infinitas, como também se as informações da sequência estiverem incompleta ou até mesmo indisponíveis, outro caso é quando os estados são difíceis de compreender ou não é possivel representar-los numericamente.
```

---
Resposta 2:

```
MDP não é adequado em diversos cenários como por exemplo jogo de Xadrez onde o oponente apresenta centenas de jogadas com probabilidade não definida. Jogo de futebol de robôs apresentam diversos estados e probabilidade nao definida quando tomamos uma determinada ação.
```

---
Resposta 3:

```
Qualquer cenário que não haja o acesso a todas as probabilidades de transições ou que o ambiente não seja estacionário (ou seja, mude ao longo da execução), não pode ser representado pelos MDPs. Um exemplo claro é um cenário com multiplos agentes, cada um interage e "modifica" o ambiente, tornando-o não estacionário, o que muda as probabilidades de forma imprevisivel.
```
