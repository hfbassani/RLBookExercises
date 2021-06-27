### *Exercise 2.2: Bandit example*

**Consider a k-armed bandit problem with k = 4 actions, denoted 1, 2, 3, and 4. Consider applying to this problem a bandit algorithm using "-greedy action selection, sample-average action-value estimates, and initial estimates of Q1(a) = 0, for all a. Suppose the initial sequence of actions and rewards is A1 = 1, R1 = -1, A2 = 2, R2 = 1, A3 = 2, R3 = -2, A4 = 2, R4 = 2, A5 = 3, R5 = 0. On some of these time steps the ε case may have occurred, causing an action to be selected at random. On which time steps did this definitely occur? On which time steps could this possibly have occurred?**

---
Resposta 1:

```
Foram executadas 5 ações, o que provoca 5 estados (s1, s2, s3, s4, s5), para cada time step temos as seguintes qualidades das ações (Q), considerando a equanção Action-Value, apenas ações com Q diferente de 0:
        A1  A2    A3  A4  A5
    - 1: 0, 0,    0,  0,  0
    - 2: 1, 0,    0,  0,  0
    - 3: 1, 1,    0,  0,  0
    - 4: 1, 1.5,  0,  0,  0
    - 5: 1, 1.67, 0,  0,  0

Analisando cada momento individualmente, no que diz respeito a ação ε:
    - 1: Inicialmente todos os Qs são 0, a escolha da ação a1 pode ter sido escolhida ε ou 1 - ε.
    - 2: A ação a2 foi escolhida aqui, só pode ter sido aleatoriamente, visto que Q(A1) é o maior valor.
    - 3: Aqui, as ações a1 e a2 possuem Q iguais, e novamente a ação a2 foi escolhida, o que pode ter sido escolhido ε ou 1 - ε.
    - 4: Q(a2) é o maior valor, 1.5, pode ter sido a escolha gulosa (maior valor) ou aleátoria também (todas as ações têm a mesma probabilidade de serem escolhidas).
    - 5: Nesse caso, Q(a2) é o maior valor, 1.67, e foi escolhida a ação a3, o que demostra que foi aleatória, pois a ação gulosa, a2, não foi escolhida.

Portanto, nos time steps 2 e 5, as ações foram escolhidas de forma aleátoria (ε), enquanto que no restante pode ter sido ε ou 1 - ε.
```

---
Resposta 2:

```
Primeira iteração = não temos certeza se a ação 1 foi escolhida aleatoriamente ou se foi por padrão (Ex: Se Q1(a) = 0 para todos os a, então a primeira ação deve ser escolhida)

Segunda iteração = Foi exploração, já que a greedy action era a primeira ação

Terceira iteração = Empate entre a primeira e segunda ação. Não temos certeza se foi uma escolha aleatória entre as duas ou se foi por padrão (Ex: Entre um empate, escolher a mais recente)

Quarta iteração = Greedy action

Quinta iteração = Foi exploração, já que a greedy action era a segunda ação
```

---
Resposta 3:

```
Valoração dos estados S1 = 0, S2 = 0, S3 = 0, S4 = 0 ----> Ação tomada = 1
No primeiro passo é possivel que tenha sido uma ação 'e' afinal todos os estados tinha valoração igual a zero

Valoração dos estados S1 = -1, S2 = 0, S3 = 0, S4 = 0 ----> Ação tomada = 2
No segundo passo é possivel que tenha sido uma ação 'e' pois  a melhor ação poderia ser S2, S3 ou S4

Valoração dos estados S1 = -1, S2 = 1, S3 = 0, S4 = 0 ----> Ação tomada = 2
No terceiro passo é possivel que tenha sido uma ação 'e' pois  a melhor ação é 2

Valoração dos estados S1 = -1, S2 = -0,5, S3 = 0, S4 = 0 ----> Ação tomada = 2
No quarto passo é usado uma ação 'e' pois  a melhor ação poderia ser 3 ou 4

Valoração dos estados S1 = -1, S2 = 1/3, S3 = 0, S4 = 0 ----> Ação tomada = 3
No quinto passo é usado uma ação 'e' pois  a melhor ação é 2
```
Resposta 4:

```
Sem o conhecimento do caso em que se encontra, podemos calcular os valores esperados para as ações 1 e 2 como:
- E[a=1] = 0,1*0,5 + 0,9*0,5 = 0,5
- E[a=2] = 0,2*0,5 + 0,8*0,5 = 0,5

Assim, o melhor comportamento a se adotar, neste caso, seria escolher as ações aleatoriamente, pois ambas devem convergir para obter a mesma qualidade Qt(a)

Já no caso em que se tem conhecimento do caso atual (A ou B), pode-se considerar um valor esperado para cada situação, ou seja:
- E[a=1|s=A] = 0,1
- E[a=2|s=A] = 0,2  =>  E[s=A] = P(a=2|s=A)*0,2+P(a=1|s=A)*0,1  =>  E[s=A] é maximizado quando o agente opta sempre pela ação 2
- E[a=1|s=B] = 0,9
- E[a=2|s=B] = 0,8  =>  Da mesma forma, E[s=B] é maximizado quando o agente opta sempre pela opção 1

Assim, E[a|s] = 0,5*(P(a=2|s=A)*0,2+P(a=1|s=A)*0,1) + 0,5*(P(a=1|s=B)*0,9+P(a=2|s=B)*0,8) = 0,5*0,2 + 0,5*0,9 = 0,55

Tendo conhecimento do seu estado atual, o agente pode reconhecer os valores de suas ações nos diferentes estados e buscar aquelas que dão um maior retorno.


```
