### Q: The pseudocode for Monte Carlo ES is inecient because, for each state–action pair, it maintains a list of all returns and repeatedly calculates their mean. It would be more ecient to use techniques similar to those explained in Section 2.4 to maintain just the mean and a count (for each state–action pair) and update them incrementally. Describe how the pseudocode would be altered to achieve this.

#### Original
```
Initialize:
    π(s) ∈ A(s) (arbitrarily) for all s ∈ S
    Q(s, a) ∈ ℝ (arbitrarily) for all s ∈ S, a ∈ A(s) 
    Returns(s, a) <- empty list, for all s ∈ S, a ∈ A(s)

Loop forever (for each episode):
    Choose S0 ∈ S, A0 ∈ A(S0) randomly such that all pairs have probability > 0
    Generate an episode from S0, A0, following π: S0, A0, R1,...,ST-1, AT-1, RT
    G <- 0
    Loop for each step of episode, t = T-1, T-2,..., 0:
        G <- γG + Rt+1
        Unless the pair St, At appears in S0, A0, S1, A1 ...,St-1, At-1:
            Append G to Returns(St, At)
            Q(St, At) <- average(Returns(St, At))
            π(St) <- argmax a Q(St, a) 
```

#### Melhoria
```
Initialize:
    π(s) ∈ A(s) (arbitrarily) for all s ∈ S
    Q(s, a) <- 0 for all s ∈ S, a ∈ A(s) 
    N(s, a) <- 0 for all s ∈ S, a ∈ A(s)

Loop forever (for each episode):
    Choose S0 ∈ S, A0 ∈ A(S0) randomly such that all pairs have probability > 0
    Generate an episode from S0, A0, following π: S0, A0, R1, ..., ST-1, AT-1, RT
    G <- 0
    Loop for each step of episode, t = T-1, T-2,..., 0:
        G <- γG + Rt+1
        Unless the pair St, At appears in S0, A0, S1, A1 ...,St-1, At-1:
            N(s, a) <- N(s, a) + 1
            Q(St, At) <- Q(St, At) + (1 / N(s, a)) * [G - Q(St, At)]
            π(St) <- argmax a Q(St, a) 
```
