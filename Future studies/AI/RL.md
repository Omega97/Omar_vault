
In a turn-based, 2-player game with hidden info, I evaluated the gradient of the EV given the policies (players in fixed locations) as:

$$\mathbb E(r(t), \pi_\theta, \pi_2) 
= \sum_t r(t) \, p(t;\pi_\theta, \pi_2)$$

$$\log p(t;\pi_\theta, \pi_2) 
= \sum_{a,s \in B^{(1)}(t)}{\log \pi_\theta(a|s)} + \sum_{a,s \in B^{(2)}(t)}{\log \pi_2(a|s)}$$

$$\nabla_\theta \log p(t;\pi_\theta, \pi_2) 
= \sum_{a,s \in B^{(1)}(t)}{\nabla_\theta \; \log \pi_\theta(a|s)}$$

$$\nabla_\theta \; EV(r(t), \pi_\theta, \pi_2) 
= \sum_t r(t) \, \nabla_\theta \, p(t;\pi_\theta, \pi_2)$$ $$= \sum_t r(t) \, p(t;\pi_\theta, \pi_2) \nabla_\theta \log p(t;\pi_\theta, \pi_2) 
= \sum_t r(t) \, p(t;\pi_\theta, \pi_2) \sum_{a,s \in B^{(1)}(t)}{\nabla_\theta \; \log \pi_\theta(a|s)}$$
$$\boxed{\nabla_\theta \; \mathbb E(r(t), \pi_\theta, \pi_2) 
= \mathbb E(r(t) w(t), \pi_\theta, \pi_2)}$$
where
$$w(t) = \sum_{a,s \in B^{(1)}(t)}{\nabla_\theta \; \log \pi_\theta(a|s)}$$

$s$ information set (the player's perspective)
$t \in T$ terminal nodes
$r(t)$ reward for player 1 in terminal node $t$
$p(t;\pi_\theta, \pi_2)$ probability of reaching terminal node $t$
$B^{(P)}(t)$ game branch of moves played by player $P$
$B(t)$ game branch of moves played by all players

---

Mini Poker, $N$ cards in deck, highest card wins (1 betting round, no common cards).
Both players ante 1 point. Raising doubles the bet. Players may call/check, raise, or fold.

Game tree (4 decision points):
"" -> ("C", "R")
"C" -> ("C", "R")
"CR" -> ("C", "F")
"R" -> ("C", "F")

Game branches (5 branches)
"CC"
"CRC"
"CRF"
"RC"
"RF"

Infoset space: 4 decision points \* N hole cards.

