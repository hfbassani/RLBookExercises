### *Exercise 2.8: UCB Spykes*

**In Figure 2.4 the UCB algorithm shows a distinct spike in performance on the 11th step. Why is this? Note that for your answer to be fully satisfactory it must explain both why the reward increases on the 11th step and why it decreases on the subsequent steps. Hint: If c = 1, then the spike is less prominent.**
---
Resposta 1:

```
Primeiro é preciso ressaltar que o agente vai tentar todos os 10 braços nos 10 primeiros passos, uma vez que Nt(a) é inicialmente 0 para todas as ações, logo, todas são consideradas "maximizadoras" e serão testadas. 
No passo 11, ele já vai ter o primeiro valor de cada ação, e priorizará a ação com o maior ganhor (argmax). Já no 12º passo, por ele ter escolhido a melhor ação já 2 vezes, o valor de Nt(a) pra melhor ação vai ser maior,
fazendo com que o termo da raiz multiplicada por c (c, que nesse caso é 2) fique menor, o que por sua vez, faz com que a melhor ação dependa mais do valor de Qt(a). O resultado é a escolha de uma ação com um ganho menor, visto que
todas as outras foram escolhidas apenas uma vez (o valor da raiz será maior para essas, do que no caso da ação que foi escolhida 2 vezes, visto que a divisão dentro da raiz será exatamente igual a ln(t), uma vez que Nt(a) é 1 para todas
as ações != da escolhida no passo 11, e isso é itensificado por c, que dobra o valor da raiz, fazendo com que o ganho estimado dessas ações na visão do agente, seja dependente tanto do ganho real, quanto do termo da raiz multiplicada por c).
Concluindo: O spike ocorre pois a melhor ação é escolhida e o ganho é maximizado, e o decaimento ocorre pois uma ação não tão boa é escolhida logo em seguida devido ao Nt(a) menor. 
```