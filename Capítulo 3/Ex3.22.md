### Q: Consider the continuing MDP shown to the right. The only decision to be made is that in the top state, where two actions are available, left and right. The numbers show the rewards that are received deterministically after each action. There are exactly two deterministic policies, πleft and πright. What policy is optimal if γ = 0? If γ = 0.9? If γ = 0.5?


```
Para γ = 0:
vπleft(left) = 1 + γ * 0 = 1 + 0 * 0 = 1
vπright(right) = 0 + γ * 2 = 0 + 0 * 2 = 0

A política ótima para γ = 0 é vπleft.

Para γ = 0.9:
vπleft(left) = 1 + γ * 0 = 1 + 0.9 * 0 = 1
vπright(right) = 0 + γ * 2 = 0 + 0.9 * 2 = 1.8

A política ótima para γ = 0.9 é vπright.

Para γ = 0.5:
vπleft(left) = 1 + γ * 0 = 1 + 0.5 * 0 = 1
vπright(right) = 0 + γ * 2 = 0 + 0.5 * 2 = 1

Para γ = 0.5, tanto vπleft quanto vπright são políticas ótimas.
```
