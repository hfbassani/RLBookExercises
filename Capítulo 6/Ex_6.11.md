### *Exercise 6.11:*

**Why is Q-learning considered an off-policy control method? **

---
Resposta 1:

```
o Q-learning é considerado off-policy porque ele aprende a função de valor ótima independentemente da política que é de fato seguida.

Compare, por exemplo, com o Sarsa. O agente que aprende via Sarsa precisa seguir a política que está sendo aprendida, já que a atualização do Sarsa depende da escolha de uma próxima ação (A', no pseudocódigo do livro) para estimar o valor Q(S', A') do estado seguinte. Se a ação tomada não viesse da política que está sendo seguida (e se tomasse, por exemplo, B), haveria uma separação entre o valor real do estado-ação seguinte (dependente da ação tomada B) e o valor do estado-ação utilizado no passo de atualização (depedente da ação A' da política), inviabilizando o aprendizado.
Já o Q-learning estima o valor do par estado-ação seguinte sem considerar a ação que de fato será realizada. Em vez disso, ele se baseia na melhor ação disponível seguindo a própria função Q. **Em outras palavras, na hora de estimar o valor do par estado-ação do próximo estado, o algoritmo Q-learning não se baseia na ação que será efetivamente tomada**, mas na ação que seria tomada se fosse seguida a política gulosa. Assim, o agente que aprende via Q-learning pode seguir qualquer outra política diferente da que é de fato aprendida (contanto que ela siga o requisito mínimo de explorar completamente o espaço estado-ação)
```
