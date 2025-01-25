# Julia Code Bug: Unexpected Behavior with Negative Numbers

This repository demonstrates a subtle bug in a Julia function that involves unexpected behavior when handling negative numbers within a conditional statement.

## Description

The `myfunction` in `bug.jl` is designed to square the input if it is positive, return 0 if it is 0, and return the negative of the square if it is negative.  However, due to the order of operations, the calculation `-x^2` yields unexpected results for negative inputs. The solution file demonstrates the correct approach.

## How to Reproduce

1. Clone this repository.
2. Run the Julia script `bug.jl`.
3. Observe the output for positive, zero, and negative inputs. Note the unexpected behavior with negative numbers. 
4. Then run `bugSolution.jl` to see the corrected code.

## Solution

The solution involves using parentheses to ensure that the negation is applied after the squaring operation, fixing the order of operations issues.  See `bugSolution.jl` for a corrected version of the function.