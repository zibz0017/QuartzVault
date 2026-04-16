# Definition
A random variable is some event with results that occur randomly.
## Examples
1. <span style="display: block; text-align: justify;">A die roll.</span>
2. <span style="display: block; text-align: justify;">A coin flip.</span>
3. <span style="display: block; text-align: justify;">The outdoor temperature tomorrow.</span>
# Notation
Random Variables are generally given a capital letter and then we write what they equal.
## Examples
$$X=\{Amount \space of \space heads \space in \space 3 \space coin \space flips\}$$
$$Y=\{Exact \space weight \space of \space the \space Empire \space State \space Building\}$$
$$A=\{Amount \space of \space noodles \space in \space a \space box \space of \space macaroni\}$$
# Why This is Useful
This is useful because it makes discussing probabilities simpler. Using the previous examples, we can say:
$$P(X=1)=\frac{1}{8}$$
This means that the probability of flipping 1 head in 3 coin flips is $\frac{1}{8}$.
# Types of Random Variables
<span style="color:rgb(255, 0, 0)">Perhaps divide Discrete and Continuous into their own articles. Combine Continuous with [[Density Curve]], and maybe move [[Density Curve]] to the Random Variables folder. Also, take [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance]] and put into Discrete article. Maybe binomials, too?</span>
## Discrete
There are no potential values that can be infinitely long decimals.
### Examples
$$F=\{The \space year \space that \space the \space next \space person \space I \space meet \space was \space born \space in\}$$
There is a discrete answer for this. It may be in year $2000$. It could be in year $1920$. It could be in a bunch of possible different years. But it can't be in year $1950.15782052948$, for example. We are dealing with discrete years.
### Specific Types of Discrete Random Variables
There are specific types of discrete random variables, such as [[Binomial|binomials]], and [[Geometric Random Variable|geometric random variables]]. See those articles for more details.
## Continuous
Values can have infinitely long decimals.
### Examples
$$T=\{The \space exact \space outdoor \space temperature \space tomorrow \space at \space 12:00 \space PM\}$$
The temperature may be $70\degree F$. It may be $70.1\degree F$. It may be $70.2\degree F$. It may be $70.3\degree F$. It may be $70.0142\degree F$. There is no limit to how many digits long our decimal can go.
## Why This Matters
When charting the probabilities of different results of out random variable, a discrete random variable can be expressed using a bar chart:
![[Pasted image 20251103214037.png]][^1]
There are discrete "buckets" of possible values and we can map the probabilities that any one of these values may occur.
When charting the probability of a continuous random variable, we are going to use graph, like this:
![[Pasted image 20250610221007.png]]
This is called a [[Density Curve|density curve]] (see there for more details).
The reason we can't use the bar chart is because we don't have an infinite number of discrete "buckets". In the temperature example, the temperature can be $70\degree F$. It may be $70.1\degree F$. It may be $70.2\degree F$. It may be $70.3\degree F$. It may be $70.01\degree F$. It may be $70.0001\degree F$. It may be $70.01385092837\degree F$, and it keeps going, as discussed earlier. There is no way to map this using a bar chart. We would have a near-infinite number of bars to draw.
Additionally, the odds that an event occurs at any precise value is basically 0. What are the odds that the temperature tomorrow is precisely $70.1\degree F$ and not $70.100000000001\degree F$ or $70.099999999999\degree F$? It's basically 0 as there are technically an infinite number of possible temperatures that there may be.
# How Frequencies Are Recorded
## Exact Amount
As the name implies, the exact amounts are given.
For example, a person counts the amount of eggs that are broken in egg cartons. The results were as follows:

| Amount of Broken Eggs | Frequency |
| --------------------- | --------- |
| 0                     | 27        |
| 1                     | 6         |
| 2                     | 3         |
| 3                     | 3         |
| 4                     | 1         |
The data is given over with the exact amounts.
## Relative Frequency
The percentage of each "bucket" of the total is given.
Using the same data from the previous example, we get:

| Amount of Broken Eggs | Relative Frequency |
| --------------------- | ------------------ |
| 0                     | .675               |
| 1                     | .15                |
| 2                     | .075               |
| 3                     | .075               |
| 4                     | .025               |
### Rules about Relative Frequencies
1. <span style="display: block; text-align: justify;">By definition, the relative frequencies must add up to 1 (or 100%).</span>
2. <span style="display: block; text-align: justify;">Relative frequencies must be positive values.</span>
# Expected Value (Average)
As the name implies, this is an amount you should expect to get over time. It is basically an average of all of the different possibilities of the [[Random Variable|random variable]] and then weighed by their frequency.
For example, the expected value of a die roll is 3.5, because the average of the values (1-6) is 3.5, and each one has an equal chance. If the die was weighted so it was more likely to land on a 1, 2, or 3, the expected value would be lower, because these lower values are more likely. Similarly, if the die was weighted so it was more likely to land on the 4, 5, or 6, the expected value would rise, as now the higher values are more likely.
Obviously, this does not mean that you should expect to spin a 3.5. That doesn't make any sense. It means that over time, the average of your spins will probably be close to 3.5.
## Example 1
A person kept track of how many times they exercised in a week. The results were:

| Times per Week | Frequency |
| -------------- | --------- |
| 0              | 5         |
| 1              | 3         |
| 2              | 1         |
| 3              | 7         |
| 4              | 2         |
| 5              | 3         |
The expected value can be calculated by finding the weighted average. This is done by adding up all of the values and then dividing them by the total amount of values, as follows:
$$\frac{0+0+0+0+0+1+1+1+2+3+3+3+3+3+3+3+4+4+5+5+5}{5+3+1+7+2+3}$$

To make it simpler, instead of adding up all of the values, we can use multiplication, as follows:
$$\frac{(0 \times 5) + (1 \times 3) + (2 \times 1) + (3 \times 7) + (4 \times 2) + (5 \times 3)}{5+3+1+7+2+3}$$
Either way we get:
$$49 \div 21 = \boxed{2 \frac{1}{3}}$$
## Example 2
A person records the relative frequencies of how much customers spend in a store, rounded to the nearest dollar.

| Amount of Money Spent | Relative Frequency |
| --------------------- | ------------------ |
| $1.00                 | .05                |
| $2.00                 | .15                |
| $3.00                 | .4                 |
| $4.00                 | .3                 |
| $5.00                 | .1                 |
When given relative frequencies (which is just a percentage of the total), to calculate the expected value, we just need to add the numbers multiplied by their relative frequencies. As such, we get:
$$(1.00 \times .05) + (2.00 \times .15) + (3.00 \times .4) + (4.00 \times .3) + (5.00 \times .1) \Rightarrow$$$$.05+.3+1.2+1.2+.5=\boxed{3.25}$$
## What This means
The expected value is a good guess for what we can expect a result to be, on average. In [[#Example 1|example 1]], we we would expect to exercise, on average, $2\frac{1}{3}$ times per week. Obviously, we can't do a $\frac{1}{3}$ workout. What that means is that over time, we would expect that average. Like over 3 weeks, we would expect to have exercised around 7 time.
This is just an estimate. it isn't guaranteed that this person will exercise 7 times in 3 weeks, but this is the best guess that we can come up with based on the data that we have.
## Symbol
The symbol for expected value is the same as the symbol for average, which is: $\mu$.
If we wanted to write the expected value for random variable $X$ is 7 (for example), we write: $\mu_X=7$.
## Law of Large Numbers
If we take many samples of a random variable, the average of the will be close to the actual expected value, and the more samples we take, the closer it will usually get.
For example, lets say we want to count the amount of heads in 2 coin flips. The expected value is $np$, as discussed, and so that would be $2 \times .5 = 1$. However, it is very reasonable that we get 2 heads or 2 tails. Even if we run this experiment twice, it is reasonable that we get 3 heads or 3 tails in total, which would bring our average between the 2 samples to 1.5 or .5 (the probability would be around .62 or 62%). However, after 10 flips, the probability of having an average of at least 1.5 or at most .5 drops to around .04, or 4%. After 100 flips, the probability of averaging at least 1.5 or at most .5 is 0.0000005636 or er 0.00005636%. In fact, the probability of averaging only over 1.3 or under .7 heads is only around .002 or .2%.
The idea basically is that while you can get lucky or unlucky a few times, it is very unlikely to keep happening.
# [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]] And [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]]
The standard deviation and variance can be good measure of the spread of a discrete random variable. See those articles for how to calculate.
## Example
We are going to calculate the variance and standard deviation of the [[#Relative Frequency|egg example]] from above (we are going to do this for the relative frequencies, but these can be calculated for the exact amounts as well. See the articles for [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|standard deviation]] and [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|variance]] for examples).
To calculate the variance, we need to:
1. <span style="display: block; text-align: justify;">Get the differences for each amount from the mean.</span>
2. <span style="display: block; text-align: justify;">Square the difference.</span>
3. <span style="display: block; text-align: justify;">Multiply by their frequency.</span>
4. <span style="display: block; text-align: justify;">Add those differences together.</span>
To get the standard deviation, we take the square root of that amount.
Going through the steps, the mean is:
$$0 \times .675 +1 \times .15 + 2 \times .075 + 3 \times .075 + 4 \times .025 = \boxed{.625}$$
We then get the differences of each value from the mean:
$0-.625=-.625$
$1-.625=.375$
$2-.625=1.375$
$3-.625-2.375$
$4-.625=3.375$
We then square each one:
$-.625^2=.390625$
$.375^2=.140625$
$1.375^2 = 1.890625$
$2.375^2=5.640625$
$3.375^2=11.390625$
We then multiply each value by its relative frequency:
$.390625 × .675 = .263671875$
$.140625 × .15=.02109375$
$1.890625 × .075=.141796875$
$5.640625 × .075=.423046875$
$11.390625 × .025=.284765625$
Finally, to get the variance, we need to add all of these values together:
$$0.263671875 + 0.02109375 + 0.141796875 + 0.423046875 + 0.284765625=\boxed{1.134375}$$
To get the standard deviation, we need to take the square root of this, which is:
$$1.134375 \approx \boxed{1.066}$$
# Footnotes

[^1]: [MathBitsNotebook.com : Algebra 1](https://mathbitsnotebook.com/Algebra1/StatisticsData/SThistogram.html)