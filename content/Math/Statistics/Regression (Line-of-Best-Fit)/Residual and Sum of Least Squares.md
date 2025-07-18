# Residual
<span style="display: block; text-align: justify;">Residual is the amount of difference between what is predicted by my regression line and what the actual data came out to be.</span>
<span style="display: block; text-align: justify;">This may be able to be calculated by looking at the point and looking at the regression line on the graph, or this can be figured out using the equation for the regression line ($y=mx+b$).</span>
<span style="display: block; text-align: justify;">We measure the difference for the $y$ value (meaning, what is the predicted $y$ value for something that has that $x$ value). If the actual value is above the predicted value, the residual is positive. If the actual value is below, the residual is negative.</span>
<span style="display: block; text-align: justify;">This can be calculated for every point.</span>
# Sum of Least Squares
<span style="display: block; text-align: justify;">The sum of least squares simply squaring the residuals and adding that up. The idea is that we want the regression line to have the smallest sum of least squares value (meaning, we want the regression line to predict the actual values as best as possible. The higher the sum of least squares value, the more off the regression line is).</span>
## Why Do We Take the Squared Values
<span style="display: block; text-align: justify;">We can't just add up the values together because some may be negative and some may be positive. Theoretically, we can have a regression line that is very off from all points but is higher than some and lower than others and has a very low sum of least squares value, even though the regression line is extremely inaccurate.</span>
<span style="display: block; text-align: justify;">To combat this, we can add up the absolute values. This would be effective.</span>
<span style="display: block; text-align: justify;">However, we take the squares because this makes outlier values carry more weight. See [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Advantage of Variance and $s$ over MAD|here]] for a more detailed explanation.</span>


