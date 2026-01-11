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
## Expected Value
<span style="color:rgb(255, 0, 0)">Come back to [this video](https://www.khanacademy.org/math/statistics-probability/random-variables-stats-library/random-variables-geometric/v/proof-of-expected-value-of-geometric-random-variable) for the formula and the logic behind it. You need to know about the math of infinite sequences</span>
# Calculating at Least $n$ Number of Trials
You want to figure out the probability that the first success for an event comes on the $n$<sup>th</sup> trial or later.
## Formula
$$(1-p)^n$$
## Reasoning
Technically, a way to figure this out would be to add up the probability of getting a success in exactly $n$ trials, and then exactly $n+1$ trials, and then $n+2$ trials, etc. However, this is obviously difficult if not impossible.
Another way to think about getting a success after $n$ number of trials is *not* getting a success on $n-1$ number of trials.
For example, the odds of getting heads on the 5<sup>th</sup> coin flip or later is the same as the odds of getting tails for the first 4 flips. They actually mean the same thing. Getting a heads on you 5<sup>th</sup> flip or later means that you got tails for the first 4 flips.
The way to figure this out is the odds of "failing" $n$ times in a row. The probability of failure, is $1-p$.
The way we calculate the odds that multiple independent events happen together is by multiplying them together, as discussed [[Independent Events#Probability of Event A AND B|here]].
As such, the probability of failing is:
$$(1-p) \times (1-p) \times (1-p) … (1-p)$$
(We multiply $1-p$, $n$ times.)
A simpler way of writing this is just:
$$(1-p)^n$$
Plugging this in to the coin flip question, this becomes:
$$(1-.5)^4 \Rightarrow .5^4 = \boxed{.0625}$$
# Calculating at Most $n$ Number of Trials
## Formula
$$1-(1-p)^n$$
## Reasoning
This can be calculated by finding the probability of getting a success on the first event, or the second event, or the third event… until we get up to $n$<sup>th</sup> event. However, this can be difficult.
A simpler way of thinking about this is that we don't want out first success to be after the $n$<sup>th</sup> event. We can calculate the probability of getting the first success after at least $n$ trials, as discussed [[#Calculating at Least $n$ Number of Trials|above]], and so all we need to do is find the probability that that doesn't happen. The way we do that is by subtracting the probability that it does happen from $1$, as discussed [[Independent Events#Probability of NOT Event A|here]]. (A way to think about that is that the probability that an event happens or doesn't happen is 100% or 1, like the probability that you will either win or not win a game you are playing is 100%, sort of by definition. What else could possibly happen? With a little algebra, we can therefore say that the probability that something won't happen is $1-probability \space it \space will \space happen$).
As such, the formula is $1-probability \space it \space takes \space at \space least \space n \space trials$, which becomes:
$$1-(1-p)^n$$