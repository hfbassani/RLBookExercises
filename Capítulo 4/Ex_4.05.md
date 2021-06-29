### *Exercise 4.5:*

**How would policy iteration be defined for action values? Give a complete algorithm for computing q*, analogous to that on page 80 for computing v*. Please pay special attention to this exercise, because the ideas involved will be used throughout the rest of the book.**

---
Resposta 1:

```
1. Initialization
    Q(s, a) arbitrarily, for all s ∈ S, a ∈ A
    π(s) ∈ A(s) arbitrarily for all s ∈ S

2. Policy Evaluation
    Loop:
        Δ <- 0
        Loop for each s ∈ S, for each a ∈ A:
            q <- Q(s, a)
            Q(s, a) <- Σp(s', r | s, π(s))[r + γqπ(s', π(s'))]
            Δ <- max(Δ, |q - Q(s, a)|)
    until Δ < θ (a small number determining the accuracy of estimation)

3. Policy Improvement 
    policy-stable <- true
    For each s ∈ S:
        old-action <- π(s)
        π(s) <- argmax a Σp(s', r | s, a)[r + γqπ(s', a)]
        If old-action ≠ π(s), then policy-stable <- false
    If policy-stable, then stop and return Q ≅ x* and π ≅ π*; else go to 2 
```
