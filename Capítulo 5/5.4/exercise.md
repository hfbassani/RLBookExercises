Exercise 5.4 The pseudocode for Monte Carlo ES is inefficient because, for each state– action pair, it maintains a list of all returns and repeatedly calculates their mean. It would be more efficient to use techniques similar to those explained in Section 2.4 to maintain just the mean and a count (for each state–action pair) and update them incrementally. Describe how the pseudocode would be altered to achieve this.

    Para melhorar a eficência do algoritmo MC Exploring Starts, guardando apenas a média atual e a quantidade (para cada par estado-ação), o pseudo-código deveria ser alterado da seguinte forma:
        1) Remover as linhas que guardam os retornos para cada par estado-ação;
        2) Guardar a quantidade para cada par estado-ação e calcular a média com esse valor, ou seja:
            Para cada par estado-ação (s,a):
            ```
            qtd(s,a)++, para cada par estado-ação
            Q(s,a)  <-- (Q(s,a) * (qtd(s,a) - 1)) + G / qtd(s,a)
            ```

            Disclaimer:
                Na primeira opção, o valor inicial de Q(s,a) será zerado, visto que q(s,a) - 1 = 0, o que fará que o algoritmo leve em consideração apenas o valor de G (recompensa acumulada)na primeira iteração. Notei que no algoritmo do livro, isso também é feito.

            Lembrando que é necessário inicializar esses valores no início do algoritmo:
                ```
                qtd(s,a) <-- 0
                ```