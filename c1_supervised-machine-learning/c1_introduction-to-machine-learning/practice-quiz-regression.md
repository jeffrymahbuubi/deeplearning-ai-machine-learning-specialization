## Practice quiz: Regression

<br>

### Question 1

For linear regression, the model is $f_{w,b}(x) = wx + b$.

Which of the following are inputs, or features, that are fed into the model and with which the model is expected to make a prediction?

- $(x,y)$
- $w$ and $b$
- **$x$**
- $m$

> The $x$, the input features, are fed into the model to generate prediction $f_{w,b}(x)$

### Question 2

For linear regression, if you find parameters $w$ and $b$ so that $J(w,b)$ is very close to zero, what can you conclude?

- This is never possible --there must be a bug in the code.
- The selected values of the parameters $w$ and $b$ cause the algorithm to fith the training set really poorly.
- **The selected values of the parameters $w$ and $b$ cause the algorithm to fit the training set very well.**

> When the cost is small, this means that the model fits the training set well.
