Exercise 2.6: Mysterious Spikes The results shown in Figure 2.3 should be quite reliable
because they are averages over 2000 individual, randomly chosen 10-armed bandit tasks.
Why, then, are there oscillations and spikes in the early part of the curve for the optimistic
method? In other words, what might make this method perform particularly better or
worse, on average, on particular early steps?

Quando utilizamos valores otimistas inicialmente, teremos uma maior exploração no começo e essa exploração pode causar esses "spikes" no gráfico. Acredito que ele será pior, nos passos iniciais, quando houver uma grande discrepância entre os resultados médios/bons em relação aos péssimos; Para ele ser melhor nos passos iniciais, acredito que a maioria dos resultados devem ser bons, mas poucos ótimos.
