### *Exercise 6.6:*

**In Example 6.2 we stated that the true values for the random walk example are 1/6, 2/6, 3/6, 4/6, and 5/6, for states A through E. Describe at least two different ways
that these could have been computed. Which would you guess we actually used? Why?**
---
Resposta 1:

```
1) Os valores poderiam ser obtidos através de aprendizagem de máquinas, utilizando um algoritmo TD(0), por exemplo, 
como demonstrado no próprio Ex. 6.2, que compara a convergência de diferentes implementações com diferentes valores para os parâmetros α, ou;

2) Como os valores de cada estado podem ser dados pela probabilidade de obter recompensa 1 a partir daquele estado, ou seja, de finalizar o episódio no estado terminal 
da direita e, a cada passo, as probabilidades de se mover para a direita ou esquerda são iguais, podemos computar V(s) da seguinte forma:
V(E) = p(s=T,r=1|E) = 0,5 + 0,5*p(s=T,r=1|D)
V(D) = p(s=T,r=1|D) = 0,5*(p(s=T,r=1|E) + p(s=T,r=1|C))
V(C) = p(s=T,r=1|C) = 0,5*(p(s=T,r=1|D) + p(s=T,r=1|B))
V(B) = p(s=T,r=1|B) = 0,5*p(s=T,r=1|A)
V(A) = p(s=T,r=1|A)

Denotando p(s=T,r=1|E) por p1(E) e assim por diante, apenas por simplificação, a partir das equações acima temos:
p1(B) = 2*p1(A)
p1(C) = 3*p1(A)
p1(D) = 4*p1(A)
p1(E) = 5*p1(A)

De forma análoga podemos computar as probabilidades p(s=T,r=0|X) e denotá-las por p2(X):
p2(D) = 2*p2(E)
p2(C) = 3*p2(E)
p2(B) = 4*p2(E)
p2(A) = 5*p2(E)

Porém, para qualquer estado X, temos que p(s=T,r=1|X) + p(s=T,r=0|X) = 1, logo:
p(s=T,r=1|E) + p(s=T,r=0|E) = p1(E) + p2(E) = 5*p1(A) + 1/5*(1-p1(A)) = 1
=> 25*p1(A) + 1 - p1(A) = 5 => 24*p1(A) = 4 => p1(A) = 1/6

Consequentemente: p1(B) = 2/6, p1(C) = 3/6, p1(D) = 4/6 e p1(E) = 5/6

```
