# Question 1
Question 1
Take a look at the 'iris' dataset that comes with R. The data can be loaded with the code:

```R
library(datasets)
data(iris)
```
A description of the dataset can be found by running
```
?iris
```

There will be an object called 'iris' in your workspace. In this dataset, what is the mean of 'Sepal.Length' for the species virginica? Please round your answer to the nearest whole number.

(Only enter the numeric result and nothing else.)

# Question 2
Continuing with the 'iris' dataset from the previous Question, what R code returns a vector of the means of the variables 'Sepal.Length', 'Sepal.Width', 'Petal.Length', and 'Petal.Width'?

* rowMeans(iris[, 1:4])
* apply(iris, 1, mean)
* apply(iris[, 1:4], 2, mean)
* apply(iris[, 1:4], 1, mean)
* colMeans(iris)
* apply(iris, 2, mean)

# Question 3
Load the 'mtcars' dataset in R with the following code

```
library(datasets)
data(mtcars)
```

There will be an object names 'mtcars' in your workspace. You can find some information about the dataset by running

```
?mtcars
```

How can one calculate the average miles per gallon (mpg) by number of cylinders in the car (cyl)? Select all that apply.

* split(mtcars, mtcars$cyl)
* apply(mtcars, 2, mean)
* with(mtcars, tapply(mpg, cyl, mean))
* sapply(split(mtcars$mpg, mtcars$cyl), mean)
* mean(mtcars$mpg, mtcars$cyl)
* tapply(mtcars$cyl, mtcars$mpg, mean)
* sapply(mtcars, cyl, mean)
* lapply(mtcars, mean)
* tapply(mtcars$mpg, mtcars$cyl, mean)
