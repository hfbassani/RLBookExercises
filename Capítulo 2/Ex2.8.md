Exercise 2.8: Suppose you face a 2-armed bandit task whose true action values change randomly from time step to time step. Specifically, suppose that, for any time step, the true values of actions 1 and 2 are respectively 0.1 and 0.2 with probability 0.5 (case A), and 0.9 and 0.8 with probability 0.5 (case B). If you are not able to tell which case you face at any step, what is the best expectation of success you can achieve and how should you behave to achieve it? Now suppose that on each step you are told whether you are facing case A or case B (although you still don’t know the true action values). This is an associative search task. What is the best expectation of success you can achieve in this task, and how should you behave to achieve it?

    No primeiro caso não é conhecido o caso que está sendo tratado, a melhor solução é escolher a opção que possua a melhor estimativa de valor em combinação. Entretando eles possuem valores iguais:
    
   A<sub>1 = 0.5 * 0.1 + 0.5 * 0.9 = 0.5

   A<sub>2 = 0.5 * 0.2 + 0.5 * 0.8 = 0.5
    
    Portando a melhor expectativa de sucesso é 0.5 e o comportamento que se deve adotar é escolher aleatóriamente uma ação em cada etapa.
    
    No segundo caso é informado previamente o caso a ser enfrentado, portanto nós tratamos eles como problemas independentes, explorando os mesmos para assim podermos aprender a melhor ação para cada um. A melhor expectativa de sucesso é 0.55:
    
   0.2 * 0.5 + 0.9 * 0.5 = 0.55
    
    
    

    
