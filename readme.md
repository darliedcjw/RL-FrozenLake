# 1. Frozen Lake

### Introduction

<p>The main goal in "Frozen Lake" requires the agent to tranverse the frozen lake from the start to the goal without falling into any of the holes.</p>

<b><u>Start</u></b>
<br><br>
<img src="./asset/example-frozen-lake-start.png"></img>

<b><u>Goal</u></b>
<br><br>
<img src="./asset/example-frozen-lake-goal.png"></img>

# 2. Method

### Reinforcement learning

<p>There are 3 usual considerations in reinforcement learning: agent, state, a set of action per state. Given a state, an agent performs an action available in the state and is subsequently presented with a reward/penalty. The goal of reinfocement learning is to maximize the total reward.</p>

### Q-learning

<p>Q-learning is a reinforcement learning algorithm that is suitable for finite Markov Decision Process (MDP) and it does not require a model of the environment (a.k.a model-free).
<br>
<i>**Finite MDP refers a specific type of MDP where state space, action space and reward functions are all finite.</i>
<br><br>
<img src="./asset/q-learning-algorithm.png"></img>
<br><br>
<p>Let's explore Q-learning algorithm with an example. At step T, in state S<sub>T</sub>, an agent would be present with a set of actions (each with their respective Q value). When the agent performs an action A<sub>T</sub>, a reward R<sub>T+1</sub> is given, and the agent enters a new state S<sub>T+1</sub>. In Q-learning algorithm, it involves updating the Q value of the action A<sub>T</sub> in S<sub>T</sub> with the consideration of temporal difference between the current Q value and the estimated Q value.</p>
<p>Intuitively, it measure the before and after effect of taking an action. Coupled with a learning rate, it takes a portion of the learning (positive/negative) experience and update the current Q value.</p>

# 3. Result

<video src="./asset/video.mp4"></video>
