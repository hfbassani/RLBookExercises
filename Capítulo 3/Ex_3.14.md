### *Exercise 3.14:*

**The Bellman equation (3.14) must hold for each state for the value function vπ shown in Figure 3.2 (right) of Example 3.5. Show numerically that this equation holds for the center state, valued at +0.7, with respect to its four neighboring states, valued at +2.3, +0.4, -0.4, and +0.7. (These numbers are accurate only to one decimal place.)**

---
Resposta 1:

```
0.25 * (0 + 0.9 * 2.3) + 0.25 * (0 + 0.9 * 0,4) + 0.25 * (0 - 0.9 * 0.4) + 0.25 * (0 + 0.9 * 0.7)

= 0.5175 + 0.09 - 0.09 + 0.1575 = 0.675

Arredondando para uma casa decimal ≅ 0.7
```
