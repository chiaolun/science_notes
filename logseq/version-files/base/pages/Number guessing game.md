# Problem Statement
	- Guess the number that I picked, an integer between 1 and 100. After each of your guesses, I’ll tell you if the number you guessed is higher or lower than the number I picked. Game would start with \$100 prize money and reduce \$20 for each wrong guess. So \$100 for first guess, \$80 for second, etc etc. - The Art of Strategy by Avinash Dixit and Barry Nalebuff
	- Two players
		- Picker
			- Policy is fully characterized by a one dimensional distribution of the hidden number. This would be 100 positive numbers that sum to one.
		- Guesser
			- Policy is characterized by a policy function that takes as input a lower and upper bound (summarizing information obtained from previous guesses) and outputting the distribution of next guesses.
- ### Guesser Policy given Picker
	- If you know the picker's policy, as represented by the distribution of picks from 1 to 100, the optimal strategy for the guesser can be obtained by constructing a value function. The value function gives the expected gain given what you know about the lower and upper bounds, and can be defined recursively by adding up the value of the three possible outcomes from a guess - the pick is either less than, equal to, or greater than your guess.
		- Value of guessing $k$ given $lower$ and $upper$ and with $n$ guesses is equal to (unnormalized)
			- Getting it right with $P_k$
			- Pick being lower with $(\Sigma_{i=lower}^{k-1} P_i )\times V(n - 1, lower, k-1)$
			- Pick being lower with $(\Sigma_{i=k+1}^{upper} P_i) \times V(n - 1, k + 1, upper)$
		- V consists of summing these terms with a max over k, i.e., picking the best guess for any given $(n, lower, upper)$
		- When $n = 0$, $V = 0$, so the recursion terminates
- Given that I have two players in a zero-sum game, and I know how to solve for player 2's optimal strategy given knowledge of player 1's strategy, if I then optimizer player 1 to minimize player 2's gain, does this guarantee that I will arrive at the Nash equilibrium?
	- ChatGPT: In a zero-sum game, the goal is typically to find the Nash equilibrium where no player can benefit by unilaterally changing their strategy. If you know player 1's strategy and can solve for player 2's optimal response, that gives you the optimal strategy for player 2 given player 1's strategy. 
	  
	  To find the Nash equilibrium, you need both players to be optimizing their strategies. By optimizing player 1 to minimize player 2's gain (which is equivalent to maximizing player 1's payoff in a zero-sum context), you are essentially looking for player 1's best response to player 2's strategy. If you follow this process iteratively for both players, or if both players are simultaneously playing their optimal strategies, you should arrive at the Nash equilibrium.
	  
	  In zero-sum games, the Nash equilibrium corresponds to a situation where player 1 is minimizing player 2's maximum possible gain, and player 2 is maximizing their payoff given player 1's strategy. Therefore, optimizing player 1 to minimize player 2's gain, while simultaneously having player 2 best respond to player 1's strategy, will lead to the Nash equilibrium.
	- In this case, the optimal strategy for the guesser given the picker strategy is deterministic, but no deterministic strategy can be nash stable