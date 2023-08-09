## Recommender systems implementation

### Question 1

Lecture described using `mean normalization` to do feature scaling of ratings. What equation below test describes this algorithm?

- $y_{norm}(i,j)=\frac{y(i,j)-\mu_{i}}{\sigma_{i}}$ where $\\$ $\mu_{i}=\frac{1}{\sum_{j}r(i,j)}\sum_{j : r(i,j) = 1}y(i,j)$ $\\$ $\sigma_{i}^{2}=\frac{1}{\sum_{j}r(i,j)}\sum_{j:r(i,j)=1}(y(i,j)-\mu_{j})^2$
- $y_{norm}(i,j)=\frac{y(i,j)-\mu_{i}}{\sigma_{i}}$ where $\\$ $\mu_{i}=\frac{1}{\sum_{j}r(i,j)}\sum_{j : r(i,j) = 1}y(i,j)$
- $y_{norm}(i,j)=\frac{y(i,j)-\mu_{i}}{max_{i}-min_{i}}$ where $\\$ $\mu_{i}=\frac{1}{\sum_{j}r(i,j)}\sum_{j : r(i,j) = 1}y(i,j)$

> This is mean normalization described in lecture. This will result in a zero average value on per-row basis.

### Question 2

The implementation of collborative filtering utilized a custom training loop in TensorFlow. Is it true that TensorFlow always requieres a custom training loop?

- Yes. TensoFlow gains flexibility by providing the user primitive operations they can combine in many ways.
- **No; TensorFlow provides simplified training operations for some applications.**

> Recall in Course 2, you were able to build a neural network using a 'model', 'compile', 'fit', sequence which managed the training for you. A custom training loop was utilized in this situation because training $w, b$, and $x$ does not fit the standard layer paradigm of TensorFlow's neural network flow. There are alternate solutions such as custom layers, however, it is useful in this course to introduce you to this powerful feature of TensorFlow.

### Question 3

Once a model is trained, the 'distance' between features vectors gives an indication of how similar items are. The squared distance between the two vectors $x^{(k)}$ and $x^{(i)}$ is : $\\$ $\text{distance}=||x^{(k)}$ and $x^{(i)}||^{2}=\sum_{l=1}^{n}(x_{1}^{(k)}-x_{l}^{(i)})^{2}$

Using the table below, find the closes item to the movie "Pies, Pies, Pies"

| Movie               | User 1 | ... | User n | $x_{0}$ | $x_{1}$ | $x_{2}$ |
| ------------------- | ------ | --- | ------ | ------- | ------- | ------- |
| Pastries for Supper |        |     |        | 2.0     | 2.0     | 1.0     |
| Pies, Pies, Pies    |        |     |        | 2.0     | 3.0     | 4.0     |
| Pies and You        |        |     |        | 5.0     | 3.0     | 4.0     |

- Pastries for Supper
- **Pies and You**

> The distance from 'Pies, Pies, Pies' is 9 + 0 + 0 = 9

### Question 4

Which of these is an exampe of the cold start problem? (Check all that apply)

- **A recommendation system is unable to give accurate rating predictions for a new user that has rated few products.**

> A recommendation system uses user feedback to fit the prediction model.

- A recommendation system takes a long to train that users get bored and leave.
- **A recommendation system is unable to give accurate rating predictions for a new product that no users have rated.**

> A recommendation system uses product feedback to fit the prediction model.

- A recommendation system is so computationally expensive that it causes your computer CPU to heat up, causing your computer to need be cooled down and restarted.
