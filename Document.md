# Matplotlib
#### A comprehensive Python library for data visualization

Latest Release: 3.4.3
Date: August 13, 2021

## Features

- High quality plots with a few lines of code
- Interactive plots that can zoom, update, pan and much more
- Full control of styles and properties
- Can be exported and embedded to many file formats and interactive environments

## Installation

Install the official release.

```sh
python -m pip install -U pip
python -m pip install -U matplotlib
```

### Third-Party Distributions
Some third-parties include Matplotlib
#### Conda

via the *Anaconda main channel*...
```sh
conda install matplotlib
```

...or the *conda-forge community channel*
```sh
conda install -c conda-forge matplotlib
```
The complete installation guide can be found [here](https://matplotlib.org/stable/users/installing.html)

---
## Scatter Plot

A scatter plot is generally used to plot data points to demonstrate the extent to which one variable is affected by the other.

Given here is a code which develops a scatter plot.
```sh
import matplotlib.pyplot as plt
x = [79, 90, 100, 59, 100, 80, 90, 70, 80, 34]
y = [30, 29, 49, 48, 100, 48, 38, 45, 20, 30]
range = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]
fig=plt.figure()
ax=fig.add_axes([0,0,1,1])
ax.scatter(range, x, color='r')
ax.scatter(range, y, color='b')
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('scatter plot')
plt.show()
```

#### Change axes color

The following code will change the color of the x-axis to blue...

```sh
ax.spines['bottom'].set_color('blue')
```

... and this will make the y-axis red

```sh
ax.spines['left'].set_color('red')
```