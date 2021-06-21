### *Exercise 5.1:*

**Consider the diagrams on the right in Figure 5.1. Why does the estimated value function jump up for the last two rows in the rear? Why does it drop off for the whole last row on the left? Why are the frontmost values higher in the upper diagrams than in the lower?**

---
Resposta 1:

```
"Why does the estimated value function jump up for the last two rows in the rear?"

The estimated value function jumps up for the last two rows because those states mean the player is sticking with a 20 or 21 and, thus, is very likely to win. In contrast, on the other states, the player will hit, making it more likely that they will lose. For instance, hitting on a 19 means they bust unless they can draw an ace or a 2, which is a very low chance. Another example would be the state 14, in which the reward is also low since the transition to the 20-21 states is unlikely.

In shorter words, the last two rows represent the states in which the player was lucky enough. The other, lower rows represent the states in which the player's decision of only sticking at 20 or 21 takes its toll, since they are very likely to burst.


"Why does it drop off for the whole last row on the left?"

Because, overall, having an Ace increases the chance of winning. Since it's an ambivalent card, there are two times more winning configurations with an ace. THe row on the left shows the Dealer drawing an ace.


"Why are the frontmost values higher in the upper diagrams than in the lower?"

Because having an usable ace decreases the chance of busting. The first row depicts a sum of 12, which may represent the player drawing two aces.

```
