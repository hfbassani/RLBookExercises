### *Exercise 2.10:* 

**Suppose you face a 2-armed bandit task whose true action values change randomly from time step to time step. Specifically, suppose that, for any time step, the true values of actions 1 and 2 are respectively 0.1 and 0.2 with probability 0.5 (case A), and 0.9 and 0.8 with probability 0.5 (case B). If you are not able to tell which case you face at any step, what is the best expectation of success you can achieve and how should you behave to achieve it? Now suppose that on each step you are told whether you are facing case A or case B (although you still don’t know the true action values). This is an associative search task. What is the best expectation of success you can achieve in this task, and how should you behave to achieve it?**

---
Resposta 1:

```
No primeiro caso não é conhecido o caso que está sendo tratado, a melhor solução é escolher a opção que possua a melhor estimativa de valor em combinação. Entretando eles possuem valores iguais:

A1 = 0.5 * 0.1 + 0.5 * 0.9 = 0.5

A2 = 0.5 * 0.2 + 0.5 * 0.8 = 0.5

Portando a melhor expectativa de sucesso é 0.5 e o comportamento que se deve adotar é escolher aleatóriamente uma ação em cada etapa.

No segundo caso é informado previamente o caso a ser enfrentado, portanto nós tratamos eles como problemas independentes, explorando os mesmos para assim podermos aprender a melhor ação para cada um. A melhor expectativa de sucesso é 0.55:

0.2 * 0.5 + 0.9 * 0.5 = 0.55
```

Resposta 2:

```
Sem o conhecimento do caso em que se encontra, podemos calcular os valores esperados para as ações 1 e 2 como:
- E[a=1] = 0,1*0,5 + 0,9*0,5 = 0,5
- E[a=2] = 0,2*0,5 + 0,8*0,5 = 0,5

Assim, o melhor comportamento a se adotar, neste caso, seria escolher as ações aleatoriamente, pois ambas devem convergir para obter a mesma qualidade Qt(a)

Já no caso em que se tem conhecimento do caso atual (A ou B), pode-se considerar um valor esperado para cada situação, ou seja:
- E[a=1|s=A] = 0,1
- E[a=2|s=A] = 0,2  =>  E[s=A] = P(a=2|s=A)*0,2+P(a=1|s=A)*0,1  =>  E[s=A] é maximizado quando o agente opta sempre pela ação 2
- E[a=1|s=B] = 0,9
- E[a=2|s=B] = 0,8  =>  Da mesma forma, E[s=B] é maximizado quando o agente opta sempre pela opção 1

Assim, E[a|s] = 0,5*(P(a=2|s=A)*0,2+P(a=1|s=A)*0,1) + 0,5*(P(a=1|s=B)*0,9+P(a=2|s=B)*0,8) = 0,5*0,2 + 0,5*0,9 = 0,55

Tendo conhecimento do seu estado atual, o agente pode reconhecer os valores de suas ações nos diferentes estados e buscar aquelas que dão um maior retorno.


```
