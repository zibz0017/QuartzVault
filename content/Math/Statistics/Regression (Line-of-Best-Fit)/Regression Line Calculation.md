# Form
<span style="display: block; text-align: justify;">Like all calculations of a straight line, the formula is presented as $y=mx+b$.</span>
# Formula
<span style="display: block; text-align: justify;">The symbol for a regression line is $\hat{y}$</span>
<span style="display: block; text-align: justify;">The formula  is:</span>
$$\hat{y}=r*\left(\frac{s_x}{s_y}\right)+b$$

<span style="display: block; text-align: justify;">$r$ is the correlation and $s_x$ and $s_y$ is the [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|standard deviation]] of $x$ and $y$.</span>
<span style="display: block; text-align: justify;">As can be seen, the formula for the slope is $r*\left(\frac{s_x}{x_y}\right)$.</span>
<span style="display: block; text-align: justify;">$b$ is calculated by plugging a point into the regression formula once we figure out the slope. The regression line has to go through the point $(\overline{x},\overline{y})$ (the average of the x values and the average of the y values). We then rearrange the equation using algebra to give us the following: $b=y-mx$. We plug the slope and the values of $\overline{x}$ and $\overline{y}$ into the equation to figure out $b$.</span>
## Intuition
<span style="display: block; text-align: justify;">{<span style="color:rgb(255, 0, 0)">I don't really understand why the point $(\overline{x},\overline{y})$ must be on the line. I can understand why the regression line will be somewhere around there, but I don't see why it must go through there. I also don't understand why the slope should be lower if $r$ is lower.</span>}</span>
The slope formula ($r*\left(\frac{s_y}{s_x}\right)$) makes sense. If the standard deviation for $y$ us <span style="display: block; text-align: justify;">large, that means that the points are spread out. This means that the $y$ values with extend very far from the average on the vertical axis. As such, as $s_y$ increases, the slope must increase as well. Conversely, if $s_x$ is large, then that means that points are spread far from the average on the horizontal axis, and so the slope must decrease.</span>

