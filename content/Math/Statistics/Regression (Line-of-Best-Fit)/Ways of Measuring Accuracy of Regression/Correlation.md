
# Definition
A measure of how well a straight line fits the data.
## Specific Points
1. <span style="display: block; text-align: justify;">Correlation is always between -1 and 1.</span>
2. <span style="display: block; text-align: justify;">If the line-of-best-fit (as it is called) has a positive slope, the correlation is positive. And the same is true for negative.</span>
3. <span style="display: block; text-align: justify;">A correlation of 1 or -1 means that a straight line can be drawn perfectly through the data. (The difference is that a correlation of 1 means that the line is upward-sloping, while a correlation of -1 means that the line is negative-sloping.) (See [[#Example 1]] and [[#Example 2]].)</span>
4. <span style="display: block; text-align: justify;">A correlation of 0 means that a line-of-best-fit does an extremely poor job of representing the data (see [[#Example 3]]).</span>
5. <span style="display: block; text-align: justify;">Correlation only measures for a straight line, not any other type of line (see [[#Example 4]]).</span>
6. <span style="display: block; text-align: justify;">Correlation only measures if a straight line can be drawn through the data. It does not measure how steep the line-of-best-fit is (see [[#Example 5]] and [[#Example 6]]). This is important because you can have data for which there is a smaller correlation between $x$ and $y$, but it can matter more.</span>
7. <span style="display: block; text-align: justify;">This is not as good at expressing the accuracy of the regression line as the [[Coefficient of Determination|coefficient of determination]]. See [[Coefficient of Determination#Coefficient of Determination vs Correlation]] for why.</span>
## Symbol and Formula
<span style="display: block; text-align: justify;">The symbol for correlation is $r$.</span>
The formula is: $$r=\frac{1}{n-1}\left(\sum_{i=1}^{n}((z \space score \space of \space x_i)(z \space score \space of \space y_i)) \right)$$
### Version 1 of the Formula
With the [[Z-Score#Formula for Converting Values Into Z-Scores|z-score formula written out]], it becomes this:$$\boxed{r=\frac{1}{n-1}\left(\sum_{i=1}^{n}\left(\left(\frac{x_i-\overline{x}}{s_X}\right)\left(\frac{y_i-\overline{y}}{s_Y}\right)\right) \right)}$$
The previous formula is what you should use if you already know the standard deviation (or you want to figure it out anyway, or you can easily calculate it).

See [[#Example 7]] for a worked-through problem.
### Version 2 of the Formula
#### Step by Step Simplification from Previous Version
*Note: We are going to explain how to simplify the previous formula to get to the next version. The final second version is [[#Final Step|here]].*

We can simplify the previous a little if we [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation|write out the standard deviation formula]]. It becomes this:$$r=\frac{1}{n-1} \sum_{i=1}^{n}\left(\left(\frac{x_i-\overline{x}}{\sqrt{\frac{1}{n-1}\sum_{j=1}^{n}{(x_j-\overline{x})^2}}}\right)\left(\frac{y_i-\overline{y}}{\sqrt{\frac{1}{n-1}\sum_{j=1}^{n}{(y_j-\overline{y})^2}}}\right)\right) \Rightarrow$$

(We then multiply the 2 big fractions in the middle together)

$$r=\frac{1}{n-1} \sum_{i=1}^{n}\left(\frac{(x_i-\overline{x})(y_i-\overline{y})}{\left(\sqrt{\frac{1}{n-1}\sum_{j=1}^{n}{(x_j-\overline{x})^2}}\right)\left(\sqrt{\frac{1}{n-1}\sum_{j=1}^{n}{(y_j-\overline{y})^2}}\right)}\right) \Rightarrow$$


(We the multiply the 2 square roots in the denominator together. The $\frac{1}{n-1}$ pops out of the square root because $\sqrt{\frac{1}{n-1}} \cdot \sqrt{\frac{1}{n-1}} = \frac{1}{n-1}$)

$$r=\frac{1}{n-1} \sum_{i=1}^{n}\left(\frac{(x_i-\overline{x})(y_i-\overline{y})}{\frac{1}{n-1}\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}}\right) \Rightarrow$$

(We can now pull the $\frac{1}{n-1}$ out of the whole summation (the $\sum$) as [[Σ (Uppercase Sigma, Summation)#Turn Into Multiplication|you can pull a constant value out of a summation]]. However, whenever you pull a fraction out of the denominator, you have to flip the fraction. It was dividing the denominator which is like multiplying the numerator.)

$$r=\frac{1}{n-1}\cdot\frac{n-1}{1} \sum_{i=1}^{n}\left(\frac{(x_i-\overline{x})(y_i-\overline{y})}{\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}}\right) \Rightarrow$$

(The first terms multiply together to equal 1, which can ignore.)

$$r=1 \cdot \sum_{i=1}^{n}\left(\frac{(x_i-\overline{x})(y_i-\overline{y})}{\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}}\right) \Rightarrow$$
(The denominator is not affected by the summation, meaning, [[Σ (Uppercase Sigma, Summation)#Turn Into Multiplication (Continued)|it is like a constant which can be pulled out]].)

$$r=\frac{1}{\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}} \cdot \sum_{i=1}^{n}(x_i-\overline{x})(y_i-\overline{y}) \Rightarrow$$

(We then multiply them together to get to the final form.)
#### Final Form
$$\boxed{r=\frac{\sum_{i=1}^{n}(x_i-\overline{x})(y_i-\overline{y})}{\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}}}$$

This last formula is slightly simpler if you don't already have the standard deviation.

See [[#Example 7]] for a worked-through problem.
#### Alternative Final Form
We can use the [[Sum of Cross-Products and Sum of Squares Notation|sum of cross-products and sum of squares notation]] to make things a bit neater. As such, we convert to:

$$\boxed{r=\frac{SS_{xy}}{\sqrt{{SS_{xx}} \cdot SS_{yy}}}}$$
<span style="display: block; text-align: justify;">(As a side note, the notation can't be broken down. $S_x$ technically just means the population standard deviation of x. It doesn't mean $\sum_{i=1}^{n}(x_i-\overline{x})$ or something like that.)</span>
### Version 3 of the Formula
#### Step by Step Simplification from Previous Version
##### Step 1
<span style="display: block; text-align: justify;">We are going to start with the numerator:</span>
$$\sum_{i=1}^{n}(x_i-\overline{x})(y_i-\overline{y}) \Rightarrow$$
First we multiply it out:
$$\sum_{i=1}^{n}x_iy_i-x_i\overline{y}-\overline{x}y_i+\overline{x}\overline{y} \Rightarrow$$
We can now use some manipulations that can be done with summations. We can [[Σ (Uppercase Sigma, Summation)#Split the Summation|split this into multiple summations]]:
$$\sum_{i=1}^{n}x_iy_i-\sum_{i=1}^{n}x_i\overline{y}-\sum_{i=1}^{n}\overline{x}y_i+\sum_{i=1}^{n}\overline{x}\overline{y} \Rightarrow$$
We can further simplify by [[Σ (Uppercase Sigma, Summation)#Turn Into Multiplication]]. For the last term (the $\sum_{i=1}^{n}\overline{x}\overline{y}$), the summation turns into $n$ which was the amount of times that the values there were being added up:

$$\sum_{i=1}^{n}x_iy_i-\overline{y}\sum_{i=1}^{n}x_i-\overline{x}\sum_{i=1}^{n}y_i+n\overline{x}\overline{y} \Rightarrow$$
$\sum_{i=1}^{n}x_i=n\overline{x}$ and $\sum_{i=1}^{n}y_i=n\overline{y}$. In other words, if we take all of the values and add them up, that will equal the average times the amount of values that there are. (If you get a 60, an 80, and a 100 on 3 tests, this adds up to 240. If you take the average (80) and multiply it by the amount of tests that there are (3), you also get 240). We can plug this into the formula:
$$\sum_{i=1}^{n}x_iy_i-\overline{y}n\overline{x}-\overline{x}n\overline{y}+n\overline{x}\overline{y} \Rightarrow$$

The 3rd and 4th terms (or the 2nd and 4th terms. The 2nd and 3rd term are the same) cancel out, giving us:
$$\sum_{i=1}^{n}x_iy_i-\overline{y}n\overline{x}$$

Plugging this back into the numerator of version 2 of the formula, we get:
$$\frac{\sum_{i=1}^{n}x_iy_i-n\overline{y}\overline{x}}{\sqrt{\left(\sum_{j=1}^{n}{(x_j-\overline{x})^2}\right)\left(\sum_{j=1}^{n}{(y_j-\overline{y})^2}\right)}}$$ ^0f5417
##### Step 2
We can simplify the $\sum_{j=1}^{n}{(x_j-\overline{x})^2}$ and $\sum_{j=1}^{n}{(y_j-\overline{y})^2}$ in the denominator by using foil (we'll just display it with $x$, but the same is obviously true for $y$):
$$\sum_{j=1}^{n}{(x_j-\overline{x})^2} \Rightarrow \sum_{j=1}^{n}x_j^2 - 2\sum_{j=1}^{n}x_j\overline{x} + \sum_{j=1}^{n}\overline{x}^2$$
Pulling the constants out of the summations we get:
$$\sum_{j=1}^{n}x_j^2 - 2\overline{x}\sum_{j=1}^{n}x_j + n\overline{x}^2$$
We can simplify the $\sum_{j=1}^{n}x_j$ in the middle term to $n\overline{x}$. We can then further simplify the middle term:
$$\sum_{j=1}^{n}x_j^2 - 2\overline{x}n\overline{x} + n\overline{x}^2 \Rightarrow \sum_{j=1}^{n}x_j^2 - 2n\overline{x}^2 + n\overline{x}^2$$
Adding the 3rd term to the 2nd term we get:
$$\sum_{j=1}^{n}x_j^2 - n\overline{x}^2$$

We can now plug this back into the denominator of the formula we created [[#^0f5417|here]] to give us:
$$\frac{\sum_{i=1}^{n}x_iy_i-n\overline{y}\overline{x}}{\sqrt{\left({\sum_{j=1}^{n}(x_j^2) - n\overline{x}^2}\right)\left(\sum_{j=1}^{n}(y_j^2) - n\overline{y}^2\right)}}$$ ^847605
##### Step 3
Another thing we can change is $\overline{x}=\frac{\sum^n_{i=1}x_i}{n}$ and $\overline{y}=\frac{\sum^n_{i=1}y_i}{n}$. We start by plugging it into the numerator:
$$\sum_{i=1}^{n}x_iy_i-n\overline{y}\overline{x} \Rightarrow \sum_{i=1}^{n}x_iy_i-n\frac{\sum^n_{i=1}y_i}{n}\cdot\frac{\sum^n_{i=1}x_i}{n}$$
Multiplying the fractions and the $n$ on the right together we get:
$$\sum_{i=1}^{n}x_iy_i-\frac{n\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n^2}$$
Then we cancel out the $n$ in the numerator the squared in the denominator:
$$\sum_{i=1}^{n}x_iy_i-\frac{\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n}$$
We can then add the 1st term with the second term by multiplying the first term by $\frac{n}{n}$, giving us:
$$\frac{n\sum_{i=1}^{n}x_iy_i}{n}-\frac{\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n}$$
Combining them together becomes:
$$\frac{n\sum_{i=1}^{n}x_iy_i-\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n}$$

We can plug this into the numerator of the equation we created [[#^847605|here]], giving us: ^2df87e

$$\frac{\frac{n\sum_{i=1}^{n}x_iy_i-\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n}}{\sqrt{\left({\sum_{j=1}^{n}(x_j^2) - n\overline{x}^2}\right)\left(\sum_{j=1}^{n}(y_j^2) - n\overline{y}^2\right)}}$$
##### Step 4
Now we can change the denominator. We start by plugging in $\overline{x}=\frac{\sum^n_{i=1}x_i}{n}$ and $\overline{y}=\frac{\sum^n_{i=1}y_i}{n}$:
$$\sqrt{\left({\sum_{j=1}^{n}(x_j^2) - n\overline{x}^2}\right)\left(\sum_{j=1}^{n}(y_j^2) - n\overline{y}^2\right)} \Rightarrow$$
$$\sqrt{\left({\sum_{j=1}^{n}(x_j^2) - n\frac{(\sum^n_{i=1}x_i)^2}{n^2}}\right)\left(\sum_{j=1}^{n}(y_j^2) - n\frac{(\sum^n_{i=1}y_i)^2}{n^2}\right)} \Rightarrow$$
We cancel out the $n$s with the $n^2$s in the denominator, giving us:
$$\sqrt{\left({\sum_{j=1}^{n}(x_j^2) - \frac{(\sum^n_{i=1}x_i)^2}{n}}\right)\left(\sum_{j=1}^{n}(y_j^2) - \frac{(\sum^n_{i=1}y_i)^2}{n}\right)} \Rightarrow$$
We now multiply both summations (meaning, the summation in the first parentheses and the summation in the second parentheses) by $\frac{n}{n}$ giving us:

$$\sqrt{\left({\frac{n\sum_{j=1}^{n}(x_j^2)}{n} - \frac{(\sum^n_{i=1}x_i)^2}{n}}\right)\left(\frac{n\sum_{j=1}^{n}(y_j^2)}{n} - \frac{(\sum^n_{i=1}y_i)^2}{n}\right)} \Rightarrow$$
We can now combine the fraction on the left and on the right together, giving us:
$$\sqrt{\left({\frac{n\sum_{j=1}^{n}(x_j^2) - \sum^n_{i=1}(x_i)^2}{n}}\right)\left(\frac{n\sum_{j=1}^{n}(y_j^2)-\sum^n_{i=1}(y_i)^2}{n}\right)} \Rightarrow$$
We can multiply the fractions together, which becomes:
$$\sqrt{\frac{(n\sum_{j=1}^{n}(x_j^2) - \sum^n_{i=1}(x_i)^2)(n\sum_{j=1}^{n}(y_j^2)-\sum^n_{i=1}(y_i)^2)}{n^2}} \Rightarrow$$
We can pull the $n^2$ in the denominator out of the square root by turning it into $n$. As such, this becomes:
$$\frac{\sqrt{(n\sum_{j=1}^{n}(x_j^2) - \sum^n_{i=1}(x_i)^2)(n\sum_{j=1}^{n}(y_j^2)-\sum^n_{i=1}(y_i)^2)}}{n} \Rightarrow$$
We can now plug this back into the denominator in the equation we created [[#^2df87e|here]], giving us:
$$\frac{\frac{n\sum_{i=1}^{n}x_iy_i-\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{n}}{\frac{\sqrt{(n\sum_{j=1}^{n}(x_j^2) - \sum^n_{i=1}(x_i)^2)(n\sum_{j=1}^{n}(y_j^2)-\sum^n_{i=1}(y_i)^2)}}{n}} \Rightarrow$$
##### Final Form
We can now get rid of the $n$s in the denominator of the numerator and the denominator of the denominator:
$$\boxed{\frac{n\sum_{i=1}^{n}x_iy_i-\sum^n_{i=1}y_i\cdot\sum^n_{i=1}x_i}{\sqrt{(n\sum_{j=1}^{n}(x_j^2) - \sum^n_{i=1}(x_i)^2)(n\sum_{j=1}^{n}(y_j^2)-\sum^n_{i=1}(y_i)^2)}}}$$
Just to make things a little easier to read, we are going to get rid of all subtext (the $_i$s and $_j$s) and all that just to make it more readable:
$$\boxed{\frac{n\sum xy-\sum y\cdot\sum x}{\sqrt{(n\sum(x^2) - \sum(x)^2)(n\sum(y^2)-\sum(y)^2)}}}$$
### Intuition
(We are going to focus on the first version of the formula but the same is true about the second and third version.)

In the formula, we multiply the z-score of the x and y coordinates of each point together.

<span style="display: block; text-align: justify;">If the z-scores of the x and y coordinates are both negative or both positive, then the product is positive. In other words, if the point being measured is in the bottom left or the top right the product is positive. If there are a lot of points in the bottom left or top right, the correlation will be positive. That makes sense as line-of-best-fit will be positively sloping.</span>
<span style="display: block; text-align: justify;">Conversely, if the z-score of the x coordinate is positive and the y coordinate is negative, the product will be negative. As such, if the point being measured is in the top left or bottom right, the product will be negative. If there are many points in the top left or bottom right, the correlation will be negative. That makes sense as the line-of-best-fit will be negatively sloping.</span>

# Examples
## Example 1
![[Pasted image 20250702232938.png]]
<span style="display: block; text-align: justify;">The correlation here is 1 because a positive-sloping straight line can be drawn perfectly through the data.</span>
## Example 2
![[Pasted image 20250702233257.png]]
<span style="display: block; text-align: justify;">The correlation here is 1 because a negative-sloping straight line can be drawn perfectly through the data.</span>
## Example 3
![[Pasted image 20250702234000.png]]
<span style="display: block; text-align: justify;">There isn't much correlation here, and it is hard to know if it is positive or negative just by eyeballing. The correlation will probably be close to 0.</span>
## Example 4
![[Pasted image 20250702235259.png]]
<span style="display: block; text-align: justify;">There is a strong positive correlation, but it is not 1. Even though you can draw a perfect quadratic graph through this ($y=x^2$), you can't draw a perfect straight line through it.</span>
## Example 5
![[Pasted image 20250703000525.png]]
<span style="display: block; text-align: justify;">Both data sets have a correlation of 1, even though the black dots have a steeper slope.</span>
## Example 6
![[Pasted image 20250703000705.png]]
<span style="display: block; text-align: justify;">Both data sets have a correlation of -1, even though the black dots have a steeper slope.</span>
## Example 7
![[Pasted image 20250711011425.png]]
The points in the previous set have the following coordinates: (1,1), (2,3), (3,6), (4,4).
### Solving with Version 1 of the Formula
1. Calculate the values for all of the relevant variables.
$$n=4$$
$$\overline{x} \Rightarrow \frac{1+2+3+4}{4} \Rightarrow \frac{10}{4}=\textbf{2.5}$$
$$\overline{y} \Rightarrow \frac{1+3+6+4}{4} \Rightarrow \frac{14}{4} \Rightarrow \textbf{3.5}$$
$$SD_x \Rightarrow \sqrt{\frac{\sum_{1}^{n}(x_i-\overline{x})^2}{n-1}} \Rightarrow \sqrt{\frac{(1-2.5)^2+(2-2.5)^2+(3-2.5)^2+(4-2.5)^2}{4-1}} \Rightarrow$$
$$\sqrt{\frac{(-1.5)^2+(-.5)^2+(.5)^2+(1.5)^2}{3}} \Rightarrow \sqrt{\frac{2.25+.25+.25+2.25}{3}} \Rightarrow \sqrt{\frac{5}{3}} \approx \textbf{1.29}$$
$$SD_y \Rightarrow \sqrt{\frac{\sum_{1}^{n}(y_i-\overline{y})^2}{n-1}} \Rightarrow \sqrt{\frac{(1-3.5)^2+(3-3.5)^2+(6-3.5)^2+(4-3.5)^2}{4-1}} \Rightarrow$$
$$\sqrt{\frac{(-2.5)^2+(-.5)^2+(2.5)^2+(.5)^2}{3}} \Rightarrow \sqrt{\frac{6.25+.25+6.25+.25}{3}} \Rightarrow \sqrt{\frac{13}{3}} \approx \textbf{2.08}$$
2. Plug the values into the correlation formula.
$$\frac{1}{4-1}\left(\left(\frac{1-2.5}{1.29}\right)\left(\frac{1-3.5}{2.08}\right) + \left(\frac{2-2.5}{1.29}\right)\left(\frac{3-3.5}{2.08}\right) + \left(\frac{3-2.5}{1.29}\right)\left(\frac{6-3.5}{2.08}\right) + \left(\frac{4-2.5}{1.29}\right)\left(\frac{4-3.5}{2.08}\right)\right) \Rightarrow$$
$$\frac{1}{3} \left(\left(\frac{-1.5}{1.29}\right)\left(\frac{-2.5}{2.08}\right) + \left(\frac{-.5}{1.29}\right)\left(\frac{-.5}{2.08}\right) + \left(\frac{.5}{1.29}\right)\left(\frac{2.5}{2.08}\right) + \left(\frac{1.5}{1.29}\right)\left(\frac{.5}{2.08}\right)\right) \approx$$
$$\frac{1}{3}(1.4+.09+.47+.28) \approx \textbf{.747}$$
### Solving with Version 2 of the Formula
1. Calculate the values for all of the relevant variables.

$$n=4$$

$$\overline{x} \Rightarrow \frac{1+2+3+4}{4} \Rightarrow \frac{10}{4}=\textbf{2.5}$$

$$\overline{y} \Rightarrow \frac{1+3+6+4}{4} \Rightarrow \frac{14}{4} \Rightarrow \textbf{3.5}$$

2. Plug the values into the correlation formula.

$$\frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{\left(\sum_{j=1}^{4}{(x_j-2.5)^2}\right)\left(\sum_{j=1}^{4}{(y_j-3.5)^2}\right)}} \Rightarrow$$

(Solving for the denominator)

$$\frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{((1-2.5)^2+(2-2.5)^2+(3-2.5)^2+(4-2.5)^2)((1-3.5)^2+(3-3.5)^2+(6-3.5)^2+(4-3.5)^2)}} \Rightarrow$$

$$\frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{((-1.5)^2+(-.5)^2+(.5)^2+(1.5)^2)((-2.5)^2+(-.5)^2+(-2.5)^2+(.5)^2)}} \Rightarrow$$

$$\frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{(2.25+.25+.25+2.25)(6.25+.25+6.25+.25)}} \Rightarrow$$

$$\frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{5\cdot13}} \Rightarrow \frac{\sum_{i=1}^{4}(x_i-2.5)(y_i-3.5)}{\sqrt{65}} \Rightarrow$$

(Solving for the numerator)

$$\frac{(1-2.5)(1-3.5)+(2-2.5)(3-3.5)+(3-2.5)(6-3.5)+(4-2.5)(4-3.5)}{\sqrt{65}} \Rightarrow$$

$$\frac{(-1.5\cdot-2.5)+(-.5\cdot-.5)+(.5\cdot2.5)+(1.5\cdot.5)}{\sqrt{65}} \Rightarrow $$

$$\frac{3.75+.25+1.25+.75}{\sqrt{65}} \Rightarrow \frac{6}{\sqrt{65}} \approx \textbf{.744}$$
(There is a slight difference between the answers from each version of the equation due to rounding.)
# Example 8
![[Pasted image 20250803201118.png]]
<span style="display: block; text-align: justify;">The black dots have a perfect correlation of 1, while the purple dots clearly have a lower correlation. But the $x$ value for the purple dots may matter more.</span>
<span style="display: block; text-align: justify;">For example, if this was a graph measuring different weight-loss treatments, even though there is a perfect correlation between the weight lost and the "black dots method", most people would want to try the "purple dots method", even though it has a lower correlation, because the effects are clearly more drastic, even if they are somewhat less predictable.</span>



