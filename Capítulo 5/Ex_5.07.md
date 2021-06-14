### *Exercise 5.7:*

**In learning curves such as those shown in Figure 5.3 error generally decreases with training, as indeed happened for the ordinary importance-sampling method. But for the weighted importance-sampling method error first increased and then decreased. Why do you think this happened?**

---
Resposta 1:

```
Algumas coisas precisam ser esclarecidas, primeiro é que por ser divida pelos episódios a média ordinária tende a ter uma maior variância nas informações, um dos motivos para se ter um grande valor de erro inicial, entretanto ela não é enviesada, segundo fato importante é que a média ponderada
é enviesada pelo fator de p(t)-1 e por consequência não tem uma grande variância nos resultados, o pico no gráfico nos estágios iniciais pode ser influência do valor de G(t), que apresenta valores altos e conforme o tempo passa ele começa a ficar menor. Como os valores de cima e baixo são iguais podemos 
cancelar esses fatores e deixar apenas o valor de G(t).
```
