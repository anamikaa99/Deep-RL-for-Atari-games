# Deep-RL-for-Atari-games
 The aim is to explore the performance of deep learning algorithms in three different environments, with one being more complex than the other two.


Environments in consideration :
**• Cartpole • MountainCar • Boxing**

Algorithms in consideration :
**• DQN • Double DQN • A2C • PPO**

2 Environments
 
 2.1 **CartPole-v1 environment**
 
  Observation Space : 4-dimensional array -
  • Cart Position
  • Cart Velocity
  • Pole Angle
  • Pole Angular Velocity
  
  Action Space :
  [{0 : push cart to left}, {1 : push cart to right}] 
  
  Rewards :
  Since the goal is to keep the pole upright for as long as possible, a reward of `+1` for every step taken, including the termination step, is allotted. The threshold for rewards
  is 475 for v1.
  
  Termination :
  The episode ends if any one of the following occurs:
  1. Pole Angle > ±12°
  2. Cart Position > ±2.4 (center of the cart reaches the edge of the display)
  3. Length of episode is greater than 500


 2.2 **MountainCar environment**
  
  Observation Space :
   n-dimensional array with shape (2, ). Elements correspond to :
   • position of the car along the x-axis 
   • velocity of the car
  
  Action Space :
   [{0 : accelerate to left}, {1 : don’t accelerate}, {2 : accelerate to right}]
  
  Rewards :
   Agent is penalized with the reward of -1 at each time-step.
 
  Termination :
   • The position of the car is greater than or equal to 0.5 (the goal position on the top of the right hill) 
   • The length of the episode is 200


2.3 **Boxing environment**

 Observation Space : (210, 160, 3)
 
 Action Space : Discrete(18)
 
 Rewards : You score points by landing punches
 
 Termination : If the score is 100 points, the opponent is knocked out

