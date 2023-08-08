## Practice quiz: Additional Neural Network Concepts

### Question 1

![8](./images/8.png)

The Adam optimizer is the recommended optimizer for finding the optimal parameters of the model. How do you use the Adam optimizer in TensorFlow?

- **When calling model.compile, set optimizer=tf.keras.optimizers.Adam(learning_rate=1e-3)**
- The call to model.compile() uses the Adam optimizer by default.
- The Adam optimizer works only with Softmax outputs. So if a neural network has a Softmax output layer, ThensorFlow ill automatically pick the Adam optimizer.
- The call to model.copile() will automatically pick the best optimizer, whther it is gradient descent, Adam or something else. So there's no need to pick an optimizer manually.

> Correct. Set the optimizer to Adam.

### Question 2

![9](./images/9.png)

The lecture covered a different layer type where each single neuron of the layer does not look at all the values of the input vector that is fed into that layers. What is this name of the layer type discussed in lecture?

- **convolutional layer**
- Image layer
- A fully connected layer
- 1D layer or 2D layer (depending on the input dimension)

> Correct. For a convolutional layer, each neuron takes as input a subset of the vector that is fed into that layer.
