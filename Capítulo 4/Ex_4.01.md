### *Exercise 4.1:*

**In Example 4.1, if π  is the equiprobable random policy, what is qπ(11, down)? What is qπ(7, down)?**

---
Resposta 1:

```
Ao executar o policy evaluation chegamos numa função estado-valor como mostrado na Figura 4.1 (k = ∞). Portanto:

    qπ(11, down) = R11-T + vπ(T) = -1 + 0 = -1
    qπ(7, down) = R7-11 + vπ(11) = -1 + -14 = -15
```