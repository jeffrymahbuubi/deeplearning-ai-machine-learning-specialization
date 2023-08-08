## Practice quiz: Neural network model

### Question 1

![2](./images/2.png)

For a neural network, what is the expression for calculating the activation of the third neuron in layer 2? Note, this is different from the question that you saw in the lecture video.

- **$a^{[2]}_{3} = g(\vec{w}^{[2]}_{3}\cdot\vec{a}^{[1]}+b^{[2]}_{3})$**
- $a^{[2]}_{3} = g(\vec{w}^{[2]}_{3}\cdot\vec{a}^{[2]}+b^{[2]}_{3})$
- $a^{[2]}_{3} = g(\vec{w}^{[2]}_{3}\cdot\vec{a}^{[2]}+b^{[3]}_{2})$
- $a^{[2]}_{3} = g(\vec{w}^{[2]}_{3}\cdot\vec{a}^{[1]}+b^{[3]}_{2})$

> Yes! The superscript [2] refers to layer 2. The subscript 3 refers to the neuron in that layer. The input to layer 2 is the activation from layer 1.

### Question 2

For the handwriting recognition task discussed in lecture, what is the output $a^{[3]}_{1}$?

- A number that is either exactly 0 or 1, comprising the network's prediction
- A vector of several numbers, each of which is either exactly 0 or 1
- A vector of several numbers that take values between 0 and 1
- **The estimated prbability that the input image is of a number 1, a number that ranges from 0 to 1.**

> Yes! The neural network outputs a single number between 0 and 1.
