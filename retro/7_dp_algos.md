## 💡 What we learned

_DP_

- (Re)Learned about the different approaches to dynamic programming problems
  - Identify optimal substructures and overlapping subproblems!
- Top down recursive
- Bottom up iterative
- Memoization is performed either through key value storing or tabular data storing

_Problems_

- Coin Change problem, top-down:
  Can be solved through following the subtree by continually navigating the call tree by choosing the minimum number at each depth level.
- Fibonacci problem: top-down:
  Can be solved through combining the values of the two child nodes to determine the parent node.
- 0-1 Knapsack problem: bottom-up:
  Can be solved by tabulating a 2D matrix of possible solutions for each combination of {weight, value}. Possible table solutions are determined by calculating which items honor the problem constraints at each input combinations.

_C++_

- Explored some stdc++ methods to take advantage of vectors and maps
- Refreshed how maps, std outputs, method scoping, compilation work in C++

## ✅ Accomplishments that we're proud of

- Working solutions to 3 dp programming problems in C++ so far

## ⚠Challenges we ran into

- Understanding which data types to use is somewhat difficult, coming from Javascript, C#, Python, Progress, there are so many options within C++.
- Minor nuances in language slowed down the problem solution development.

## 🚧 How we built it

- Based on the problem, reviewed the problem, designed a solution and programmed it with trial and error :)

### 💎Full Feature List

- Do you want to know the nth fibonacci number? we got that
- Do you want to know what to put in your knapsack? got that too
- Do you want to know the fewest num of coins to use? okay we can do that
