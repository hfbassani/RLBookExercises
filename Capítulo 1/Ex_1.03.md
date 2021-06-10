### *Exercise 1.3: Symmetries*

**Suppose the reinforcement learning player was greedy, that is, it always played the move that brought it to the position that it rated the best. Might it learn to play better, or worse, than a nongreedy player? What problems might occur?**

---
Resposta 1.03:

```
Na suposição de que um jogador seja sempre greedy, ocorre que esse jogador não conseguirá alcançar uma boa recompensa cumulativa, pois não explora suficientemente outras possibilidades. Um jogador greedy irá conseguir ganhar de um nongreedy, 
entretanto se o jogador passar de nongreedy para gradual greedy, o jogador greedy ganhará inicialmente, mas com o passar do tempo o gradual greedy passará a ser melhor que o greedy, pois consegue explorar as melhores ações ao contrário do greedy que sempre
seguirá um caminho. 
```

