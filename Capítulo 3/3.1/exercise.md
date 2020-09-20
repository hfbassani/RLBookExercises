Exercise 3.1 Devise three example tasks of your own that fit into the MDP framework, identifying for each its states, actions, and rewards. Make the three examples as different from each other as possible. The framework is abstract and flexible and can be applied in many di↵erent ways. Stretch its limits in some way in at least one of your examples.

    1) Jogo de Xadrez
        - Estados: posição das peças (adversáro e agente) no tabuleiro em cada tempo t.
        - Ações: movimentos disponíveis para cada peça durante cada estado do jogo.
        - Recompensas: resultado final do jogo (vitória ou derrota), também jogadas durante a partida que tiveram influência importante no resultado final (ex. Eliminar a rainha adversária).

    2) Decisão de compra ou venda de ações
        - Estados: resultados do mercado como um todo (subindo ou descendo) no tempo t, e dos ativos que o agente possui
        - Ações: comprar ou vender as ações, aumentar ou diminuir posição em alguma ação
        - Recompensas: lucro ou Prejuízo ao final da operação

    3) Carro autônomo
        - Estados: visão, radares, informações do sensores sobre a estrada (placas, faixas, etc).
        - Ações: freiar, acelerar, direção e parar.
        - Recompensas: chegada no destino, tempo para chegar no destino, acidentes evitados.