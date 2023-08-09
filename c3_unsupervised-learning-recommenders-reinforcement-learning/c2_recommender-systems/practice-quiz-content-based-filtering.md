## Content-based filtering

### Question 1

Vector $x_{u}$ and vector $x_{m}$ must be of the same dimension, where $x_{u}$ is the input features vector for a user (age, gender, etc) $x_{m}$ is the input features vector for a movie (year, genre, etc.) True or false?

- True
- **False**

> The vectors can be different dimensions.

### Question 2

If we find that two movies, $i$ and $k$, have vectors $v_{m}^{(i)}$ and $v_{m}^{(k)}$ that are similar to each other (i.e., $||v_{m}^{(i)}-v_{m}^{(k)}||$ is small), then which of the following is likely to be true? Pick the best answer.

- **The two movies are similar to each other and will be liked by similar users.**
- We should recommend to users one of these two movies, but not both.
- The two movies are very dissimilar.
- A user that has watced one of these two movies has probably watched the other as well.

> Similar movies generate similar $v_{m}'s$

### Question 3

Which of the following neural network configurations are valid for a content based filtering application Please note carefully the dimensions of the neural network indicated in the diagram. Check all the options that apply:

- ![2](./images/2.png) $\\$ **The user and the item networks have different architectures** <hr>

> User and item networks can be the same or different sizes.

- ![3](./images/3.png) $\\$ The user vector v_u is 32 dimensional and the item vector v_m is 64 dimensional <hr>
- ![4](./images/4.png) $\\$ The user and the item networks have 64 dimensional v_u and v_m vector respectively<hr>
- ![5](./images/5.png) $\\$ **Both the user and the item networks have the same architecture** <hr>

> User and item networks can be the same or different sizes.

### Question 4

You have built a recommendation system to retrieve musical pieces from a large database of music, and have an algorithm that uses separate retrieval and ranking steps. If you modify the algorithm to add more musical pieces to the retrieved list (i.e., the retrieval step returns more items), which of these are likely to happen? Check all that apply.

- The quality of recommendations made to users should stay the same or worsen.
- **The system's response time might increase (i.e., users have to wait longer to get recommendations)**

> A larger retrieval list may take longer to process which may _increase_ response time

- The system's response time might decrease (i.e., users get recommendations more quickly)
- **The quality of recommendations made to users should stay the same or improve.**

> A larger retrieval list gives the ranking system more options to choose from which should maintain or improve recommendations.

### Question 5

To speed up the response time of your recommendation system, you can pre-compute the vectors v*m for all the items you might recommend. This can be done even before a user logs in to your website and even before you know the $x*{u}$ or $v_{u}$ vector. True/False?

- **True**

> The output of the item/movie neural network, $v_{m}$ is noto dependent on the user network when making predictions. Precomputing the results speeds up the prediction process.

- False
