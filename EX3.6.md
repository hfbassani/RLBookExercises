Exercise 3.6 Suppose you treated pole-balancing as an episodic task but also used
discounting, with all rewards zero except for 1 upon failure. What then would the
return be at each time? How does this return differ from that in the discounted, continuing formulation of this task?

R =  Quando o agente se movimenta e o bastão não cai então recebe 0 de recompensa e 
quando o bastão cai recebe -1 de recompensa. Dessa forma analisando a formula do Ganho teremos:

G = R1 + y*R2 + y²R3 + y3R4 + ... + y^(K+1)*RK
como o episodio termina quando o bastao e quando nao cai recebe recompensa 0 então:
G = 0 + y*0 + y²0 + y0 + ... + y^(K+1)*-1
De modo que só iria importar o estado final daquele episodio