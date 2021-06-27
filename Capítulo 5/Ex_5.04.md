### *Exercise 5.4:*

**The pseudocode for Monte Carlo ES is inecient because, for each state–action pair, it maintains a list of all returns and repeatedly calculates their mean. It would be more ecient to use techniques similar to those explained in Section 2.4 to maintain just the mean and a count (for each state–action pair) and update them incrementally. Describe how the pseudocode would be altered to achieve this.**

---
Resposta 1:

```
1) Na nicialização não será necessária a criação da list de retornos, pois será utilizada apenas uma variável para computar a média.

2) No início do loop (para cada episódio), será reatribuído o valor 0 para a média dos retornos:
ReturnsAvg <- 0

3) Para cada passo do episódio, após a atribuição do valor da recompensa acumulada, será computado o novo valor da média da recompensa acumulada:
ReturnsAvg <- (ReturnsAvg*(T-t+1)+G)/(T-t)

4) Os valores de G não serão mais armazenados em Returns(St, At) e Q(St,At) <- ReturnsAvg

```
