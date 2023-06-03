# Question 1
R was developed by statisticians working at

1 / 1 point

The University of Auckland


Johns Hopkins University


StatSci


Insightful

Correct
The R language was developed by Ross Ihaka and Robert Gentleman who were statisticians at the University of Auckland in New Zealand.

2.
Question 2
The definition of free software consists of four freedoms (freedoms 0 through 3). Which of the following is NOT one of the freedoms that are part of the definition?  Select all that apply.

0 / 1 point

The freedom to restrict access to the source code for the software.

Correct
This is not part of the free software definition. Freedoms 1 and 3 require access to the source code.


The freedom to sell the software for any price.

Correct
This is not part of the free software definition. The free software definition does not mention anything about selling software (although it does not disallow it).


The freedom to run the program, for any purpose.


The freedom to prevent users from using the software for undesirable purposes.


The freedom to redistribute copies so you can help your neighbor.

This should not be selected
This is freedom 2.


The freedom to improve the program, and release your improvements to the public, so that the whole community benefits.


The freedom to study how the program works, and adapt it to your needs.

3.
Question 3
In R the following are all atomic data types EXCEPT: (Select all that apply)

0 / 1 point

integer


list


array


complex


logical


data frame


matrix


table

Correct
'table' is not an atomic data type in R.


numeric


character

You didn’t select all the correct answers
4.
Question 4
If I execute the expression x <- 4 in R, what is the class of the object `x' as determined by the `class()' function?

1 / 1 point

matrix


list


integer


complex


real


numeric


vector

Correct
5.
Question 5
What is the class of the object defined by the expression x <- c(4, "a", TRUE)?

0 / 1 point

logical


numeric


mixed


integer


character

Incorrect
The character class is the "lowest common denominator" here and so all elements will be coerced into that class.

6.
Question 6
If I have two vectors x <- c(1,3, 5) and y <- c(3, 2, 10), what is produced by the expression rbind(x, y)?

1 / 1 point

a 3 by 3 matrix


a 3 by 2 matrix


a vector of length 2


a matrix with two rows and three columns


a vector of length 3


a 2 by 2 matrix

Correct
The 'rbind' function treats vectors as if they were rows of a matrix. It then takes those vectors and binds them together row-wise to create a matrix.

7.
Question 7
A key property of vectors in R is that

0 / 1 point

a vector cannot have have attributes like dimensions


elements of a vector all must be of the same class


elements of a vector can only be character or numeric


the length of a vector must be less than 32,768


elements of a vector can be of different classes

Incorrect
8.
Question 8
Suppose I have a list defined as x <- list(2, "a", "b", TRUE). What does x[[1]] give me? Select all that apply.

1 / 1 point

a numeric vector containing the element 2.

Correct

a list containing the letter "a".


a character vector containing the element "2".


a numeric vector of length 1.

Correct

a list containing the number 2.

9.
Question 9
Suppose I have a vector x <- 1:4 and a vector y <- 2. What is produced by the expression x + y?

1 / 1 point

a numeric vector with elements 3, 2, 3, 6.


a numeric vector with elements 3, 4, 5, 6.


an integer vector with elements 3, 2, 3, 4.


an integer vector with elements 3, 2, 3, 6.


a numeric vector with elements 3, 2, 3, 4.


a numeric vector with elements 1, 2, 3, 6.

Correct
10.
Question 10
Suppose I have a vector x <- c(3, 5, 1, 10, 12, 6) and I want to set all elements of this vector that are less than 6 to be equal to zero. What R code achieves this? Select all that apply.

1 / 1 point

x[x %in% 1:5] <- 0

Correct
You can create a logical vector with the expression x %in% 1:5 and then use the [ operator to subset the original vector x.


x[x == 0] <- 6


x[x > 6] <- 0


x[x <= 5] <- 0

Correct
You can create a logical vector with the expression x <= 5 and then use the [ operator to subset the original vector x.


x[x > 0] <- 6


x[x == 0] < 6


x[x >= 6] <- 0


x[x < 6] == 0


x[x != 6] <- 0


x[x < 6] <- 0

Correct
You can create a logical vector with the expression x < 6 and then use the [ operator to subset the original vector x.


x[x == 6] <- 0

11.
Question 11
Use the 
Week 1 Quiz Data Set
 to answer questions 11-20.

In the dataset provided for this Quiz, what are the column names of the dataset? 

1 / 1 point

Ozone, Solar.R, Wind, Temp, Month, Day


1, 2, 3, 4, 5, 6


Month, Day, Temp, Wind


Ozone, Solar.R, Wind

Correct
You can get the column names of a data frame with the `names()' function.

12.
Question 12
Extract the first 2 rows of the data frame and print them to the console. What does the output look like?

1 / 1 point

123
  Ozone Solar.R Wind Temp Month Day
1     7      NA  6.9   74     5  11
2    35     274 10.3   82     7  17


123
  Ozone Solar.R Wind Temp Month Day
1    41     190  7.4   67     5   1
2    36     118  8.0   72     5   2


123
  Ozone Solar.R Wind Temp Month Day
1     9      24 10.9   71     9  14
2    18     131  8.0   76     9  29


123
  Ozone Solar.R Wind Temp Month Day
1    18     224 13.8   67     9  17
2    NA     258  9.7   81     7  22

Correct
You can extract the first two rows using the [ operator and an integer sequence to index the rows.

13.
Question 13
How many observations (i.e. rows) are in this data frame?

1 / 1 point

45


129


160


153

Correct
You can use the `nrows()' function to compute the number of rows in a data frame.

14.
Question 14
Extract the last 2 rows of the data frame and print them to the console. What does the output look like?

1 / 1 point

123
    Ozone Solar.R Wind Temp Month Day
152    11      44  9.7   62     5  20
153   108     223  8.0   85     7  25


123
    Ozone Solar.R Wind Temp Month Day
152    31     244 10.9   78     8  19
153    29     127  9.7   82     6   7


123
    Ozone Solar.R Wind Temp Month Day
152    34     307 12.0   66     5  17
153    13      27 10.3   76     9  18


123
    Ozone Solar.R Wind Temp Month Day
152    18     131  8.0   76     9  29
153    20     223 11.5   68     9  30

Correct
The `tail()' function is an easy way to extract the last few elements of an R object.

15.
Question 15
What is the value of Ozone in the 47th row?

1 / 1 point

18


34


63


21

Correct
The single bracket [ operator can be used to extract individual rows of a data frame.

16.
Question 16
How many missing values are in the Ozone column of this data frame?

1 / 1 point

9


78


43


37

Correct
The `is.na' function can be used to test for missing values.

17.
Question 17
What is the mean of the Ozone column in this dataset? Exclude missing values (coded as NA) from this calculation.

1 / 1 point

18.0


42.1


53.2


31.5

Correct
The `mean' function can be used to calculate the mean.

18.
Question 18
Extract the subset of rows of the data frame where Ozone values are above 31 and Temp values are above 90. What is the mean of Solar.R in this subset?

1 / 1 point

212.8


185.9


334.0


205.0

Correct
You need to construct a logical vector in R to match the question's requirements. Then use that logical vector to subset the data frame.

19.
Question 19
What is the mean of "Temp" when "Month" is equal to 6? 

1 / 1 point

79.1


75.3


85.6


90.2

Correct
20.
Question 20
What was the maximum ozone value in the month of May (i.e. Month is equal to 5)?

1 / 1 point

97


115


18


100
