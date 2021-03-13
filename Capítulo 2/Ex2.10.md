Exercise 2.10 Suppose you face a 2-armed bandit task whose true action values change
randomly from time step to time step. Specifically, suppose that, for any time step,
the true values of actions 1 and 2 are respectively 10 and 20 with probability 0.5 (case
A), and 90 and 80 with probability 0.5 (case B). If you are not able to tell which case
you face at any step, what is the best expected reward you can achieve and how should
you behave to achieve it? Now suppose that on each step you are told whether you are
facing case A or case B (although you still don’t know the true action values). This is an
associative search task. What is the best expected reward you can achieve in this task,
and how should you behave to achieve it?

No caso cego com mudanças aleatórias a cada passo, a melhor recompensa absoluta será a Ação 1 no caso B mas toda vez que a Ação 1 for escolhida no caso A, 10 pontos deixarão de ser ganhos o que também é verdade nas seleções da Ação 2, logo como a probabilidade é 0.5 para qualquer um dos casos, dados passos suficientes qualquer um dos métodos terá a mesma recompensa total.

Já quando o caso é conhecido, primeiro deve ser feita uma exploração que irá definir os valores da ações para caso ativo e assim fazer uma escolha gananciosa quando as 4 combinações forem encontradas.
