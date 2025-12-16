# Definition
A geometric random variable is similar to a [[Binomial|binomial]], with one key difference.
A random variable is a geometric random variable if:
1. There are two possible outcomes.
2. The probability of each outcome is the same.
3. There will keep being more events until a "success" is reached.
This last point is what differs a geometric random variable from a binomial. A binomial has a specific amount of events. A geometric does not have a specific amount of events.
## Example
The amount of coinflips it takes to flip a heads.
This checks all of the boxes: there are two possible outcomes (ignoring the fact that the coin can technically land on its side), the probability of each event is the same, and there will keep being more events until a "success" is reached.
# Calculating Exactly $n$ Number of Trials
## Formula
$$(1-p)^{n-1} \times p$$
## Reasoning
Let's say we want to calculate the probability that out first success will be in exactly $n$ number of trials, like for example, we want to calculate the odds that the first 6 we will spin on a six sided die will be in 5 spins.
A way to think about this is that we basically are trying to figure out the odds that we will have a failure for the first $n-1$ trials, and then a success on the $n^{th}$ trial. In our die example, it would mean that we need to figure out the probability of not getting a 6 in the first 4 spins and then getting a 6 on the 5th spin.
The formula for this is multiplying the probability of failure ($1-p$) by itself for the amount of failures that we want ($n-1$) and then multiplying that by the probability of success. Multiplying a number by itself is simply raising a number to a power.
As such, this becomes:
$$(1-p)^{n-1} \times p$$
In terms of the die roll, we multiply the probability of not spinning a 6 ($1-1/6=5/6$) by itself 4 times (or raise it to the fourth power), and then we multiply that by the probability of spinning a 6 ($1/6$).
This becomes:
$$(1-1/6)^4 \times 1/6 \Rightarrow (5/6)^4 \times 1/6 \Rightarrow 625/1296 \times 1/6 = \boxed{625/7776} \space or \approx \boxed{.08}$$
# Calculating at Least $n$ Number of Trials
# Calculating at Most $n$ Number of Trials