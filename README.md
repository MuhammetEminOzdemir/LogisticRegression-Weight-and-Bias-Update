# Logistic Regression Weight and Bias Update


![Ekran Resmi 2024-05-28 14 24 08](https://github.com/MuhammetEminOzdemir/LogisticRegression-Weight-and-Bias-Update/assets/80462839/b202c5e3-b293-4528-824d-e77214def545)

Now lets look at computation graph of logistic regression


![Ekran Resmi 2024-05-28 14 24 44](https://github.com/MuhammetEminOzdemir/LogisticRegression-Weight-and-Bias-Update/assets/80462839/2a55b801-0f31-4e64-9410-12c3e1c994f0)

Parameters are weight and bias.

Weights: coefficients of each pixels

Bias: intercept

z = (w.t)x + b => z equals to (transpose of weights times input x) + bias

In an other saying => z = b + px1w1 + px2w2 + ... + px4096*w4096

y_head = sigmoid(z)

Sigmoid function makes z between zero and one so that is probability. You can see sigmoid function in computation graph.

Why we use sigmoid function?

It gives probabilistic result

It is derivative so we can use it in gradient descent algorithm (we will see as soon.)

Lets make example:

Lets say we find z = 4 and put z into sigmoid function. The result(y_head) is almost 0.9. It means that our classification result is 1 with 90% probability.
Now lets start with from beginning and examine each component of computation graph more detailed.


![Ekran Resmi 2024-05-28 14 39 49](https://github.com/MuhammetEminOzdemir/LogisticRegression-Weight-and-Bias-Update/assets/80462839/7abeb6cd-04dc-437e-bba7-6c7ab3bf263a)
