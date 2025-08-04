# Residual
<span style="display: block; text-align: justify;">Residual is the amount of difference between what is predicted by the regression line and what the actual data came out to be.</span>
<span style="display: block; text-align: justify;">This may be able to be calculated by looking at the point and looking at the regression line on the graph, or this can be figured out using the equation for the regression line ($y=mx+b$).</span>
<span style="display: block; text-align: justify;">We measure the difference for the $y$ value (meaning, what is the predicted $y$ value for something that has that $x$ value). If the actual value is above the predicted value, the residual is positive. If the actual value is below, the residual is negative.</span>
<span style="display: block; text-align: justify;">This can be calculated for every point.</span>
# Sum of Least Squares Regression Line
<span style="display: block; text-align: justify;">The sum of least squares simply squaring the residuals and adding that up. The idea is that we want the regression line to have the smallest sum of least squares value (meaning, we want the regression line to predict the actual values as best as possible. The higher the sum of least squares value, the more off the regression line is).</span>
## Why Do We Take the Squared Values
<span style="display: block; text-align: justify;">We can't just add up the residual values together because some may be negative and some may be positive. Theoretically, we can have a regression line that is very off from all points but is higher than some and lower than others and so adding up the residuals will give us a very low value, even though the regression line is extremely inaccurate.</span>
<span style="display: block; text-align: justify;">To combat this, we can add up the absolute values. This would be effective.</span>
<span style="display: block; text-align: justify;">However, we take the squares because this makes outlier values carry more weight. See [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Advantage of Variance and $s$ over MAD|here]] for a more detailed explanation.</span>
<span style="display: block; text-align: justify;">Keep in mind that this can be a positive and a negative. Sometimes it may make more sense for an outlier to have a larger effect, but sometimes not. An outlier can disproportionately affect the regression line. In addition, the overall accuracy of the regression line will decrease because it is accommodating the outlier at the expense of the rest of the data (meaning, it is getting pulled toward this one point, and away for a bunch of points). As such, it may sometimes make more sense to remove the outlier before making regression calculations.</span>
# Formula
<span style="display: block; text-align: justify;">The symbol for a regression line is $\hat{y}$.</span>
<span style="display: block; text-align: justify;">The formula for any straight line is $y=mx+b$.</span>
<span style="display: block; text-align: justify;">The formula to calculate the slope ($m$) is:</span>
$$r*\left(\frac{s_y}{s_x}\right)$$
<span style="display: block; text-align: justify;">$r$ is the correlation and $s_x$ and $s_y$ is the [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|standard deviation]] of $x$ and $y$.</span>
<span style="display: block; text-align: justify;">The formula to calculate the y-intercept ($b$) is:</span>
$$\overline{y}-m\overline{x}$$
<span style="display: block; text-align: justify;">$\overline{y}$ and $\overline{x}$ is the average values of $x$ and $y$. $m$ is the slope. Which we just showed how to calculate.</span>
## Version 1 of the Formula
### Plugging in $b$ and Simplifying
<span style="display: block; text-align: justify;">If we replace $b$, we get:</span>
$$\hat{y}=mx+\overline{y}-m\overline{x}$$
<span style="display: block; text-align: justify;">This can get simplified. We change the order of the last  2 terms to:</span>
$$\hat{y}=mx-m\overline{x}+\overline{y}$$
<span style="display: block; text-align: justify;">We then pull out the $m$, giving us:</span>
$$\boxed{\hat{y}=m(x-\overline{x})+\overline{y}}$$
## Version 2 of the Formula
### Simplification from Previous Version
<span style="display: block; text-align: justify;">The slope ($m=r \cdot \left(\frac{s_y}{s_x}\right)$) can be expanded, and then simplified. We can then plug this back into the formula. We start by plugging in the values for $r$, $s_y$, and $s_x$:</span>

$$\frac{SS_{xy}}{\sqrt{{SS_{xx}} \cdot SS_{yy}}} \cdot \frac{\frac{\sqrt{SS_{yy}}}{n-1}}{\frac{\sqrt{SS_{xx}}}{n-1}}\Rightarrow$$
<span style="display: block; text-align: justify;">The $n-1$ in the denominators of the middle fraction cancel each other out, giving us:</span>
$$\frac{SS_{xy}}{\sqrt{{SS_{xx}} \cdot SS_{yy}}} \cdot \frac{\sqrt{SS_{yy}}}{\sqrt{SS_{xx}}} \Rightarrow$$
<span style="display: block; text-align: justify;">The $\sqrt{SS_{xx}}$ in the denominators of both fractions multiply together to equal $SS_{xx}$. In addition, the $\sqrt{SS_{yy}}$ in the numerator of the second fraction and denominator of the first fraction cancel each other out, giving us:</span>
$$\frac{SS_{xy}}{{SS_{xx}}}$$
<span style="display: block; text-align: justify;">We can take this and plug it back into the formula from [[#Version 1 of the Formula|version 1]], giving us:</span>
$$\boxed{\hat{y}=\frac{SS_{xy}}{{SS_{xx}}}(x-\overline{x})+\overline{y}}$$
## Version 3 of the Formula
<span style="display: block; text-align: justify;">Sometimes, the formula is written with $\frac{SS_{xy}}{SS_{xx}}$ instead of $m$ plugged into the original way we had the formula (meaning into $\hat{y}=mx+(\overline{y}-m\overline{x})$). As such, it becomes:</span>
$$\boxed{\hat{y}=\frac{SS_{xy}}{SS_{xx}}x+\overline{y}-\frac{SS_{xy}}{SS_{xx}}\overline{x}}$$
## Intuition
<span style="display: block; text-align: justify;">{<span style="color:rgb(255, 0, 0)">I don't really understand why the point $(\overline{x},\overline{y})$ must be on the line. I can understand why the regression line will be somewhere around there, but I don't see why it must go through there. I also don't understand why the slope should be lower if $r$ is lower.</span>}</span>
<span style="display: block; text-align: justify;">The slope formula ($r*\left(\frac{s_y}{s_x}\right)$) makes sense. If the standard deviation for $y$ is large, that means that the points are spread out. This means that the $y$ values with extend very far from the average on the vertical axis. As such, as $s_y$ increases, the slope must increase as well. Conversely, if $s_x$ is large, then that means that points are spread far from the average on the horizontal axis, and so the slope must decrease.</span>
# Ways of Measuring Accuracy of Regression Line
<span style="display: block; text-align: justify;">There are a few ways of measuring how accurately the regression line represents the data, such as [[Coefficient of Determination|coefficient of determination]], [[Correlation|correlation]], and [[Root-Mean-Square-Error|root-mean-square-error]].</span>

