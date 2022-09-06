This is a series of projects where I solve RL environments by building RL algorithms from scratch using Python, Pytorch and Tensorflow

<p align="center">
<img src = "https://github.com/SwamiKannan/Lunar-Landing-using-DQN-and-DDQN/blob/main/cover.png">
</p>

# Exercise
Solving the Lunar Landing environment using DQN and DDQN

# Lunar Landing v2
## Environment:
<ul>
<li>Rocket trajectory optimization is a classic topic in Optimal Control. According to Pontryagin's maximum principle it's optimal to fire engine full throttle or turn it off. That's the reason this environment is OK to have discreet actions (engine on or off).</li><br>
<li>The landing pad is always at coordinates (0,0). The coordinates are the first two numbers in the state vector. Reward for moving from the top of the screen to the landing pad and zero speed is about 100 to 140 points.</li><br>
<li>If the lander moves away from the landing pad it loses reward. The episode finishes if the lander crashes or comes to rest, receiving an additional -100 or +100 points. Each leg with ground contact is +10 points.</li><br>
<li>Firing the main engine is -0.3 points each frame. Firing the side engine is -0.03 points each frame.</li><br>
<li>Solved is 200 points.</li><br>
<li>Landing outside the landing pad is possible. Fuel is infinite, so an agent can learn to fly and then land on its first attempt. </li><br>
</ul>

## Source code for environment: <br>
openai/gym [Source code](https://github.com/openai/gym/blob/master/gym/envs/box2d/lunar_lander.py)
