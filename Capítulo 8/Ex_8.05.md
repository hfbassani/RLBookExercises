### *Exercise 8.3:*

**How might the tabular Dyna-Q algorithm shown on page 164 be modified to handle stochastic environments? How might this modification perform poorly on changing environments such as considered in this section? How could the algorithm be modified to handle stochastic environments and changing environments?**

---
Resposta 1:

```
Vamos dividir o nosso algoritmo Dyna-Q em duas partes: planejamento e aprendizagem direta. Para aprendizagem direta, uma forma de modelar uma ambiente estocástico ainda sendo tabular é adicionar o que pode ser chamado de two-step ϵ-soft. Basicamente, a parte estocástica da política ϵ-greedy já ajuda bastante na seleção ocasional de outras ações, porém, para um ambiente verdadeiramente estocástico, isso pode não ser o suficiente. Nesse caso, podemos deixar nossa política greedy mais estocástica ao selecionar com certa chance a segunda melhor ação em vez da primeira. Note que a política ainda é gulosa, mas caso exista mais de uma opção tão boa quanto pela natureza estocástica do problema, podemos selecionar de vez em quando a segunda melhor opção, que pode se tornar a primeira. Essa política ϵ-soft pode ser aplicada para três seleções ou até mais, dependendo de quão estocástico é o ambiente.

## PSEUDO-CÓDIGO

COM CHANCE ϵ SELECIONE UMA AÇÃO ALEARÓRIA;
COM CHANCE 1 - ϵ SELECIONE:
    COM CHANCE ρ SELECIONE A AÇÃO GREEDY;
    COM CHANCE 1 - ρ SELECIONE A SEGUNDA MELHOR AÇÃO;

Na prática, para problemas reais, a resolução do problema para essa fase de aprendizagem direta é usar um método de política de gradiente que será visto no capítulo 13.

Para o planejamento, a questão é como modelar o ambiente. Uma forma de modelar o ambiente de forma tabular é basicamente fazer algo parecido com o passo de aprendizagem direta e em vez de só armazenar a ação tomada em um estado, armazenar também a probabilidade de tomar cada ação em um estado, e a média de recompensa ao tomar a ação, ou p(a|S) e R. Dessa forma, podemos marcar qual foi a última ação tomada e ao mesmo tempo ter a modelagem estocástica do ambiente. Se o ambiente for estocástico, então podemos sortear a próxima ação pelo modelo usando a estimativa de p(a|S). Uma forma de fazer essa estimativa é usar uma média móvel.

Em ambientes que mudam, a parte de aprendizagem direta com o two-step ϵ-soft não deve ter perda, ainda mais, ele deve aumentar a velocidade que o modelo muda para uma segunda abordagem, mas ao mesmo tempo faz com que o modelo performe mal em ambientes determinísticos. A parte de planejamento performaria mal em um ambiente que muda desde que a média móvel tenha um termo α grande. Se o termo α abaixo for suficientemente pequeno, estaremos esquecendo a probabilidade antiga com mais frequência e portanto o modelo se ajusta mais rápido.

p(A|S) = α * p(A|S) + (1 - α)
R = β * R + (1 - β) * r

O Algoritmo para ambientes estocásticos e ambientes que mudam seria com a aprendizagem direta de política n-step ϵ-soft e modelo tabular estocástico com uma média móvel e um α e β suficientemente pequenos para "esquecer" mais rápido as estimativas mais antigas.
```