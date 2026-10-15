# Definition
The central limit theorem states that for every distribution, if you take sets of samples from them and take the average of each of those sets and then you plot the distribution of those averages, they will start to look like a [[Density Curve#Normal Distribution|normal distribution]].
The larger the sample size is for each set of samples, the more it will look normal (it will be less skewed to one side or the other, and have a smaller kurtosis) and the tighter around the mean it will be.
This is true even for distributions that are very far from normal.
# Example
## Example Distribution
Here is an example of a made-up distribution:

| Amount | Probability |
| ------ | ----------- |
| 1      | .4          |
| 2      | .1          |
| 3      | .05         |
| 4      | .05         |
| 5      | .15         |
| 6      | .25         |

^991fd4

```chart
type: bar
labels: []
series:
  - title: 
    data: []
id: 991fd4
tension: 0.2
width: 80%
labelColors: false
fill: false
beginAtZero: true
bestFit: false
bestFitTitle: undefined
bestFitNumber: 0
```
This distribution is clearly far from normal.
## First Set of Samples
Here are 100 sets of 4 samples created using Google Sheets based on this distribution and their averages.

| 1st Sample in Set | 2nd | 3rd | 4th | Average |
| ----------------- | --- | --- | --- | ------- |
| 5                 | 5   | 5   | 1   | 4       |
| 3                 | 5   | 1   | 2   | 2.75    |
| 1                 | 2   | 4   | 6   | 3.25    |
| 1                 | 1   | 6   | 6   | 3.5     |
| 6                 | 6   | 3   | 5   | 5       |
| 1                 | 1   | 6   | 5   | 3.25    |
| 1                 | 3   | 1   | 1   | 1.5     |
| 2                 | 1   | 4   | 5   | 3       |
| 6                 | 2   | 1   | 1   | 2.5     |
| 1                 | 1   | 6   | 6   | 3.5     |
| 1                 | 1   | 1   | 5   | 2       |
| 3                 | 1   | 1   | 1   | 1.5     |
| 3                 | 6   | 3   | 1   | 3.25    |
| 1                 | 1   | 2   | 2   | 1.5     |
| 6                 | 1   | 5   | 6   | 4.5     |
| 6                 | 1   | 1   | 5   | 3.25    |
| 1                 | 5   | 3   | 6   | 3.75    |
| 1                 | 1   | 5   | 6   | 3.25    |
| 6                 | 1   | 6   | 6   | 4.75    |
| 6                 | 5   | 5   | 5   | 5.25    |
| 6                 | 1   | 3   | 5   | 3.75    |
| 3                 | 4   | 1   | 2   | 2.5     |
| 1                 | 2   | 1   | 4   | 2       |
| 1                 | 5   | 1   | 4   | 2.75    |
| 1                 | 1   | 1   | 1   | 1       |
| 6                 | 2   | 5   | 6   | 4.75    |
| 1                 | 1   | 6   | 2   | 2.5     |
| 6                 | 1   | 2   | 6   | 3.75    |
| 1                 | 1   | 1   | 1   | 1       |
| 1                 | 2   | 2   | 1   | 1.5     |
| 1                 | 6   | 1   | 1   | 2.25    |
| 1                 | 2   | 1   | 1   | 1.25    |
| 4                 | 6   | 3   | 5   | 4.5     |
| 6                 | 1   | 6   | 2   | 3.75    |
| 1                 | 5   | 1   | 1   | 2       |
| 5                 | 5   | 1   | 1   | 3       |
| 6                 | 2   | 1   | 5   | 3.5     |
| 2                 | 1   | 4   | 1   | 2       |
| 4                 | 5   | 5   | 5   | 4.75    |
| 2                 | 5   | 6   | 1   | 3.5     |
| 1                 | 1   | 6   | 6   | 3.5     |
| 1                 | 2   | 1   | 5   | 2.25    |
| 6                 | 2   | 3   | 6   | 4.25    |
| 6                 | 6   | 3   | 1   | 4       |
| 6                 | 6   | 6   | 5   | 5.75    |
| 2                 | 2   | 1   | 6   | 2.75    |
| 5                 | 1   | 2   | 6   | 3.5     |
| 1                 | 6   | 5   | 3   | 3.75    |
| 6                 | 1   | 1   | 2   | 2.5     |
| 3                 | 6   | 6   | 5   | 5       |
| 2                 | 1   | 1   | 5   | 2.25    |
| 2                 | 6   | 1   | 1   | 2.5     |
| 2                 | 5   | 3   | 1   | 2.75    |
| 2                 | 6   | 5   | 6   | 4.75    |
| 1                 | 1   | 1   | 1   | 1       |
| 5                 | 1   | 4   | 1   | 2.75    |
| 1                 | 6   | 5   | 1   | 3.25    |
| 5                 | 1   | 6   | 5   | 4.25    |
| 1                 | 1   | 5   | 1   | 2       |
| 6                 | 5   | 1   | 2   | 3.5     |
| 3                 | 1   | 6   | 3   | 3.25    |
| 5                 | 1   | 5   | 5   | 4       |
| 1                 | 1   | 1   | 6   | 2.25    |
| 1                 | 1   | 2   | 2   | 1.5     |
| 6                 | 1   | 4   | 1   | 3       |
| 1                 | 6   | 1   | 6   | 3.5     |
| 2                 | 1   | 6   | 4   | 3.25    |
| 5                 | 5   | 6   | 2   | 4.5     |
| 5                 | 5   | 5   | 6   | 5.25    |
| 5                 | 1   | 6   | 1   | 3.25    |
| 6                 | 2   | 4   | 3   | 3.75    |
| 5                 | 5   | 5   | 1   | 4       |
| 1                 | 6   | 6   | 4   | 4.25    |
| 1                 | 6   | 6   | 6   | 4.75    |
| 6                 | 2   | 4   | 2   | 3.5     |
| 6                 | 1   | 1   | 1   | 2.25    |
| 1                 | 6   | 6   | 6   | 4.75    |
| 1                 | 1   | 6   | 6   | 3.5     |
| 1                 | 5   | 3   | 1   | 2.5     |
| 1                 | 5   | 3   | 1   | 2.5     |
| 1                 | 1   | 2   | 1   | 1.25    |
| 6                 | 1   | 2   | 6   | 3.75    |
| 1                 | 1   | 5   | 3   | 2.5     |
| 5                 | 6   | 6   | 1   | 4.5     |
| 5                 | 1   | 6   | 1   | 3.25    |
| 6                 | 6   | 5   | 1   | 4.5     |
| 2                 | 1   | 5   | 1   | 2.25    |
| 6                 | 2   | 1   | 2   | 2.75    |
| 6                 | 1   | 6   | 6   | 4.75    |
| 1                 | 6   | 1   | 1   | 2.25    |
| 2                 | 6   | 2   | 6   | 4       |
| 6                 | 3   | 6   | 1   | 4       |
| 1                 | 2   | 6   | 1   | 2.5     |
| 6                 | 1   | 6   | 3   | 4       |
| 2                 | 1   | 1   | 5   | 2.25    |
| 1                 | 1   | 1   | 2   | 1.25    |
| 5                 | 4   | 1   | 1   | 2.75    |
| 4                 | 5   | 1   | 1   | 2.75    |
| 3                 | 2   | 3   | 1   | 2.25    |
| 6                 | 1   | 5   | 5   | 4.25    |

### Aggregate Data
If we aggregate the averages of the sets into groups we get:

| Bins     | Count |
| -------- | ----- |
| 1-1.49   | 6     |
| 1.5-1.99 | 5     |
| 2-2.49   | 14    |
| 2.5-2.99 | 17    |
| 3-3.49   | 13    |
| 3.5-3.99 | 17    |
| 4-4.49   | 11    |
| 4.5-4.99 | 12    |
| 5-5.49   | 4     |
| 5.5-6    | 1     |

^66fee9

```chart
type: line
labels: []
series:
  - title: 
    data: []
id: 66fee9
tension: 0.2
width: 80%
labelColors: false
fill: false
beginAtZero: true
bestFit: false
bestFitTitle: undefined
bestFitNumber: 0
```
As can be seen, this somewhat resembles a normal distribution, despite the fact that the distribution that this is based on wasn't anything like a normal distribution.
## Second Set of Samples
If we increase the sample size (meaning, the amount of samples in each set), the distribution will tighten around the mean, and will be closer to a normal distribution.
Here are sets of 25 samples (created the same way. I put the averages in the table below):

| 1st Trial | 2nd | 3rd | 4th | 5th | 6th | 7th | 8th | 9th | 10th | 11th | 12th | 13th | 14th | 15th | 16th | 17th | 18th | 19th | 20th | 21st | 22nd | 23rd | 24th | 25th |
| --------- | --- | --- | --- | --- | --- | --- | --- | --- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1         | 1   | 6   | 6   | 6   | 6   | 2   | 1   | 5   | 1    | 6    | 5    | 5    | 2    | 5    | 1    | 6    | 6    | 6    | 2    | 1    | 5    | 3    | 6    | 6    |
| 1         | 3   | 6   | 2   | 2   | 5   | 6   | 6   | 1   | 1    | 1    | 1    | 1    | 5    | 6    | 2    | 1    | 1    | 2    | 6    | 1    | 4    | 1    | 1    | 3    |
| 1         | 6   | 6   | 1   | 1   | 4   | 2   | 2   | 1   | 5    | 1    | 1    | 1    | 6    | 1    | 1    | 5    | 1    | 6    | 6    | 3    | 1    | 1    | 6    | 1    |
| 1         | 1   | 1   | 1   | 1   | 6   | 6   | 1   | 5   | 6    | 1    | 6    | 3    | 1    | 3    | 6    | 2    | 6    | 2    | 6    | 1    | 1    | 5    | 1    | 1    |
| 6         | 1   | 6   | 6   | 5   | 1   | 1   | 6   | 6   | 1    | 1    | 6    | 1    | 1    | 6    | 1    | 1    | 1    | 1    | 6    | 5    | 6    | 5    | 6    | 5    |
| 1         | 6   | 1   | 1   | 4   | 1   | 1   | 1   | 1   | 1    | 1    | 3    | 1    | 4    | 3    | 6    | 6    | 6    | 2    | 6    | 6    | 4    | 6    | 1    | 5    |
| 6         | 6   | 2   | 3   | 1   | 2   | 4   | 6   | 5   | 1    | 4    | 5    | 6    | 1    | 1    | 1    | 2    | 1    | 4    | 5    | 1    | 1    | 6    | 3    | 1    |
| 1         | 1   | 1   | 1   | 5   | 1   | 1   | 1   | 4   | 1    | 1    | 4    | 2    | 1    | 1    | 4    | 4    | 6    | 1    | 1    | 3    | 5    | 1    | 1    | 1    |
| 6         | 5   | 5   | 1   | 5   | 1   | 5   | 6   | 6   | 6    | 5    | 5    | 1    | 4    | 1    | 1    | 1    | 5    | 1    | 1    | 6    | 1    | 6    | 1    | 1    |
| 1         | 6   | 1   | 6   | 2   | 3   | 5   | 1   | 5   | 6    | 1    | 1    | 6    | 1    | 6    | 1    | 6    | 5    | 6    | 1    | 1    | 2    | 1    | 1    | 6    |
| 3         | 2   | 1   | 1   | 5   | 1   | 6   | 6   | 2   | 3    | 6    | 1    | 6    | 1    | 1    | 6    | 6    | 6    | 6    | 4    | 6    | 2    | 1    | 2    | 5    |
| 5         | 1   | 3   | 1   | 6   | 5   | 6   | 5   | 1   | 1    | 6    | 6    | 2    | 1    | 2    | 1    | 6    | 6    | 2    | 1    | 6    | 1    | 1    | 6    | 5    |
| 1         | 1   | 6   | 1   | 6   | 1   | 1   | 5   | 6   | 6    | 1    | 3    | 1    | 1    | 1    | 4    | 2    | 5    | 4    | 1    | 3    | 5    | 3    | 1    | 5    |
| 2         | 1   | 4   | 4   | 5   | 1   | 6   | 1   | 6   | 2    | 1    | 2    | 1    | 2    | 5    | 3    | 1    | 6    | 1    | 1    | 6    | 6    | 2    | 6    | 6    |
| 5         | 5   | 2   | 6   | 6   | 2   | 1   | 1   | 5   | 1    | 1    | 3    | 6    | 1    | 6    | 6    | 4    | 1    | 6    | 1    | 2    | 1    | 2    | 1    | 6    |
| 5         | 6   | 1   | 1   | 5   | 1   | 1   | 1   | 6   | 6    | 1    | 2    | 5    | 1    | 1    | 5    | 1    | 6    | 2    | 1    | 1    | 1    | 2    | 5    | 5    |
| 1         | 3   | 1   | 6   | 1   | 3   | 1   | 6   | 6   | 2    | 3    | 6    | 1    | 3    | 3    | 1    | 6    | 6    | 1    | 1    | 1    | 6    | 6    | 2    | 1    |
| 1         | 1   | 5   | 6   | 1   | 1   | 1   | 6   | 1   | 1    | 6    | 1    | 6    | 1    | 4    | 6    | 1    | 5    | 6    | 6    | 2    | 6    | 6    | 1    | 6    |
| 6         | 5   | 1   | 2   | 6   | 6   | 1   | 1   | 5   | 3    | 1    | 1    | 1    | 6    | 1    | 1    | 1    | 1    | 1    | 1    | 1    | 6    | 1    | 5    | 6    |
| 1         | 1   | 6   | 1   | 1   | 1   | 1   | 3   | 6   | 1    | 6    | 6    | 1    | 4    | 2    | 6    | 1    | 2    | 5    | 6    | 6    | 1    | 2    | 2    | 6    |
| 1         | 6   | 1   | 3   | 1   | 6   | 1   | 1   | 1   | 4    | 1    | 2    | 1    | 1    | 1    | 6    | 6    | 1    | 5    | 6    | 4    | 1    | 5    | 1    | 5    |
| 1         | 6   | 6   | 6   | 6   | 6   | 1   | 1   | 6   | 1    | 1    | 5    | 1    | 3    | 1    | 1    | 6    | 6    | 6    | 6    | 1    | 5    | 6    | 5    | 1    |
| 6         | 4   | 1   | 3   | 6   | 1   | 5   | 2   | 1   | 1    | 6    | 1    | 2    | 2    | 5    | 1    | 1    | 6    | 1    | 6    | 2    | 6    | 5    | 6    | 6    |
| 1         | 1   | 5   | 6   | 5   | 1   | 1   | 6   | 5   | 6    | 1    | 1    | 1    | 1    | 3    | 6    | 2    | 5    | 5    | 3    | 2    | 5    | 1    | 1    | 5    |
| 1         | 5   | 6   | 6   | 2   | 1   | 6   | 6   | 6   | 1    | 1    | 1    | 1    | 1    | 6    | 1    | 5    | 1    | 1    | 1    | 2    | 5    | 1    | 1    | 5    |
| 5         | 5   | 1   | 5   | 1   | 1   | 2   | 2   | 1   | 6    | 6    | 1    | 2    | 5    | 5    | 1    | 1    | 1    | 4    | 1    | 5    | 4    | 1    | 1    | 5    |
| 1         | 1   | 1   | 1   | 1   | 1   | 1   | 6   | 6   | 2    | 1    | 3    | 3    | 1    | 1    | 1    | 2    | 6    | 1    | 2    | 1    | 1    | 6    | 3    | 6    |
| 6         | 1   | 6   | 1   | 1   | 1   | 4   | 1   | 6   | 6    | 1    | 1    | 1    | 5    | 6    | 2    | 1    | 6    | 1    | 1    | 1    | 5    | 4    | 4    | 2    |
| 1         | 6   | 1   | 5   | 1   | 1   | 5   | 6   | 1   | 1    | 1    | 1    | 4    | 4    | 1    | 1    | 1    | 1    | 6    | 1    | 1    | 1    | 6    | 1    | 6    |
| 1         | 6   | 1   | 5   | 1   | 1   | 5   | 5   | 1   | 3    | 1    | 6    | 1    | 3    | 6    | 5    | 5    | 6    | 1    | 1    | 5    | 1    | 3    | 4    | 1    |
| 6         | 6   | 3   | 6   | 5   | 6   | 1   | 3   | 1   | 5    | 1    | 5    | 5    | 1    | 1    | 5    | 1    | 2    | 1    | 6    | 5    | 1    | 6    | 1    | 1    |
| 5         | 1   | 5   | 6   | 1   | 1   | 1   | 1   | 6   | 2    | 6    | 5    | 1    | 1    | 1    | 2    | 1    | 5    | 6    | 1    | 6    | 5    | 1    | 5    | 5    |
| 2         | 3   | 5   | 6   | 6   | 6   | 5   | 5   | 1   | 6    | 1    | 1    | 5    | 5    | 6    | 6    | 6    | 6    | 1    | 6    | 1    | 1    | 1    | 1    | 1    |
| 1         | 6   | 1   | 1   | 6   | 2   | 1   | 1   | 1   | 1    | 1    | 1    | 1    | 1    | 3    | 2    | 6    | 4    | 1    | 6    | 6    | 1    | 1    | 1    | 3    |
| 1         | 3   | 3   | 5   | 4   | 5   | 1   | 3   | 5   | 1    | 6    | 1    | 1    | 5    | 5    | 6    | 1    | 2    | 1    | 1    | 5    | 5    | 6    | 6    | 1    |
| 1         | 1   | 6   | 6   | 2   | 6   | 6   | 5   | 5   | 4    | 2    | 6    | 6    | 6    | 5    | 5    | 6    | 2    | 2    | 1    | 6    | 1    | 5    | 6    | 5    |
| 6         | 5   | 6   | 1   | 1   | 3   | 4   | 2   | 6   | 1    | 1    | 3    | 1    | 5    | 5    | 6    | 4    | 3    | 4    | 1    | 6    | 5    | 1    | 5    | 1    |
| 5         | 1   | 6   | 1   | 6   | 6   | 6   | 6   | 1   | 5    | 4    | 5    | 6    | 1    | 5    | 1    | 5    | 1    | 5    | 1    | 6    | 6    | 1    | 4    | 6    |
| 1         | 6   | 1   | 1   | 6   | 1   | 1   | 6   | 6   | 6    | 5    | 2    | 1    | 1    | 5    | 6    | 2    | 4    | 1    | 5    | 6    | 5    | 5    | 1    | 1    |
| 6         | 1   | 6   | 2   | 4   | 3   | 1   | 6   | 2   | 1    | 6    | 6    | 5    | 4    | 1    | 1    | 5    | 1    | 3    | 6    | 1    | 1    | 1    | 6    | 1    |
| 2         | 1   | 6   | 2   | 1   | 4   | 5   | 2   | 6   | 1    | 2    | 1    | 6    | 1    | 1    | 6    | 6    | 2    | 6    | 5    | 6    | 1    | 2    | 5    | 4    |
| 4         | 2   | 4   | 1   | 2   | 5   | 1   | 5   | 2   | 1    | 1    | 1    | 6    | 1    | 1    | 6    | 6    | 5    | 2    | 1    | 5    | 2    | 1    | 1    | 1    |
| 1         | 6   | 6   | 6   | 1   | 2   | 3   | 1   | 1   | 5    | 6    | 1    | 2    | 4    | 2    | 3    | 1    | 1    | 1    | 1    | 4    | 1    | 1    | 5    | 1    |
| 6         | 6   | 4   | 6   | 6   | 5   | 2   | 1   | 1   | 1    | 3    | 2    | 1    | 6    | 6    | 1    | 1    | 5    | 6    | 4    | 1    | 1    | 5    | 6    | 6    |
| 6         | 1   | 3   | 1   | 2   | 3   | 5   | 3   | 2   | 2    | 6    | 3    | 1    | 1    | 5    | 5    | 6    | 6    | 3    | 6    | 2    | 6    | 6    | 6    | 6    |
| 2         | 5   | 6   | 6   | 1   | 5   | 1   | 6   | 1   | 1    | 6    | 5    | 1    | 3    | 1    | 2    | 6    | 6    | 1    | 1    | 1    | 1    | 3    | 3    | 1    |
| 6         | 1   | 6   | 1   | 5   | 6   | 2   | 6   | 6   | 5    | 2    | 5    | 5    | 6    | 6    | 5    | 5    | 2    | 6    | 1    | 4    | 6    | 1    | 3    | 4    |
| 1         | 5   | 3   | 6   | 6   | 1   | 1   | 1   | 6   | 1    | 2    | 3    | 6    | 5    | 6    | 1    | 4    | 2    | 1    | 6    | 1    | 5    | 5    | 1    | 6    |
| 1         | 6   | 5   | 6   | 5   | 1   | 6   | 5   | 5   | 1    | 1    | 3    | 6    | 6    | 2    | 5    | 1    | 4    | 3    | 2    | 1    | 1    | 1    | 6    | 2    |
| 3         | 2   | 1   | 1   | 3   | 6   | 1   | 5   | 6   | 2    | 2    | 1    | 6    | 1    | 1    | 1    | 2    | 3    | 1    | 6    | 1    | 5    | 1    | 1    | 1    |
| 6         | 6   | 5   | 1   | 2   | 1   | 6   | 3   | 1   | 1    | 3    | 5    | 1    | 6    | 3    | 1    | 5    | 5    | 5    | 6    | 1    | 2    | 6    | 5    | 3    |
| 1         | 1   | 4   | 1   | 1   | 1   | 5   | 3   | 6   | 1    | 1    | 6    | 1    | 6    | 6    | 5    | 1    | 6    | 5    | 1    | 1    | 1    | 2    | 1    | 6    |
| 5         | 1   | 6   | 1   | 5   | 6   | 6   | 2   | 1   | 5    | 1    | 2    | 5    | 1    | 5    | 4    | 4    | 3    | 4    | 6    | 6    | 6    | 6    | 1    | 6    |
| 1         | 1   | 1   | 4   | 5   | 5   | 1   | 6   | 1   | 1    | 2    | 1    | 1    | 6    | 3    | 4    | 6    | 6    | 2    | 6    | 5    | 1    | 5    | 1    | 1    |
| 1         | 1   | 6   | 5   | 1   | 6   | 5   | 5   | 6   | 5    | 6    | 6    | 2    | 3    | 1    | 1    | 1    | 1    | 1    | 1    | 6    | 3    | 1    | 1    | 6    |
| 1         | 1   | 6   | 4   | 6   | 1   | 1   | 5   | 3   | 1    | 6    | 1    | 1    | 6    | 1    | 6    | 1    | 3    | 1    | 6    | 1    | 4    | 1    | 6    | 6    |
| 1         | 2   | 1   | 6   | 5   | 1   | 4   | 2   | 1   | 6    | 1    | 1    | 1    | 6    | 1    | 2    | 6    | 2    | 1    | 5    | 1    | 4    | 1    | 5    | 1    |
| 4         | 5   | 5   | 5   | 3   | 6   | 1   | 1   | 6   | 1    | 5    | 1    | 4    | 6    | 5    | 5    | 5    | 1    | 1    | 1    | 1    | 6    | 6    | 4    | 6    |
| 3         | 6   | 6   | 5   | 4   | 1   | 1   | 4   | 1   | 5    | 1    | 6    | 1    | 6    | 2    | 5    | 1    | 6    | 1    | 1    | 6    | 5    | 5    | 1    | 1    |
| 1         | 1   | 2   | 5   | 1   | 1   | 5   | 1   | 5   | 3    | 2    | 5    | 5    | 6    | 1    | 5    | 1    | 1    | 4    | 1    | 1    | 1    | 1    | 6    | 1    |
| 6         | 6   | 2   | 1   | 6   | 2   | 6   | 6   | 5   | 2    | 6    | 3    | 1    | 1    | 4    | 6    | 6    | 2    | 1    | 1    | 5    | 3    | 5    | 5    | 1    |
| 1         | 6   | 3   | 2   | 1   | 5   | 6   | 3   | 6   | 3    | 6    | 4    | 1    | 3    | 5    | 5    | 5    | 1    | 1    | 6    | 5    | 1    | 2    | 1    | 4    |
| 1         | 6   | 1   | 5   | 1   | 5   | 1   | 1   | 1   | 3    | 1    | 1    | 1    | 1    | 2    | 6    | 1    | 1    | 4    | 1    | 2    | 6    | 3    | 1    | 6    |
| 1         | 1   | 1   | 5   | 4   | 5   | 5   | 2   | 6   | 5    | 1    | 1    | 1    | 1    | 1    | 1    | 1    | 1    | 2    | 5    | 1    | 1    | 2    | 1    | 2    |
| 5         | 1   | 1   | 6   | 2   | 1   | 1   | 6   | 4   | 6    | 1    | 5    | 4    | 6    | 2    | 6    | 2    | 1    | 1    | 2    | 3    | 1    | 1    | 1    | 1    |
| 2         | 1   | 1   | 5   | 6   | 5   | 1   | 5   | 1   | 2    | 1    | 1    | 6    | 6    | 1    | 1    | 1    | 3    | 4    | 1    | 1    | 4    | 1    | 1    | 2    |
| 1         | 5   | 1   | 6   | 1   | 1   | 1   | 1   | 3   | 1    | 6    | 1    | 2    | 5    | 1    | 1    | 6    | 1    | 5    | 6    | 1    | 4    | 6    | 5    | 1    |
| 6         | 1   | 1   | 1   | 5   | 1   | 1   | 6   | 6   | 5    | 5    | 2    | 1    | 4    | 1    | 1    | 3    | 4    | 1    | 1    | 1    | 6    | 3    | 1    | 1    |
| 1         | 2   | 1   | 1   | 6   | 6   | 5   | 1   | 2   | 3    | 6    | 6    | 6    | 1    | 2    | 1    | 3    | 6    | 6    | 6    | 6    | 1    | 6    | 5    | 6    |
| 1         | 6   | 2   | 5   | 1   | 3   | 2   | 3   | 3   | 2    | 4    | 3    | 2    | 5    | 3    | 1    | 1    | 4    | 4    | 6    | 1    | 5    | 4    | 1    | 2    |
| 1         | 1   | 5   | 6   | 3   | 1   | 1   | 6   | 1   | 1    | 1    | 6    | 2    | 4    | 2    | 6    | 2    | 2    | 3    | 6    | 6    | 1    | 5    | 1    | 1    |
| 6         | 1   | 1   | 6   | 1   | 6   | 3   | 1   | 6   | 5    | 1    | 5    | 4    | 2    | 6    | 6    | 1    | 5    | 1    | 6    | 6    | 6    | 6    | 6    | 1    |
| 6         | 3   | 1   | 1   | 6   | 1   | 3   | 6   | 5   | 3    | 5    | 1    | 1    | 1    | 1    | 4    | 5    | 1    | 6    | 6    | 1    | 5    | 1    | 1    | 2    |
| 1         | 6   | 1   | 1   | 2   | 6   | 5   | 1   | 6   | 6    | 6    | 3    | 1    | 6    | 4    | 1    | 6    | 1    | 6    | 1    | 6    | 3    | 1    | 6    | 1    |
| 2         | 1   | 1   | 4   | 1   | 2   | 4   | 3   | 6   | 2    | 5    | 6    | 1    | 1    | 6    | 1    | 5    | 5    | 1    | 1    | 2    | 6    | 1    | 6    | 6    |
| 2         | 1   | 2   | 1   | 5   | 2   | 6   | 5   | 5   | 1    | 6    | 6    | 5    | 2    | 1    | 4    | 1    | 4    | 6    | 2    | 1    | 6    | 4    | 1    | 1    |
| 3         | 1   | 1   | 6   | 5   | 5   | 6   | 1   | 5   | 5    | 1    | 2    | 4    | 6    | 4    | 5    | 1    | 1    | 6    | 1    | 2    | 1    | 5    | 6    | 6    |
| 2         | 6   | 6   | 6   | 1   | 1   | 6   | 6   | 5   | 6    | 1    | 6    | 1    | 1    | 1    | 3    | 1    | 6    | 1    | 4    | 1    | 1    | 3    | 6    | 6    |
| 1         | 6   | 1   | 5   | 5   | 1   | 6   | 1   | 4   | 3    | 2    | 1    | 2    | 2    | 5    | 6    | 1    | 1    | 1    | 1    | 1    | 5    | 6    | 1    | 2    |
| 6         | 6   | 6   | 6   | 6   | 1   | 6   | 3   | 1   | 1    | 1    | 4    | 6    | 5    | 6    | 1    | 1    | 1    | 6    | 5    | 6    | 1    | 5    | 1    | 1    |
| 2         | 3   | 4   | 5   | 5   | 3   | 1   | 5   | 4   | 5    | 6    | 5    | 1    | 3    | 1    | 5    | 1    | 2    | 4    | 5    | 5    | 3    | 1    | 1    | 5    |
| 1         | 2   | 6   | 5   | 1   | 6   | 6   | 5   | 6   | 6    | 2    | 1    | 1    | 5    | 2    | 1    | 6    | 2    | 1    | 1    | 1    | 6    | 1    | 1    | 6    |
| 3         | 2   | 1   | 1   | 1   | 6   | 6   | 1   | 2   | 6    | 1    | 5    | 5    | 2    | 3    | 5    | 5    | 5    | 2    | 6    | 1    | 1    | 1    | 4    | 5    |
| 6         | 4   | 5   | 6   | 1   | 5   | 1   | 1   | 1   | 1    | 5    | 1    | 2    | 1    | 2    | 1    | 1    | 2    | 4    | 1    | 6    | 1    | 1    | 5    | 1    |
| 6         | 6   | 6   | 6   | 1   | 1   | 1   | 1   | 1   | 4    | 4    | 1    | 1    | 1    | 4    | 6    | 5    | 6    | 6    | 5    | 1    | 6    | 3    | 1    | 6    |
| 6         | 1   | 4   | 6   | 6   | 6   | 1   | 4   | 5   | 6    | 2    | 1    | 6    | 6    | 2    | 1    | 1    | 1    | 5    | 5    | 6    | 6    | 3    | 2    | 2    |
| 6         | 6   | 1   | 2   | 2   | 6   | 5   | 1   | 5   | 1    | 1    | 1    | 6    | 6    | 3    | 1    | 1    | 6    | 1    | 1    | 1    | 1    | 1    | 6    | 2    |
| 1         | 6   | 5   | 1   | 2   | 6   | 5   | 1   | 2   | 1    | 6    | 6    | 1    | 1    | 5    | 1    | 6    | 5    | 6    | 5    | 5    | 5    | 1    | 1    | 1    |
| 5         | 1   | 5   | 6   | 6   | 1   | 3   | 2   | 1   | 5    | 1    | 1    | 1    | 1    | 1    | 1    | 3    | 1    | 5    | 3    | 1    | 6    | 4    | 4    | 6    |
| 2         | 1   | 5   | 4   | 1   | 1   | 6   | 1   | 6   | 1    | 2    | 6    | 5    | 1    | 6    | 6    | 2    | 2    | 6    | 6    | 1    | 4    | 1    | 1    | 6    |
| 1         | 6   | 1   | 5   | 1   | 1   | 6   | 1   | 2   | 5    | 2    | 2    | 2    | 1    | 5    | 5    | 5    | 1    | 4    | 6    | 2    | 3    | 1    | 1    | 1    |
| 3         | 6   | 5   | 2   | 2   | 1   | 1   | 5   | 1   | 6    | 1    | 1    | 1    | 1    | 2    | 1    | 6    | 6    | 6    | 1    | 1    | 6    | 1    | 1    | 5    |
| 5         | 6   | 6   | 6   | 1   | 1   | 1   | 1   | 5   | 6    | 5    | 6    | 1    | 6    | 6    | 6    | 1    | 6    | 2    | 2    | 6    | 5    | 5    | 1    | 6    |
| 5         | 1   | 5   | 1   | 1   | 1   | 4   | 1   | 2   | 1    | 6    | 1    | 5    | 5    | 1    | 6    | 6    | 4    | 5    | 1    | 6    | 5    | 1    | 1    | 5    |
| 1         | 6   | 6   | 6   | 1   | 2   | 6   | 6   | 6   | 2    | 1    | 5    | 4    | 6    | 6    | 1    | 1    | 1    | 6    | 6    | 1    | 2    | 4    | 1    | 1    |
| 2         | 5   | 6   | 1   | 3   | 1   | 6   | 1   | 5   | 1    | 6    | 6    | 5    | 6    | 1    | 1    | 6    | 1    | 4    | 3    | 6    | 4    | 1    | 5    | 4    |
| 1         | 5   | 6   | 1   | 4   | 2   | 5   | 6   | 1   | 4    | 5    | 1    | 1    | 6    | 1    | 6    | 6    | 3    | 6    | 1    | 1    | 5    | 5    | 2    | 1    |
| 2         | 6   | 5   | 6   | 1   | 6   | 1   | 5   | 1   | 1    | 1    | 1    | 1    | 1    | 6    | 4    | 1    | 5    | 1    | 5    | 1    | 2    | 3    | 1    | 1    |
| 1         | 1   | 6   | 2   | 6   | 6   | 6   | 1   | 6   | 5    | 6    | 1    | 5    | 1    | 2    | 4    | 3    | 1    | 5    | 6    | 6    | 1    | 6    | 6    | 4    |
| 1         | 2   | 5   | 1   | 6   | 1   | 3   | 6   | 1   | 1    | 2    | 6    | 1    | 1    | 6    | 5    | 1    | 2    | 2    | 1    | 5    | 5    | 1    | 4    | 2    |
Here are the averages aggregated. We also put the data from the sets of 4 samples from earlier.

| Bins     | Sets of 4 | Sets of 25 |
| -------- | --------- | ---------- |
| 1-1.49   | 6         | 6          |
| 1.5-1.99 | 5         | 5          |
| 2-2.49   | 14        | 9          |
| 2.5-2.99 | 17        | 18         |
| 3-3.49   | 13        | 20         |
| 3.5-3.99 | 17        | 16         |
| 4-4.49   | 11        | 13         |
| 4.5-4.99 | 12        | 7          |
| 5-5.49   | 4         | 2          |
| 5.5-6    | 1         | 4          |

^22a06a

```chart
type: line
labels: []
series:
  - title: 
    data: []
id: 22a06a
tension: 0.2
width: 80%
labelColors: false
fill: false
beginAtZero: true
bestFit: false
bestFitTitle: undefined
bestFitNumber: 0
```

As can be seen, the larger sample size (in <span style="color:rgb(0, 176, 240)">teal</span>) is tighter and looks more like a normal distribution. ^a626ed
# Distribution of Means of Samples from Distribution
*This is officially called the "sample distribution of the sample mean"*
## Definition
<span style="display: block; text-align: justify;">We start off with a random distribution. If I theoretically take an infinite amount of samples, all of the same size, from this distribution, and find the means of these samples, this will create its own distribution.</span>
## Getting a Normal Distribution for the Distribution of Sample Means
### Non-Bernoulli Random Variables
The shape of the distribution of sample means will be normal if one of the following is true:
1. <span style="display: block; text-align: justify;">It came from a normal distribution. <span style="color:rgb(255, 0, 0)">While this does seem intuitive, I don't think I have a good explanation for why this is.</span></span>
2. <span style="display: block; text-align: justify;">There is a somewhat large sample size. The "rule of thumb" is to say that this is 30 or more. However, if the original distribution is extremely skewed, this will not work and you will require more samples.
   This is true because of the Central Limit Theorem. As discussed above, as the sample size approaches infinity the distribution of the means of the samples will begin approximate a normal distribution. As such, as long as we have a "large" sample size, we will start to see this.</span>
### Bernoulli Random Variables
For Bernoulli Trials, we say that the following two things need to be true to get a normal distribution:
$$(sample \space size) \times (probability) \ge 10$$
and:
$$(sample \space size) \times (1-probability) \ge 10$$
This is generally just written as:
$$np \ge 10$$
and:
$$n(1-p) \ge 10$$
#### Intuition
The basic intuition is that the more likely or less likely something is, the more the mean moves in one direction or the other, and the "less room" there is for the data to on the "small size". This will make the distribution "have a tail".
However, if we have a larger sample size, the data "tightens up" around the mean and so there is enough room to fit the data. This makes the graph look normal.
For example, let's say that a certain event has a 90% probability and we take 10 samples. The probability distribution for the ratio of successes looks like this (there are two graphs, but they represent the same data.):
![[Pasted image 20260126221627.png]]
![[Pasted image 20260126221706.png]]
As can be seen, the data has a long tail to the left. There isn't a lot of "room" for data above the mean (which is at 90% successes, or 9 successes).
Here is the data when we run 100 trials (once again, with two graphs):
![[Pasted image 20260126221840.png]]
![[Pasted image 20260126221853.png]]
Over here, the graph looks like a normal distribution. Because there is a much larger sample size, the data is much tighter around the mean (90%, or, in this case, 90 successes). There is enough "room" above the mean.
(Side note: even though in these graphs it looks like the probability of getting a value toward the left is 0, that is certainly not actually the case. The probability is low, but it is impossible for it to be 0. The reason it looks that way is because the scale of the graph is too large. If we would make the scale of the graph smaller, the probabilities would be seen.)

### Difference Between Bernoulli and non-Bernoulli Random Variables
There isn't really an actual "magical difference" in the underlying reasoning for the "rules" for getting a normal distribution for the distribution of sample means between Bernoulli and non-Bernoulli random variables.
The reason why the rules in *actuality* are different is because of the following:
As for the first rule (if the underlying distribution is normal, the sampling distribution of the sample mean will be normal) this is only possible by non-Bernoulli random variables.
As for the second rule (the sample size is at least 30) that is similar in concept to the $np \ge 10$ and $n(1-p) \ge 10$ rule by Bernoulli random variables but more crude. As mentioned before, having a large sample size will allow the Central Limit Theorem to start making the sampling distribution of the sample mean normal. However how large it has to be depends on how skewed the distribution is. Taking a sample size of at least 30 will do fine for many distributions but not fine for others.
Since we know more about Bernoulli random variables (we know that there are exactly 2 possible outcomes) it is easier to give a rule that can incorporate the skewedness. As explained before, the $np \ge 10$ and $n(1-p) \ge 10$ rule by Bernoulli random variables does take this into account and gives you a sample size that adjusts for the skewedness.
## Mean
The distribution of the means of the samples of our original distribution will have the same mean as the original distribution, regardless of the size of the sets of the samples.
For Bernoulli random variables, that is the same as $p$.
## [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]] And [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]]
### Variance
#### Formula
<span style="display: block; text-align: justify;">$$\frac{\sigma^2}{n}$$
($\sigma^2$ is the variance of the population and $n$ is the size of the sets of samples.)</span>
<span style="display: block; text-align: justify;">For Bernoulli Trials, this is going to be $\frac{p(1-p)}{n}$ (because the variance is $p(1-p)$).</span>
#### Proof
The sampling distribution of the sample mean can be thought of in the following way:
1. I take a specific amount of random samples from a distribution.
2. I add them all up.
3. I divide by the amount of selections I made.
4. I repeat this a theoretically infinite number of times.

When I look at any specific number picked in the infinite samples, the variance will be, by definition: $\sigma^2$ (the variance of the original distribution).
In other words, if I look at the first selection in all of my sets of samples, the variance for the first selections will be $\sigma^2$. The same will be true for the second selection in each set, as well as the third, fourth, fifth, etc.
When I add all of these selections together and take the variances of totals of all of the sets (in other words, I add up all of the selections for each set, and then calculate the variance of these totals), the variance is going to be $n\sigma^2$ (where $n$ is the sample size).
This is because of what was discussed [[Adjusting and Combining Random Variables#Variance|here]], that when we add random variables together, the variance of the total is equal to the variance of each individual random variable added together. In our situation, since we have $n$ random variables in each set, and the variance for each one of these is $\sigma^2$, and we are adding these variances together, the total is going to be $n\sigma^2$.
However, we are not done. We aren't looking for the variance of the distribution of the *totals* of the samples, we are looking for the variance of the distribution of the *means* of the samples. As such, we need to divide the total of each sample by the amount of selections that there are (which is $n$) and find the variance of this. This is going to look something like this:

$$Var\left(\frac{X_1+X_2+…+X_n}{n}\right)$$

(Where each $X$ ($X_1, X_2,…,X_n$) represents all of the 1st, 2nd, 3rd, etc. selections of each set. We then add them up, divide by the sample size ($n$) and then get the variance of that.)
Using a drop of algebra, this is the same as:

$$Var\left(\frac{X_1}{n}+\frac{X_2}{n}+…+\frac{X_n}{n}\right)$$

As discussed [[Adjusting and Combining Random Variables#Multiplying Constant to Random Variables|here]], when multiplying each value in a random variable by a constant, the variance for the random variable will change by the constant, squared. In this case, the variance of just the numerators is $n\sigma^2$, as discussed. Now, however, we are dividing each individual value by a constant (namely, $n$). As such, the variance shrinks by $n^2$. This becomes:
$$\frac{n\sigma^2}{n^2} \Rightarrow \boxed{\frac{\sigma^2}{n}}$$
#### Some Intuition
The greater the sample size, the more $n$ increases, so the smaller the value of the fraction is. This means that the values cluster around the mean more, as discussed [[#Definition|here]] and [[#^a626ed|here]].
### Standard Deviation
The standard deviation is just the square root of the variance. As such, that is:

$$\sqrt{\frac{\sigma^2}{n}} \Rightarrow \frac{\sqrt{\sigma^2}}{\sqrt{n}} = \boxed{\frac{\sigma}{\sqrt{n}}}$$

For Bernoulli random variables, this is going to be $\frac{\sqrt{p(1-p)}}{\sqrt{n}}$ (the [[Bernoulli Trial#Standard Deviation|standard deviation of a Bernoulli random variable]] is $\sqrt{p(1-p)}$), which is the same as $\sqrt{\frac{p(1-p)}{n}}$ or $\frac{\sqrt{np(1-p)}}{n}$.