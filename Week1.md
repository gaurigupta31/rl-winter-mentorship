<h3>Exercise 3.1:</h3>
<b>Devise three example tasks of your own that fit into the reinforcement learning framework, identifying for each its states, actions, and
rewards. Make the three examples as different from each other as possible. The framework is abstract and flexible and can be applied in many different ways. Stretch its limits in some way in at least one of your examples.</b>
<br>

1. <i>In the simple case of an agent playing the game of Piano Tiles:</i>
The actions will be clicking on the screen when the required tile appears. The reward, as per the game rules and from the previous state of whether or not the agent lost a game based on an action. 

2. <i>In the case of self-driving car navigating in traffic, in outline:</i>
The agent will take actions to move forward while using its sensors making sure the car is at a safe distance from the car in front and from cars in other lanes. The reward is derived from the distance covered in time 't' and no or minimum possible collisions.

3. <i>In the case of a self-charging house cleaning bot:</i>
The agent will take actions to clean when it is most convenient and least disruptive around the house. The agent while on its charging pad will sense movement around the house and clean the house periodically. 
Hence, its actions include a) clean when it is least disruptive to residents of the house and b) return to the charging pad before its battery runs out. This has to be done periodically so the house remains clean. 
The agent's state is determined by a) how long it has been since the last cleaning, b) input from its sensors that sense movement in the house and, c) its battery percentage. 
There will be a large positive when the agent returns to its pad with sufficient battery, small negative rewards if there was movement other than it's own while the agent was cleaning and large negative reward if its battery runs out before reaching its charging pad. The reward will be 0 when the agent is on the charging pad and taking input from the sensors to decide on the next time it can go for a periodic cleaning. 

<br>
<h3>Exercise 3.2: </h3> 
<b>Is the reinforcement learning framework adequate to usefully represent all goal-directed learning tasks? Can you think of any clear exceptions?</b>

<br>
<br>
In the case where the agent is not constantly provided with a reward for each action/state, the goad-directed learning task will not be fulfilled.  There are no clear exceptions as long as there is a scalar reward provided for every positive or negative action for achieving the goal.

<br>
<br>
<h3>Exercise 3.3:</h3>
<b>Consider the problem of driving. You could define the actions in terms of the accelerator, steering wheel, and brake, that is, where your body meets the machine. Or you could define them farther out—say, where the rubber meets the road, considering your actions to be tire torques. Or you could define them farther in—say, where your brain meets your body, the actions being muscle twitches to control your limbs. Or you could go to a really high level and say that your actions are your choices of where to drive. What is the right level, the right place to draw the line between agent and environment? On what basis is one location of the line to be preferred over another? Is there any fundamental reason for preferring one location over another, or is it a free choice?</b>

<br>
<br>
The line between the agent and the environment is drawn where its reward signal comes from. Every place where the reward signal comes from becomes a part of the environment since we cannot depend on the agent to compute its own rewards. 
