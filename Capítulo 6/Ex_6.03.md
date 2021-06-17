### *Exercise 6.3:*

**From the results shown in the left graph of the random walk example it appears that the first episode results in a change in only V (A). What does this tell you about what happened on the first episode? Why was only the estimate for this one state changed? By exactly how much was it changed?**

---
Resposta 1:

```
Apenas o valor do estado A foi mudado, por uma quantidade igual a menos alfa, porque o episódio acabou no estado terminal à esquerda e, no TD(0), apenas o estado diretamente anterior ao estado visitado é atualizado.

Num outro episódio, os outros estados serão atualizados baseados no valor de A (por exemplo) e, assim, a informação da recompensa será propagada. Mas, como só estamos considerando o primeiro episódio, apenas o valor do estado imediatamente anterior à recompensa é atualizado.
```
