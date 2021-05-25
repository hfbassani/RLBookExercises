### *Exercise 8.7:*

**Some of the graphs in Figure 8.8 seem to be scalloped in their early portions, particularly the upper graph for b = 1 and the uniform distribution. Why do you think this is? What aspects of the data shown support your hypothesis?**

---
Resposta 1:

```
Estes recortes é pelo fato de levar muito tempo de computação para fazer uma varredura completa, e no caso do b=1 haverá maiores recortes, caso em que a mudança de um estado é totalmente transferida para outros estados, quantor maior o b, o sistema fica mais estabilizado devido à soma múltipla das mudanças parciais dos estados seguintes. Podemos observar que no caso de 1.000 estados, b=10 é mais suave, enquanto b=1 é mais recortado, o b=1 no caso de 10.000 estados seria mais recortado se a escala do eixo X, o tempo de computação, fossem iguais.


Obs: não sei ao certo a tradução de scalloped, eu traduzi como recortado
```
