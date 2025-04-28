# CMPS 2200 Assignment 3
## Answers

**Name:**Mauricio Uribe


Place all written answers from `assignment-03.md` here for easier grading.

1a.  Find the largest 2^k that is less than or equal to N, then repeatedly subtract 2^k from N until N becomes 1 or smaller.

1b. At each step, k is as large as possible because the highest coin value still fits within N. This ensures the solution is optimal, as using a smaller coin would require more coins overall.

1c. The work is O(log N) and the span is O(log N).

2a. Counterexample: with denominations (1, 3, 4) and amount 6, the greedy algorithm picks (4, 1, 1) (3 coins), while the optimal solution is (3, 3) (2 coins).

2b. This problem has optimal substructure because solving for amount N requires picking a denomination and optimally solving for the remaining amount (N - denomination). The overall optimal solution relies on optimal solutions to its subproblems.

2c. A bottom-up dynamic programming approach computes the optimal number of coins for every amount from 0 to N by considering each denomination. The work and span are both O(N * k), where N is the target amount and k is the number of denominations.

3a. Implemented the provided top-down memoized solution (fast_MED) in Python.
