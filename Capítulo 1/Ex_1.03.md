### *Exercise 1.3: Symmetries*

**Suppose the reinforcement learning player was greedy, that is, it always played the move that brought it to the position that it rated the best. Might it learn to play better, or worse, than a nongreedy player? What problems might occur?**

---
Resposta 1:

```
Ele aprenderá pior, o grande problema de apenas selecionar os melhores lances, baseado no que ele sabe até o momento, é que tal comportamento reforça o caminhamento apenas pelas possibilidades já conhecidas que melhor performaram até então. Logo, o player aprenderá algo novo em duas circunstâncias:

    1. Quando o adversário conduzir o jogo para uma posição que o player desconhece, ou seja, ele terá que jogar algo "novo", ou;
    2. Quando um caminho já reforçado, que possuí o melhor valor, sofrer a circustância 1 e sua pontuação se tornar inferior, ocasionado pela descoberta de novas possibilidades que resultam em resultados ruins.
    
Desconsiderando tais casos, o player estará caminhando através daquelas possibilidades já conhecidas que são consideradas boas, isso limita o potencial de descoberta, fazendo com que possíveis jogadas mais promissoras não sejam, ou com muita dificuldade, descobertas. Além disso, as novas possibilidades causadas pelas jogadas do **adversário** podem estar conduzindo para derrotas constantes, sendo assim o aprendizado além de ineficiente pode não ser muito proveitoso.
```

---
Resposta 2:

```
Acredito que iria depender de quanto "conhecimento" o algoritmo já acumula, imaginando um algoritmo que no contexto de jogo da velha o mesmo se torna invencível, em que no pior dos casos um empate vai acontecer. Mas diria que pior, se o objetivo é aprender a jogar melhor, o "greedy player" não vai explorar novas possibilidades com determinada frequência, em contrapartida, o "nongredy player" pode não ter as melhores recompensas, mas vai explorar novas possibilidades com muito mais frequência que o jogador ganancioso, dessa forma o aprendizado, acredito que, é considerado melhor para o "nongreedy player". 
```

---
Resposta 3:

```
Neste caso o algoritmo aprenderia com ele mesmo qual seria a melhor jogada para um determinado estado, porém poderia ocorrer um certo bias devido ao inimigo sempre repetir algum determinado passo acreditando que aquele movimento seria o melhor movimento para o estado, porém ao jogar com um ser humano o oponente poderia realizar uma jogada 'blafer' para confundir o algoritmo e assim o ser humano poderia tirar vantagem sobre o jogo.
```
