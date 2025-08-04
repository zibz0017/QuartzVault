# Definition
<span style="display: block; text-align: justify;">The square root, of the average, of the [[Residual, Sum of Least Squares, and Regression Line Calculation#Residual|residuals]], squared. This is similar to the [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)]], but slightly different.</span>
# Steps
1. <span style="display: block; text-align: justify;">Get the residual for every point.</span>
2. <span style="display: block; text-align: justify;">Square them.</span>
3. <span style="display: block; text-align: justify;">Add them all together.</span>
4. <span style="display: block; text-align: justify;">Divide by $n-1$. (We are getting the average but since we are just using a sample, we divide by $n-1$ instead of $n$. See [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Why There is a Different Calculation for the Population Variance and the Sample Variance|here]] for why that is.</span>
# Similar to Standard Deviation
<span style="display: block; text-align: justify;">As said earlier, this is similar to finding the standard deviation. The difference is that for standard deviation, we find the difference between the values and the *mean*. Here we are finding the difference between the values and the *values predicted by the regression line*. After that, though, it is the same. We square all of the values, add them up, and then divide by $n-1$ (assuming you are dealing with a sample, which is usually the case).</span>

