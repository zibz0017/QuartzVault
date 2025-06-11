# Mean Absolute Deviation (MAD)
## MAD Definition
Average of the distance of all of the numbers from the mean (with all distances being a positive value).
## Steps to Find MAD
1. Find the mean.
2. Find how far every number is from the mean by subtracting the mean from each number and getting the absolute value (make the number positive if it is negative).
3. Find the average of these distances. Add them all up together, then divide by the total number of values in the set.
## Calculating MAD Example
Set of numbers: 4, 7, 13, 23, 18, -2
Find the mean:

$$
\frac{4+7+13+23+18+\text{-}2}{6} \Rightarrow \frac{63}{6} = 10.5
$$

Find how far every number is from the mean (and make them all positive):

$$
|10.5-4|=6.5
$$

$$
|10.5-7|=3.5
$$

$$
|10.5-13|=2.5
$$

$$
|10.5-23|=12.5
$$

$$
|10.5-18|=7.5
$$

$$
|10.5-\text{-}2|=12.5
$$

Add up all of the distances:

$$
6.5+3.5+2.5+12.5+7.5+12.5=45
$$

Divide by the amount of numbers:

$$
\frac{47}{6} = \textbf{7.5}
$$

# Variance
## Symbol
Population variance: $σ^2$ (lowercase sigma squared)
Sample variance: $s^2$
## Variance Definition
Average of the *squared* distance of all of the numbers from the mean.
## Steps to Find Variance
### Steps to Find Population Variance (σ^2)
*Note: This is slightly different than finding the a sample variance. How to [[#Steps to Find Sample Variance (s 2)|calculate the sample variance]] and [[#Why There is a Different Calculation for the Population Variance and the Sample Variance|why the population and sample variance are different]] will be explained later.*
1. Find the mean.
2. Find how far the squared distance every number is from the mean by subtracting the mean from each number and squaring it.
3. Find the average of these squared distances. Add them all up together, then divide by the total number of values in the set.
### Steps to Find Sample Variance (s^2)
The exact same as finding the population variance, except instead of dividing the whole thing by the amount of numbers, we divide by the amount of numbers *minus 1*.
So the steps are:
1. Find the mean.
2. Find how far the squared distance every number is from the mean by subtracting the mean from each number and squaring it.
3. Add up all of these squared distances together, then divide by the total number of values in the sample.
## Calculating Variance Example
### Population Variance Example
Set of numbers: 4, 7, 13, 23, 18, -2
Find the mean:
$$\frac{4+7+13+23+18+\text{-}2}{6} \Rightarrow \frac{63}{6}= 10.5$$
Find the squared distances from the mean:
$$(10.5-4)^2=42.25$$
$$(10.5-7)^2=12.25$$
$$(10.5-13)^2=6.25$$
$$(10.5-23)^2=156.25$$
$$(10.5-18)^2=56.25$$
$$(10.5-\text{-}2)^2=156.25$$
Add up all of the squared distances:
$$42.25+12.25+6.25+156.25+56.25+156.25=429.5$$
Divide by the amount of numbers:
$$\frac{429.5}{6} \approx \textbf{71.583}$$
### Sample Variance Example
If the above set was a sample from a larger set, we would do the exact same thing until the last step. As such, we do:

Find the mean:
$$\frac{4+7+13+23+18+\text{-}2}{6} \Rightarrow \frac{63}{6}= 10.5$$
Find the squared distances from the mean:
$$(10.5-4)^2=42.25$$
$$(10.5-7)^2=12.25$$
$$(10.5-13)^2=6.25$$
$$(10.5-23)^2=156.25$$
$$(10.5-18)^2=56.25$$
$$(10.5-\text{-}2)^2=156.25$$
Add up all of the squared distances:
$$42.25+12.25+6.25+156.25+56.25+156.25=429.5$$
Divide by the amount of numbers *minus 1*:
$$\frac{429.5}{(6-1)} \Rightarrow \frac{429.5}{5} = \textbf{85.9}$$
## Why There is a Different Calculation for the Population Variance and the Sample Variance
{<span style="color:rgb(255, 0, 0)">This section is important and I think it can use more work</span>}
The sample variance is obviously supposed to be an estimate of the population variance. However, it comes out lower.
This is because the sample variance is not based on the real mean of the whole set. It is based on the mean of the sample. At times, this sample mean may be quite accurate (and if the sample is large enough, it will usually be so), but many times, it will not be.
For the most part, the sample data will generally not include the less extreme data so the data will generally be clustered together and the variance will be lower.
Even when there are extreme cases, the sample mean will be "pulled" toward the sample data, making the extreme data make less of difference. As such, even though some samples will have a higher variance, these relatively few cases will not have a high enough variance to counter the lower variance from most of the samples (which will generally contain largely non-extreme numbers).
To counter this "bias", we subtract 1 from the denominator in the final step to increase the sample variance to give us a better estimate of the actual variance.
## Additional Point
The sample mean and the variance are largely not correlated. On average, the variance of the sample (using n, not n-1) is lower than the population variance, regardless of what the sample mean is.
# Standard Deviation (σ or SD)
## Symbol
Population standard deviation: $σ$ (lowercase sigma)
Sample standard deviation: $s$
## Standard Deviation Definition
The square root of the [[#Variance|variance]]. In other words, the square root of the average of the squared distance from the mean.
## Steps to Find Standard Deviation
### Steps to Find Population Standard Deviation
*Note: This is slightly different than finding the a sample standard deviation. How to [[#Steps to Find Sample Standard Deviation|calculate the sample standard deviation]] will be explained later and [[#Why There is a Different Calculation for the Population Variance and the Sample Variance|why the population and sample standard deviations are different]] is the same reason why there is a difference between the population variance and the sample variance.*
Find the variance, and then take the square root. To break it down:
1. Find the mean.
2. Find how far the squared distance every number is from the mean by subtracting the mean from each number and squaring it.
3. Find the average of these squared distances. Add them all up together, then divide by the total number of values in the set.
4. Find the square root of that number.
   
In the above example, the population variance is 85.9 . The population standard deviation of is the square root of that, so it is around **8.46**.
### Steps to Find Sample Standard Deviation
The exact same as finding the population standard deviation, except instead of dividing using the sample variance. As such, most of the steps are the same, except that we divide the total squared distance from the mean by the the amount of numbers used *minus 1*.
To lay it all out, we do the following:
1. Find the mean.
2. Find how far the squared distance every number is from the mean by subtracting the mean from each number and squaring it.
3. Add them all up together, then divide by the amount of numbers in the sample *minus one*.
4. Find the square root of that number.
In the above example, the sample variance is around 71.583. The population standard deviation of is the square root of that, so it is around **9.27**.
# Purpose of These Measures
These measures are for measuring how far dispersed data in a set is. The higher the number, the more dispersed. The lower the number, the less dispersed.

## Example
Data set 1: 1, 2, 3, 4, 5
Data set 2: -1,1, 3, 5, 7

Both of these sets have a mean and median of 3, but the numbers in the first set are bunched closer together.
These measures will tell this to us.
# Advantages to Different Measures
## Advantage of MAD and SD over Variance
Units come out weird with variance, while they come out useful with MAD and SD. With variance, the units come out in units squared. With MAD and SD, they are just regular units.

For example, let's say the numbers given in the above data set are measurements in inches of some things. In [[#Calculating Variance Example|example given where we calculate the variance]], we said that:
$$(10.5-4)^2=42.25$$
If these were measurements in inches, for example, it really is:
$$(10.5 \space in -4 \space in)^2=42.25 \space in^2$$
(The same is true for all of the calculations. I just picked one to illustrate.)

*in<sup>2</sup>* is an odd unit and not very useful. We don't square anything in the calculations to find the MAD, so the units are normal. 

For MAD:
$$|10.5 \space in-4 \space in|=6.5 \space in$$
For the SD, we do square the units, but then we find the square root, so the units are turned back into the normal units. So in the above example, the variance ends up being:
$$\frac{42.25 \space in^2 +12.25 \space in^2 +6.25 \space in^2 +156.25 \space in^2 +56.25 \space in^2 +156.25 \space in^2}{6} \Rightarrow \frac{429.5 \space in^2} {6}  \approx 71.583 \space in^2$$
We then take the square root of that to find the SD:
$$\sqrt{71.583 \space in^2} \approx 8.46  \space in $$
The units are *in*, not *in<sup>2</sup>*.