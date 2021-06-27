Algoritmo: off-policy TD(0)
Parametros: a(alpha), politica b
Inicializar V(s) para todo estado S!=Terminal

Loop para cada episodio:
    S <- estado inicial
    Loop para cada passo:
        A <- ação da politica b(s) 
        realize ação A -> (R, S')
        V(S) <- V(S) + a*(pi(A|S)/b(A|S))*[R + yV(S') - V(S)]
        S <- S'
    Até S==Terminal