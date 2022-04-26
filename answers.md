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


- **2a.**

Given a random number like 29, we would know how to calculate the optimal number of tokens using geometrica, show how geometrica would solve it. Because we don't know the denominations, we have no base value to comapre it to (ex. 2^k)



- **2b.**



