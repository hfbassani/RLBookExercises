Exercise 3.4 Give a table analogous to that in Example 3.3, but for p(s0
, r|s, a). It
should have columns for s, a, s0
, r, and p(s0
, r|s, a), and a row for every 4-tuple for which
p(s0
, r|s, a) > 0.

| s    | a      | s'   | r       | p(s', r \| s, a) |
|------|--------|------|---------|------------------|
| high | search | high | rsearch | α                |
| high | search | low  | rsearch | 1 - α            |
| low  | search | high | -3      | 1 - β            |
| low  | search | low  | rsearch | β                |
| high | wait   | high | rwait   | 1                |
| low  | wait   | low  | rwait   | 1                |
| low  |recharge| high | 0       | 1                |