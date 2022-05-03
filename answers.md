# CMPS 2200 Assignment 5
## Answers

**Name:** James Manzer


Place all written answers from `assignment-05.md` here for easier grading.





- **1a.**

Let X = 2^k Geometrica currency demonitations that will make up the solution to the greedy algorithm, which is the fewest coins to sum up to a number, N.

This algorithm will find the largest demonitation of Geometrica that is lower than the given value, subtract the Geomtrica demonination and continually do so until we get to 0. The number of geometrica coins will be counted upon each iteration of the recusrive function, and this will be the optimal number of tokens.

The alrogithm is always optimal because it can recursively call itself to find the fewest amount of tokens possible, which is garunteed using this method.

def greedy(x)

x = input
k = 0
i = 0
y = 0
if x == 0
  return 0
else
for 2^k > x
  k++
i++
y = x - 2^k
greedy(y)

- **1b.**

For a number $43, the number of iterations would be log_2^43

The work and span for the algorithm would be O(log_2^n)

- **2a.**

Given a random number like 29, we would know how to calculate the optimal number of tokens using geometrica, show how geometrica would solve it. Because we don't know the denominations, we have no base value to compare it to (ex. 2^k). For example, using a random number 5, there could be the currency of denomination 5, and there would be 1 coin used, whereas the algorithm from part 1 would return 2 tokens. This is not optimal.

- **2b.**

Using the bottom-up approach, work and span are O(N*k),

- **3a.**

The optimal substructure for this problem is found in the first else statement of the MED function, if (S[0] == T[0]) then it would be (MED(S[1:], T[1:])). Otherwise, it would be (1 + min(MED(S, T[1:]), MED(S[1:], T)))

