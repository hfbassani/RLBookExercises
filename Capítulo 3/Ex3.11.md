### Q: If the current state is St, and actions are selected according to a stochastic policy π, then what is the expectation of Rt+1 in terms of π and the four-argument function p (3.2)?

```
Eπ[Rt+1 | St = s] = Σ[π(a|s) * p(s', r | s, a) * r], para todo s' ∈ S, a ∈ A(s)
```
