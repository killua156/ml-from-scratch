>this doc contains info on how Linear Regression works. With first principles and intuition prefered over math

So Linear Regression is where every data science course starts, and after doing my masters in Applied statistics and Data science, I have realized that is because Linear Regression is one of the most(if not most) simple models.

Explanation:
y = mx + c

We are trying to find the parameters(m and c) for this equation where 'y' will be the variable we are trying to predict and 'x' is the input variable.

Our goal is to adjust m and c continously until the overall error(the difference between actual and predicted values for each data point) is low/least.

## How the model works
The model learns by making mistakes over and over again. In each iteration it tries to reduce the overall error by adjusting the parameters m and c. They are not adjusted randomly but adjusted in a manner that overall error reduces.This process is called gradient disant. At its core, Linear Regression is just a trial and error method over many iterations to find the best parameters.

m = m - learning_rate*gradient_m
c = c - learning_rate*gradient_c

So the learning rate here is used to reduce or increase m/c depending on which will reduce error.
A huge learning rate will overshoot and might not work.
A small leanring rate will make it too slow and might not yeild any results.
