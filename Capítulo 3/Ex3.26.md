Exercise 3.26 Give an equation for q* in terms of v*.

q𝜋(s) é a função de estado ação dado uma política 𝜋

q𝜋(s, a)  = E𝜋[Gt | St =s, At = a]

v𝜋(s) é a função de estado valor dado uma política 𝜋

v𝜋(s) = E𝜋[Gt | St =s]

q* é a função de estado ação que segue a política ótima e pode ser denotada por q*(s, a)  = max  q𝜋(s, a),

(política ótima é aquela que maximiza as funções de valor)

como GT = r +ϒE𝜋[Gt+1|St+1 =s’], então:

Gt = [r + ϒv𝜋(s’)]

substituindo GT em q𝜋(s, a)

q*(s, a)  = E[r + ϒv*(s’) | St =s, At = a]

como na equação (3.17) do livro

