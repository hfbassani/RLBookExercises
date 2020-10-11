### Q: Prove the second equality in (3.10).

```
Provar que para Rt = 1 e γ < 1:
    Gt = Σ(γ^k) = 1 / (1 - γ)

Por definição temos:
    Gt = Σ[(γ^k) * Rt+k+1], para k=0 até ∞

Para um MDP com recompensa constante = +1, então Rt+k+1 torna-se uma constate:
    Rt+k+1 = 1

Portanto:
    Gt = Σ[(γ^k) * 1], para k=0 até ∞

Uma das propriedades do somatório é:
    Σ(α * xi) = α * Σ(xi), para k=m até n

Ou seja, uma constante em multiplicação dentro de um somatório pode ser colocado fora do termo. Portanto:
    Gt = 1 * Σ(γ^k) = Σ(γ^k), para k=0 até ∞

O somatório acima é uma série geométrica, e possui uma igualdade conhecida:
    Σ(r^n) = 1 + r + r² + r³ + ... = 1 / (1 - r), para n=0 até ∞

Portanto:
    Gt = Σ(γ^k) = 1 / (1 - γ)
```

### Referências
- [Propriedades de Somatório](https://pt.wikipedia.org/wiki/Somat%C3%B3rio)
- [Série Geométrica](https://pt.wikipedia.org/wiki/S%C3%A9rie_geom%C3%A9trica)