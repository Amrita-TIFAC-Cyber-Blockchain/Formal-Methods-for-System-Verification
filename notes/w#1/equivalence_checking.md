# NPTEL Course: Formal Methods for System Verification

## Equivalence Checking
### Combinatorics Circuit 
Consider the these two circuits

```
F1​(x,y,z) = x′yz′ + xyz′ + xyz
```

```
F2​(x,y,z) = yz′ + xy
```

To verify the Equivalence of these, the obvious method is the Truth Table (Brute Force)

| x | y | z | x'yz' | xyz' | xyz | F₁ | yz' | xy | F₂ |
|:-:|:-:|:-:|:-----:|:----:|:---:|:--:|:---:|:--:|:--:|
| 0 | 0 | 0 |   0   |   0  |  0  |  0 |  0  |  0 |  0 |
| 0 | 0 | 1 |   0   |   0  |  0  |  0 |  0  |  0 |  0 |
| 0 | 1 | 0 |   1   |   0  |  0  |  1 |  1  |  0 |  1 |
| 0 | 1 | 1 |   0   |   0  |  0  |  0 |  0  |  0 |  0 |
| 1 | 0 | 0 |   0   |   0  |  0  |  0 |  0  |  0 |  0 |
| 1 | 0 | 1 |   0   |   0  |  0  |  0 |  0  |  0 |  0 |
| 1 | 1 | 0 |   0   |   1  |  0  |  1 |  1  |  1 |  1 |
| 1 | 1 | 1 |   0   |   0  |  1  |  1 |  0  |  1 |  1 |
