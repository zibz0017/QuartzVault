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
# Calculating Population Mean from Sample (Confidence Intervals)
## Calculation
We can estimate a population mean based off the mean of a sample, based off a few points previously discussed.
As mentioned [[#Mean|above]] the mean of the actual population will be the same as the mean of the distribution of the means of the samples.
Assuming that the sample distributions are normal (see [[#Getting a Normal Distribution for the Distribution of Sample Means|above]] for the parameters for when we assume that), and that the selections are independent (see [[#Achieving Independence between Selections|above]]) we can calculate the probability that the sample mean is within 1 standard deviation, or 2 standard deviation, or 2.5 standard deviation, etc. of the mean of the distribution of the means of the samples. And since the mean of the distribution of the means of the samples and the actual population mean are the same, this means that we can calculate the likelihood of how close or how far the sample mean is from the population mean.
For example, approximately 95% of sample means will be within 2 standard deviations of the mean of the distribution of the means of the samples, the same way we know that for any normal distribution, a randomly selected value will be within 2 standard deviations of the mean, as discussed [[Density Curve#Empirical Rule (68-95-99.7 Rule)|here]]. In other words, the sample mean of a random sample will be within 2 standard deviations of the mean of the distribution of the sample means 95% of the time. And since the mean of the distribution of the sample means is the same as the population mean, the sample mean of a random sample will be within 2 standard deviations of the population mean. This means that if we can calculate the standard deviation, we will be able to calculate a range for the population proportion (with a certain degree of confidence).
However, the [[#Standard Deviation|formula for calculating the standard deviation of the distribution of the samples]] is based actual population standard deviation and we don't know that.
However, we can estimate the population standard deviation using the sample, as discussed [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Steps to Find Sample Variance (s 2)|here]]. We will use that in our formula in place of the population standard deviation to calculate an estimate of the standard deviation of the distribution of the sample means. This estimate of the standard deviation of the distribution of the sample means is called the standard error.
We can use this to calculate a range of possibilities for the population proportion. For example, if we wanted to create a range that we would know that the population proportion would be part of with 95% confidence, we would need to calculate around two standard errors above and below the sample mean. This is called the margin of error (meaning, the standard error multiplied by how many standard errors we would like to be able to achieve our degree of confidence).
The larger the sample size, the smaller the standard deviation is going to be ($n$, or the sample size, is in the denominator of the fraction). This means that if we want to make the standard deviation smaller (and hence, the estimate of the population proportion to be more specific) we need to increase the sample size. ^59e303
### "Shortcut" for Bernoulli Random Variables
The standard deviation for a Bernoulli random variable is $p(1-p)$. As discussed [[Bernoulli Trial#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance and Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|here]], this is simplified from the regular standard deviation formula (getting the distances from the mean, squaring them, adding them together, dividing by $n$, and getting the square root). However, this assumes that we are dividing by $n$. In our situation, we are estimating the standard deviation of the population from the sample and so we have to use $n-1$ (Bessel's Correction) as [[#^59e303|just discussed]]. Technically, this simplification to $p(1-p)$ does not work in this situation. However, if the sample is large, the difference between $n$ and $n-1$ becomes very small and so, in most situations, the difference will not matter. As such, one can use $p(1-p)$ as the standard deviation of the Bernoulli random variable (and use that as an estimate of the population standard deviation).
### Sampling from a Finite Population (Finite Population Correction)
When sampling something, we will usually be sampling from a population with finite size (for example, we may be sampling voting patterns in a certain population. There are a finite amount of people in that population) and we are not going to be replacing the people that we sample (in the above example, once we ask someone how they are voting, we are not going to ask them again). This allows us to get get even tighter confidence intervals.
Intuitively, this makes sense. If there are 100 people in our population and we sample all 100 of them, we know with 100% certainty the exact distribution. There is no "range of values" or "degree of confidence".
Similarly, even if we don't sample everyone, the greater percentage of the population we sample, the less the means of samples can move around.
For example, let's say I have a population of 100 people and I sample 94 of the them and I get 47 successes and 47 failures, I know that the population can range from 53 successes against 47 failures, to 47 successes against 53 failures. And I also know that the extremes are unlikely as it is very unlikely that all of the people I didn't sample happened to all be the same thing (in this example where the population proportion is basically 50/50. It's basically as likely as flipping 6 heads or 6 tails in a row). In other words, because we basically sampled the whole population, the standard error is going to be very small.
#### Formula
One takes this into account by multiplying the standard error by the Finite Population Correction formula. This is:
$$\text{FPC} = \sqrt{\frac{N-n}{N-1}}$$
*($N$ is the population size and *n* is the sample size.)*
#### Some Intuition with Examples
As $N$ increases compared to $n$, the less of a difference $n$ makes. For example, let's say $N=10000$ and $n=10$, this is going to equal:
$$\sqrt{\frac{10000-10}{10000-1}} = \sqrt{\frac{99990}{99999}} \approx \sqrt{.99991} \approx \boxed .99995$$
As can be seen, this basically equals $1$. When me multiply the standard error by this number, it basically won't change. The fact that this population is finite doesn't really help us get a more precise estimate.
Conversely, as $n$ approaches the size of $N$, this will approach $0$. For example, let's say that $N=10000$ and $n=9500$, this becomes:
$$\sqrt{\frac{10000-9500}{10000-1}} = \sqrt{\frac{500}{9999}} \approx \sqrt{.05} \approx \boxed{.223}$$
In other words, we can shrink the standard error by nearly 80%. And if $n$ is even closer to $N$, the effects get stronger. For example, if $N=10000$ and $n=9990$, this becomes:
$$\sqrt{\frac{10000-9990}{10000-1}} = \sqrt{\frac{10}{9999}} \approx \sqrt{.001} \approx \boxed{.032}$$
And if $N$ and $n$ are equal, the fraction will equal $0$. The numerator is $N-n$. If $N$ and $n$ are equal, this will equal $0$. In other words, there will be no error at all. We will have the exact population proportion.
#### 10% Rule of Independence
There is a "rule of thumb" that if the sample size is 10% or less than the population size, we ignore the finite population correction. At such a small percentage, correcting for the fact that we are dealing with a finite population will barely make a difference which is barely worth it in most real-life situations.
## Example
We take a random sample of 100 people from a certain population and 75% say that they like vanilla ice cream and 25% say that they do not. We want to try and calculate a confidence interval with 95% confidence for what the population proportion is.
### Using the "Shortcut"
*Note: We are only able to use the shortcut because this is a Bernoulli random variable. This does not work for non-Bernoulli random variables.*

The sample proportion is .75, so the standard deviation of the sample is:

$$.75 \times (1-.75)$$

To calculate the standard error, we use this in place of the population standard deviation to calculate the standard deviation of the distribution of the means of samples. As [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation#formula|discussed above]], we just need to divide by $n$ (which is 100) and then take the square root, like so:
$$\sqrt{\frac{.75 \times (1-.75)}{100}} \Rightarrow \sqrt{\frac{.75 \times .25}{100}} \approx \boxed{.043}$$
Now that we have our standard error, we need to calculate two standard errors above and below the sample proportion (our margin of error) and we will have a range of different values for the population proportion (with 95% certainty).
This becomes:
$$.75 + (.043 *2) \Rightarrow .75 + (.086) = \boxed{.836}$$
$$.75 - (.043*2) \Rightarrow .75 - (.086) = \boxed{.664}$$
We can say with 95% confidence that between 67.4% and 83.6% of people in this population like vanilla ice cream.
As noted, if we want to make this range smaller, we would have to get a larger sample.
For example, let's say we sampled 250 people and got 75% of people who said that they liked vanilla ice cream, the standard error would be:
$$\sqrt{\frac{.75 \times (1-.75)}{250}} \Rightarrow \sqrt{\frac{.75 \times .25}{250}} \approx \boxed{.027}$$
Two standard errors above and below would become:
$$.75 + (.027 *2) \Rightarrow .75 + (.054) = \boxed{.804}$$
$$.75 - (.027 *2) \Rightarrow .75 - (.054) = \boxed{.696}$$
In this case, we know with 95% certainty that the population proportion is between 69.6% and 80.4%.
### Using the "Regular" Method
We are trying to estimate the standard deviation of the population from a sample. As such, we have to get the square root of the squared distance of every sample from the mean, but then, instead of dividing by the sample size (to get the real average and the standard deviation for the sample we took), we divide by $n-1$, as discussed.
"Successes" are considered a $1$ and failures are a $0$. The mean is simply $p$, which in this case is $.75$.
There are $75$ successes and $25$ failures. We need to calculate the squared distance from the mean for each of these and add them together. For the successes, that becomes:
$$75 \times \left((1-.75)^2\right)$$
And for the failures:
$$25 \times \left((0-.75)^2\right)$$
We then add these together:
$$75 \times \left((1-.75)^2\right) + 25 \times \left((0-.75)^2\right) = 18.75$$
If we wanted to get the standard deviation of the sample, we would then divide this by the sample size. However, because we are using this as an estimate of the population standrad deviation, we divide this by $n-1$, as discussed. This becomes:
$$\frac{18.75}{100-1} \approx .189$$
Now we need to get the square root of this:
$$\sqrt{.189}= \boxed{.435}$$
This number is our approximation of the standard deviation of the population.
We can take this number and plug it into the formula for getting the standard deviation of the distribution of the means of samples. As discussed above, the formula is $\frac{\sigma}{\sqrt{n}}$. Plugging in the numbers, we get:
$$\frac{.435}{\sqrt{100}} \Rightarrow \frac{.435}{10} \approx \boxed{.044}$$
Since we are looking for 95% confidence, we need calculate 2 standard deviations above and 2 standard deviations below to create the range. For the upper bound, this is:
$$.75+(.044 \times 2) = \boxed{.838}$$
And for the lower bound:
$$.75-(.044 \times 2) = \boxed{.662}$$

As can be seen, using the "shortcut" resulted in nearly the exact same value as the "regular" method. They are approximately $.001$ apart.