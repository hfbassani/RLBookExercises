### *Exercise 3.1:*

**Devise three example tasks of your own that fit into the MDP framework, identifying for each its states, actions, and rewards. Make the three examples as different from each other as possible. The framework is abstract and flexible and can be applied in many different ways. Stretch its limits in some way in at least one of your examples.**

---
Resposta 1:

```
* Exemplo 1:
Em um jogo de Xadrez, a próxima ação depende apenas da disposição das peças nos tabuleiros. Em uma MDP o estado é a disposição das peças no tabuleiro, a ação é o movimento que o agente realiza a partir de uma das peças, a recompensa é dada ao fim do turno do adversário e é atribuída a partir da diferença entre pontuação conseguida através da conquista de peças e a pontuação cedida ao adversário a partir da perda de peças.

* Exemplo 2:

* Exemplo 3:
```


---
Resposta 2:

```
* Exemplo 1:
A tarefa de melhoramento de rota de limpeza de robô aspirador de pó inteligente que sabe determinar sua posição no ambiente por reforço. As recompensas da tarefa são de 1 para toda ação tomada, -1 para ações tomadas que levem a um estado visitado e 0 para o objetivo atingido. O ambiente é uma sala de 16m² que contém móveis que modificam as rotas do aspirador. As ações desta tarefa se baseiam em mover-se para frente, para trás, esquerda e direita com chances equiprováveis. Quando uma ação é escolhida ela tem 1 de ocorrer.

* Exemplo 2:
Tarefa de recomendação de filmes para usuários, onde o ambiente é um streaming de filmes e séries, as suas ações são tomadas com base nas características de filmes assistidos e avaliados pelo usuário, e a recompensa se dar com base no filme assistido e na avaliação dada pelo usuário, sendo penalizado por filmes que for mal avaliado ou não assistido.

* Exemplo 3:
[1] realizou em seu trabalho uma tentativa de reconfiguração autónoma de parâmetros em sistemas web multicamadas em ambientes que eram dinâmicos e baseados em VM 's. O processo foi formulado como um espaço de estados sendo a configuração do sistema, as ações eram {aumentar, diminuir, manter} para cada parâmetro e a recompensa definida como diferença entre o tempo de resposta determinando qual tempo iria ser mantido.

[1] BU, Xiangping; RAO, Jia; XU, Cheng-Zhong. A reinforcement learning approach to online web systems auto-configuration. In: 2009 29th IEEE International Conference on Distributed Computing Systems. IEEE, 2009. p. 2-11.
```
