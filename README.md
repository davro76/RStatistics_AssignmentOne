# RStatistics_AssignmentOne
CAP 3330. Fall 2021

## Assignment 1 


### Instructions

- Create a notebook in R and write all the code and comments needed to answer the questions below.

- The submission for this assignment consists of uploading to Blackboard the results of running all the code in the notebook that you will create. You can submit either a PDF with all the results OR an HTML document with all the results.

- Make sure the document that you submit (the PDF or the HTML) includes:

a) The R code you used for each exercise part.

b)The R output you got after running each line of code.

c) The comments required to answer the question. For example, 9a) needs an explanation. Make sure you include that explanation too. 

## Questions

Tip: The code you write to answer each question must be generalizable, which means that it must work for any other dataset, not only for this dataset. For example, using as a reference question 5, the following code would not be generalizable since it only works for this dataset:

DFAsg1 [4:9, 2]

This line code is not generalizable because it takes into consideration the particular situation in this dataset, where rows from 1 to 3 belong to “A”, whereas the remaining rows belong to “B” or “C”.


1) Write code that allows you to create a vector x with the numbers {10,20,30,100,150,10,30,50}. Then, insert the number 168 between the third and fourth elements and assign the result of this insertion to x again.

2) Create a data frame with the following four columns: x (from the previous question), x1, x2, and y. Name the data frame DFAsg1

- x1 and x2 are the result of generating 9 random numbers from a normal distribution with a mean of 5 and standard deviation of 1. The numbers in x1 and x2 must be rounded to 1 decimal place. Use the following code to create x1 and x2:

x1<-rnorm(9,5,1)
x1<-round(x1,1)

x2<-rnorm(9,5,1)
x2<-round(x2,1)

- y is a character vector with three A’s, followed by three B’s, and then followed by three C’s (you need to create the vector y by yourself)

3) Use the data frame DFAsg1 as a reference. Write ONE LINE of code that returns the standard deviation of the values of x for each of the letters A, B, and C.

4) Use the data frame DFAsg1 as a reference. Write ONE LINE of code that returns the average of x1 and x2. 

5) Use the data frame DFAsg1 as a reference. Write ONE LINE of code that returns the values of x2 for records (rows) where the letter is B or C (i.e., return the values of x2 excluding rows where the letter is A)

6) Add a new column to the data frame DFAsg1 with a logical vector indicating whether the value of x1 is greater than the value of x2. Name this new column “Is_x1_greater”.

7) Display the duplicate elements in x (i.e., the values that repeat). The function duplicated () may be helpful.

Note: Notice that you must return the value or values that are duplicated.

8) Write ONE LINE of code that returns the count of how many elements in x are greater than 50.

9) Create a vector called “a” containing the numbers from 1 to 9. Create another vector called “b” containing the numbers from 1 to 4.

9a) Create a new vector called “sumAB” using the following expression: sumAB<- a + b. Explain how R obtains the last and second to last elements of the vector sumAB.

9b) Write ONE LINE of code that returns the total (i.e., the sum) of all the elements in vectors a and b combined.

