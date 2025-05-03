# Meta Heuristics
- Meta-heuristic algorithm - general method to approach a solution space by smartly searching through a set of possibilities (search space).
	- They are nature inspired algorithms, commonly used where the problem exhibits dynamic nature, and exact solutions may not be possible.
	- They find near optimal solution, so the exact (perfect) solution is not given.

- ## Multiverse Optimisation
	- Inspired from physics (Cosmology); The multiverse theory
	- Acc. to the multiverse theory more than one big bang equals more than one universe, i.e., Number of big bangs equals number of universes.
	- Multiple universes interact and collide with each other, each universe is a candidate for a solution for our problem 
		- Concepts 
			- White Hole
			- Black Hole
			- Worm Hole

	- ### White Hole
		- Exploration: Good solutions share their features with others.
		- Generated when parallel universes collide with each other
	- ### Black Hole: 
		- Exploitation: Poor solutions absorb information from better ones.
		- As normal black holes in physics they attract anything everything, in our case bad solutions
	- ### Wormholes
		- Randomness: Solutions make random moves toward the best-known one.
		- They link various sections of universes together information travels between universes through this path.
	
	- ## Rules
		- Probability of a white hole increases as inflation rate increases.
		- Probability of a black hole decreases as inflation rate increases.
			> Inflation rate is determined through a fitness function used for evaluation.
			
		- Universes with higher inflation rate tend to send objects through white hole
		- Universes with lower inflation rate tend to send objects through black hole
		- **Regardless** of inflation rate objects in all universes may experience random movement towards best universe via wormholes
	
	
	- ## Mathematical Modelling
	  
	>Roulette mechanism used to describe the model of white and black holes along with wormholes.

	- #### Model of Universe
		-  $$\begin{pmatrix} x_{1}^1 & \cdots & x_{1}^d\\ \vdots & \ddots & \vdots\\ x_{n}^1 & \cdots & x_{n}^d\end{pmatrix}$$
		- $$ d \space \implies \text{Number of Parameters}$$
		- $$ n \implies \text{Number of Universes}$$
	- Wormhole existence probability - WEP
		- $$ WEP = min + l*\left( \frac{max-min}{L} \right)$$
		- $$ l \implies \text{ current iteration}$$
		- $$ L \implies \text{ max iteration}$$
		- $$ min = 0.2 , max = 1.0 \text{ usually} $$
	- Travelling Distance Rate - TDR
		- $$ TDR = 1-\left( \frac{l^{1/p}}{L^{1/p}} \right) $$
		- $$ p \implies \text{ Called exploitation accuracy usually } 6$$
	- ## Algorithm
		- We provide the population size and max iterations.
		- It gives best universe its fitness value or inflation rate.
		- Step 1: Initialise Parameters.
		- Step 2: Compute fitness value for each universe select best universe.
		- Step 3: Update WEP and TDR for each universe.
		- Step 4: Select 1 universe among N by roulette wheel mechanism as white hole.
		- Step 5: Use wormholes as a tunnel for object exchange between different universes.
		- Step 6: Repeat until stopping criteria matched.
		  
--- 
## References
[Learn Multiverse Optimization Algorithm Example Step-by-Step Explanation ~xRay Pixy🌞🌍🌃🌿 - YouTube](https://www.youtube.com/watch?v=eQL0eJo2aAg)
[Multiverse Optimization Algorithm in Additive Manufacturing](https://www.youtube.com/watch?v=LMvqIIzdL6M&t=660s)