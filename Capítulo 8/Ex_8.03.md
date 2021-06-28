### *Exercise 8.3:*

**Careful inspection of Figure 8.5 reveals that the difference between Dyna-Q+ and Dyna-Q narrowed slightly over the first part of the experiment. What is the reason for this?**

---
Resposta 1:

```
O Dyna-Q+ encontra de uma maneira mais rápida a política ótima pela sua maior natureza exploratória, porém mesmo já possuindo a política ótima ele é forçado a continuar explorando, é por esse custo exploratório que a diferença entre Dyna-Q + e Dyna-Q vai se estreitando
```
---
Resposta 2:

```

Enquanto o foco do Dyna-Q é encontrar o melhor caminho o Dyna-Q+ tenderá a buscar outros caminhos mesmo quando já tiver encontrado o melhor isso em parte significará que ao longo do tempo o acumulo de recompensas do Dyna-Q serão as maiores, então se o problema não se alterar, não faz sentido continuar buscando caminhos alternativos, mas para esse específico caso temos um problema que se altera com o ambiente fornecendo um caminho alternativo viável. Com esse novo cenário o Dyna-Q continuará indo pelo caminho que descobriu a priori, mesmo sendo o caminho mais longo, e o Dyna-Q+ com a exploração irá ter um aumento na recompensa por encontrar um caminho menor.
```