### *Exercise 9.1:*

** Show that tabular methods such as presented in Part I of this book are a special case of linear function approximation. What would the feature vectors be?**

---
Resposta 1:

```
Os vetores de características podem ser tomados como preenchidos pelo valor 1 (um).

Por exemplo, comparando a equação 9.7 com o algoritmo tabular TD(0), U seria correspondente à recompensa observada R mais o fator de desconto gama multiplicado pelo valor do estado seguinte. A estimativa de valor do estado atual v chapéu seria correspondente ao próprio V do estado atual. E o gradiente, equivalente às features no caso linear, seria preenchido com o elemento neutro da multiplicação, 1.

Isso ocorre porque o caso tabular é como um caso trivial em que o número de pesos é igual ao de estados, assim, cada peso significa o valor de cada estado e pode ser usado diretamente.
```
