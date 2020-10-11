### Q: The policy iteration algorithm on page 80 has a subtle bug in that it may never terminate if the policy continually switches between two or more policies that are equally good. This is okay for pedagogy, but not for actual use. Modify the pseudocode so that convergence is guaranteed.

#### Original

```
1. Initialization
    V(s) ∈ ℝ and π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    Loop:
        Δ <- 0
        Loop for each s ∈ S:
            v <- V(s)
            V(s) <- Σp(s', r | s, π(s))[r + γvπ(s')]
            Δ <- max(Δ, |v - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)

3. Policy Improvement 
    policy-stable <- true
    For each s ∈ S:
        old-action <- π(s)
        π(s) <- argmax a Σp(s', r | s, a)[r + γvπ(s')]
        If old-action ≠ π(s), then policy-stable <- false
    If policy-stable, then stop and return V ≅ x* and π ≅ π*; else go to 2 
```


#### Melhoria
A melhoria abaixo segue a mesma ideia de ter as etapas de **Policy Evaluation** e **Policy Improvement**, porém há algoritmos mais otimizados, como por exemplo o **Value Iteration**.

```
1. Initialization
    V(s) ∈ ℝ and π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    Loop:
        Δ <- 0
        Loop for each s ∈ S:
            v <- V(s)
            V(s) <- Σp(s', r | s, π(s))[r + γvπ(s')]
            Δ <- max(Δ, |v - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)

3. Policy Improvement
    Loop:
        Δ <- 0
        old-state-value <- v
        Go to 2
        For each s ∈ S:
            π(s) <- argmax a Σp(s', r | s, a)[r + γvπ(s')]
            Δ <- max(Δ, |old-state-value(s) - V(s)|)
    until Δ < θ (a small number determining the accuracy of estimation)
```
