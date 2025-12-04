# Definition
A random variable is some event with results that occur randomly.
## Examples
1. A die roll.
2. A coin flip.
3. The outdoor temperature tomorrow.
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
The reason we can't use the bar chart is because we don't have an infinite number of discrete "buckets". In the temperature example, the temperature can be $70\degree F$. It may be $70.1\degree F$. It may be $70.2\degree F$. It may be $70.3\degree F$. It may be $70.0142\degree F$, and it keeps going, as discussed earlier. There is no way to map this using a bar chart. We would have a near-infinite number of bars to draw.
Additionally, the odds that an event occurs at any precise value is basically 0. What are the odds that the temperature tomorrow is precisely $70.0142\degree F$ and not $70.0142000000001\degree F$ or $70.01419999999999\degree F$? It's basically 0 as there are technically an infinite number of possible temperatures that there may be.
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
1. By definition, the relative frequencies must add up to 1 (or 100%).
2. Relative frequencies must be positive values.
# [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]] And [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]]
The standard deviation and variance can be good measure of the spread of a discrete random variable. See those articles for how to calculate.
## Example
We are going to calculate the variance and standard deviation of the [[#Relative Frequency|egg example]] from above (we are going to do this for the relative frequencies, but these can be calculated for the exact amounts as well. See the articles for [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|standard deviation]] and [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|variance]] for examples).
To calculate the variance, we need to:
1. Get the differences for each amount from the mean.
2. Square the difference.
3. Multiply by their frequency.
4. Add those differences together.
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
# Binomials
Random variables that have two results, "success" and "failure" (these can be arbitrary) are called [[Binomials|binomials]].

# Footnotes

[^1]: [MathBitsNotebook.com : Algebra 1](https://mathbitsnotebook.com/Algebra1/StatisticsData/SThistogram.html)