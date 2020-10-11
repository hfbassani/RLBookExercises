### Q: What are the equations analogous to (4.3), (4.4), and (4.5), but for actionvalue functions instead of state-value functions?

#### Equação 4.3
```
qπ(s,a) = Eπ[Rt+1 + γvπ(St+1) | St = s, At = a]
```

#### Equação 4.4 e 4.5
```
qπ(s,a) = Σp(s', r | s, a)[r + γvπ(s')]
Σ para todo s', r.
```