# R Silent Subset Bug
This repository demonstrates a subtle bug in R related to subsetting data frames using logical vectors.  When a logical vector is longer than the number of rows in the data frame, R silently truncates the vector without warning, leading to incorrect results.  This is particularly problematic as it can be difficult to debug, as there's no immediate error message.

The `bug.R` file contains the problematic code, and `bugSolution.R` illustrates a way to handle this issue and prevent unexpected behavior.

## How to reproduce
1. Clone this repository.
2. Open `bug.R` and run the code.
3. Observe the output; the resulting subset is smaller than expected.
4. Compare this with the output of `bugSolution.R`, which addresses the issue.