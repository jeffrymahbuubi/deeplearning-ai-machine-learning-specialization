## Practice quiz: Multiclass Classification

### Quesiton 1

![5](./images/5.png)

For a multiclass classification task that has 4 possible outputs, the sum of all the activations adds up to 1. For a multiclass classification task that has 3 possible outputs, the sum of all the activations should add up to ...

- **1**
- More than 1
- Less than 1
- It will vary, depending on the input x.

> Yes! The sum of all the softmax activations should add up to 1. One way to see this is that if $e^{z_{1}}=10, e^{z_{2}}=20, e^{z_{3}}=30$, then the sum of $a_{1}+a_{2}+a_{3}$ is equal to $\frac{e^{z_{1}}+e^{z_{2}}+e^{z_{3}}}{e^{z_{1}}+e^{z_{2}}+e^{z_{3}}}$

### Question 2

![6](./images/6.png)

For multiclass classification, the cross entropy loss is used for training the model. If there are 4 possible classes for the output, and for a particular training example, the true class of the example is class 3 (y=3), then what does the cross entropy loss simplify to? [Hint: This loss should get smaller when $a_{3}$ gets larger.]

- $\frac{-log(a_{1})+-log(a_{2})+-log(a_{3})+-log{a_{4}}}{4}$
- z_3
- $-log(a_{3})$ - ANSWER
- z_3/(z_1+z_2+z_3+z_4)

> Correct. When the true labels is 3, then the cross entrop los for that training example is just the negative of the log of the activation for the tird neuron of the softmax. All other terms of the cross entropy loss equation $-(log(a_{1})), -log(a_{2})$, and $-log(a_{4})$ are ignored.

### Question 3

![7](./images/7.png)

For a multiclass classification, the recommended way to implement softmax regression is to set from_logits=True in the loss function, and also to define the model's output layer with...

- **a `linear` activation**
- a `softmax` activation

> Yes! Set the output as linear, because the loss function handles the calculation of the softmax with a more numerically stable method.
