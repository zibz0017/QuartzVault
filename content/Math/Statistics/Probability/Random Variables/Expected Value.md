# Definition
As the name implies, this is an amount you should expect to get over time. It is basically an average of all of the different possibilities of the [[Random Variable|random variable]] and then weighed by their frequency.
For example, the expected value of a die roll is 3.5, because the average of the values (1-6) is 3.5, and each one has an equal chance. If the die was weighted so it was more likely to land on a 1, 2, or 3, the expected value would be lower, because these lower values are more likely. Similarly, if the die was weighted so it was more likely to land on the 4, 5, or 6, the expected value would rise, as now the higher values are more likely.
Obviously, this does not mean that you should expect to spin a 3.5. That doesn't make any sense. It means that over time, the average of your spins will probably be close to 3.5.
# Examples
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
$$(0+0+0+0+0+1+1+1+2+3+3+3+3+3+3+3+4+4+5+5+5) \div (5+3+1+7+2+3)$$

To make it simpler, instead of adding up all of the values, we can use multiplication, as follows:
$$((0 \times 5) + (1 \times 3) + (2 \times 1) + (3 \times 7) + (4 \times 2) + (5 \times 3)) \div (5+3+1+7+2+3)$$
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
# What this means
The expected value is a good guess for what we can expect a result to be, on average. In [[#Example 1|example 1]], we we would expect to exercise, on average, $2\frac{1}{3}$ times per week. Obviously, we can't do a $\frac{1}{3}$ workout. What that means is that over time, we would expect that average. Like over 3 weeks, we would expect to have exercised around 7 time.
This is just an estimate. it isn't guaranteed that this person will exercise 7 times in 3 weeks, but this is the best guess that we can come up with based on the data that we have.
# Symbol
The symbol for expected value is the same as the symbol for average, which is: $\mu$.
If we wanted to write the expected value for random variable $X$ is 7 (for example), we write: $\mu_X=7$.