## Practice quiz: Machine learning development process

### Question 1

![5](./images/5.png)

Which of these is a way to do error analysis?

- Collecting additional training data in order to thelp the algorithm do better
- **Manually examine a sample of the training examples that the model miscalssified in order to identify traits and trends**
- Calculating the training error $J_{train}$
- Calculating the test error $J_{test}$

> Correct. By identifying similar types of erros, you can collect more data that are similar to these misclassified examples in order to train the model to improve on these types of examples.

### Question 2

![6](./images/6.png)

We sometimes take an existing training example and modify it (for example, by rotating an image slightly) to create a new example with the same label. What is this process called?

- Error analysis
- Machine learning diagnostic
- **Data augmentation**
- Bias/variance analysis

> Yes! Modifying existing data (such as images, or audio) is called data augmentation.

### Question 3

![7](./images/7.png)

What are two possible ways to perform transfer learning? Hint: two of the four choices are correct.

- **You can choose to train all parameters of the model, including the output layers, as well as the earlier layers.**

> Correct. It may help to train all the layers of the model on your own training set. This may take more time compared to if you just trained the parameters of the output layers.

- Download a pre-trained model and use it for prediction without modifying or re-training it.
- **You can choose to train just the output layer's parameters and leave the other parameters of the model fixed.**

> Correct. The earlier layers of the model may be reusable as is, because they are identifying low level features that are relevant to your task.

- Given a dataset, pre-train and then further fine tune a neural network on the same dataset.
