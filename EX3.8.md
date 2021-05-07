Exercise 3.8 Suppose y = 0.5 and the following sequence of rewards is received R 1 = 1,
R 2 = 2, R 3 = 6, R 4 = 3, and R 5 = 2, with T = 5. What are G 0 , G 1 , . . ., G 5 ? Hint:
Work backwards.

Fazendo de maneira mais trabalhosa
G = R1 + y*R2 + y²R3 + y3R4 + ... + y^(K+1)*RK


G0 = -1 + 0.5*2 + 0.5²*6 + 0.5³*3 + 0,5⁴*2
G0 = 2

G1 = 2 + 0.5*6 + 0.5²*3 + 0,5³*2
G1 = 6

G2 = 6 + 0.5*3 + 0,5²*2
G2 = 8

G3 = 3 + 0,5*2
G3 = 4

G4 = 2

G5 = 0



Fazendo seguindo a dica do livro
Gt = Rt+1 + y*Gt+1

G5 = 0
G4 = 2 + 0.5*G5 = 2
G3 = 3 + 0.5*G4 = 4
G2 = 6 + 0.5*G3 = 8
G1 = 2 + 0.5*G2 = 6
G0 = -1 + 0.5*G1 = 2