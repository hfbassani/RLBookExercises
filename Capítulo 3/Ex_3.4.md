### *Exercise 3.4:* 

**Give a table analogous to that in Example 3.3, but for p(s0, r|s, a). It should have columns for s, a, s0, r, and p(s0, r|s, a), and a row for every 4-tuple for which p(s0, r|s, a) > 0**

---
Resposta 1:

```
Denotando as recompensas Rsearch e Rwait por 'rs' e rw', respectivamente:

|   s  |     a    |  s'  |  r | p(s',r\|s,a) |
|:----:|:--------:|:----:|:--:|:------------:|
| High |  Search  | High | rs |      α       |
| High |  Search  |  Low | rs |     1-α      |
| High |   Wait   | High | rw |      1       |
|  Low |  Search  | High | -3 |     1-β      |
|  Low |  Search  |  Low | rs |      β       |
|  Low |   Wait   |  Low | rw |      1       |
|  Low | Recharge | High |  0 |      1       |

```
