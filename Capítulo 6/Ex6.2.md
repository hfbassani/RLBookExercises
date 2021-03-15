Exercise 6.2 This is an exercise to help develop your intuition about why TD methods
are often more efficient than Monte Carlo methods. Consider the driving home example
and how it is addressed by TD and Monte Carlo methods. Can you imagine a scenario
in which a TD update would be better on average than a Monte Carlo update? Give
an example scenario—a description of past experience and a current state—in which
you would expect the TD update to be better. Here’s a hint: Suppose you have lots
of experience driving home from work. Then you move to a new building and a new
parking lot (but you still enter the highway at the same place). Now you are starting
to learn predictions for the new building. Can you see why TD updates are likely to be
much better, at least initially, in this case? Might the same sort of thing happen in the
original scenario?

Tomando o exemplo da comutação Casa-Trabalho, no caso de Monte Carlo, se uma mudança na rota fosse feita só iríamos receber uma previsão depois da primeira vez que todo o caminho tivesse sido realizado. Enquanto no caso de TD, assim que o trecho Novo Prédio-Rodovia fosse completado, iríamos receber uma nova previsão usando o tempo gasto atual mais o tempo para este trecho restante obtido anteriormente.

E mesmo no cenário original poderemos ver melhoras possíveis pela utilização de TD, como em casos de condições adversas em que certos trechos podem ter atrasos mas a estimativa para o resto do trecho ainda pode ser usada para dar um previsão semi-precisa.