## Practice quiz: Neural Network Training

### Question 1

![1](./images/1.png)

Here is some code that you saw in the liecture:

```python
    model.compile(loss=BinaryCrossentropy())
```

For which type of task would you use the binary cross entropy loss function?

- **binary classification (classification with exactly 2 classes)**
- BinaryCrossentropy() should not be used for any task.
- A classification task that has 3 or more classes (categories)
- regression tasks (tasks that predict a number)

> Yes! Binary cross entropy, which we've also referred to as logistic loss, is used for classifying between two classes (two categories)

### Question 2

![2](./images/2.png)

Here is code that you saw in the lecture:

```python
model = Sequential ([
    Dense(units=25, activation='sigmoid')
    Dense(units=15, acitvation='sigmoid')
    Dense(units=1, activation='sigmoid')
])

model.compile(loss=BinaryCrossentropy())
model.fit(X,y,epochs=100)
```

Which line of code udpates the network parameters in order to reduce the cost?

- None of the above -- this code does not update the network parameters.
- model.compile(loss=BinaryCrossentropy())
- model = Sequential([...])
- **model.fit(X,y,epochs=100)**

> Yes! The third step of model training is to train the model on data in order to minimize the loss (and the cost)
