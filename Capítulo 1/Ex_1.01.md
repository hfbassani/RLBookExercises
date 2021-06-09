### *Exercise 1.1: Self-Play*

**Suppose, instead of playing against a random opponent, the reinforcement learning algorithm described above played against itself, with both sides learning. What do you think would happen in this case? Would it learn a different policy for selecting moves?**


---
Resposta 1.1 (Alternativa):

```
Na suposição de que dois 'jogadores/algoritmos' joguem com as mesmas policies eles não irão aprender a mesma policy de forma geral, pois um jogador está tentando obter otimizar a recompensa contra um oponente específico, sendo assim caso o adversário mude a policy também irá mudar. É importante considerar que se ambos jogadores não são imperfeitos, eles irão buscar os melhores movimentos para si, desta maneira eles irão alcançar o chamado equilíbrio Nash. De acordo com Bowling and Veloso (2001) a única estratégia que os jogadores irão assumir é a do equilíbrio Nash, pois é o único perfil de estratégia possível que agentes racionais  podem convergir em jogos contra si
```