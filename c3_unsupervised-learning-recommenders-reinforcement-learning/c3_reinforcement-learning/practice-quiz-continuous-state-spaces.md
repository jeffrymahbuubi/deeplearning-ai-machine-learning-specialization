## Continuous state spaces

### Question 1

The Lunar Lander is a continuous state Markov Decision Process (MDP) because:

- The reward contains numbers that are continuous valued
- **The state contains numbers such as position and velocity that are continuous valued.**
- The state-action value $Q(s, a)$ function outputs continuous valued numbers
- The state has multiple numbers rather than only a single number (such as position in the $x$-direction)

> The Lunar Lander can be described as a continuous state Markov Decision Process (MDP) because the state can include numbers such as position and velocity, which can take continuous values. Therefore, the correct option is:

### Question 2

In the learning algorithm described in the videos, we repeatedly create an artificial training set to which we apply supervised learning where the input $x=(s,a)$ and the target, constructed using Bellman's equations, is y=?

- $y=maxQ(s^{'},a^{'})$ where $s^{'}$ is the state you get to after taking action $a$ in state $s$
- **$y=R(s)+\gamma{max_{a^{'}}Q(s^{'},a^{'})}$ where $s^{'}$ is the state you get to after taking action $a$ in state $s$**
- $y=R(s^{'})$ where $s^{'}$ is the state you get to after taking action $a$ in state $s$
- $y=R(s)$

> In reinforcement learning algorithms such as Q-learning, the target for training the Q- function is often constructed using Bellman's equation. In this context, the target $y$ is based on the immediate reward for taking action $a$ in state $s$, plus the discounted maximum Q- value for the next state $s^{'}$.

### Question 3

You have reached the final quiz of this class! What does that mean? (Please check all the answers, because all of them are correct)
