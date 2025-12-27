Here are some clarifications about the rules for the game of Poker32:
- **Game Structure Clarification**: The game uses only one hole card per player (not two as in standard Texas Hold'em), and there's only one betting round.
- **Card Representation**: Cards are represented as 2-10, J, Q, K, A. 
- bets are only powers of 2.

- Write a Python program that implements the game in a Poker32 class. 
	- The class should have all the methods to initialize the players, make a move, return the game result
	- Add the `get_subjective_state(player_id)` method, that returns a representation of the state ass seen from that player (the branch of the state in the decision tree, and hole card)
	  
- Then, implement an Agent class, that can be used by humans and bots to interface with the game. 
    
- Subclass Agent to implement the PyTorchAgent, a probabilistic neural-network-based policy.
	  - This class should have a method for computing the probability that each player has each of the 13 cards in hand, by multiplying the prior probability ($P_0(A,A), P_0(A,K), \dots$) with the probability of each agent making the move to get to the next node in the decision tree 
	  $$P(A,K)=P_0(A,K) P(a_1|s_1) P(a_2|s_2) \dots$$
    - Note that the conditional probabilities come from the policy network itself during training, and the prior $P(A,A) = \frac{3}{4} P(A,K)$
    - The agent takes as input the subjective game state, but also the probability of the opponent having each card in hand (more specifically, list of logits). For example, if player A has a $K$ in hand, then the probability that the opponent has a $Q$ is $P(K,Q)/\sum_\text{card}{P(K,\text{card})}$
    - During training, this probability is calculated by using both player's policy.
    - During inference (i.e. against a human), this probability is calculated by using only that player's strategy, since the other strategy is unknown.
- Create a Training class. 
    - This class trains the policy of the agent through self-play.
    - Choose any reinforcement learning paradigm you find most appropriate.

