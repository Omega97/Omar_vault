
When I train a policy function on a game, the ELO score $s(t)$ (performance) increases linearly in the initial phase, to then reach a log-like plateau. It's as if there were two phases: 
- a *gas phase* - constant "improvement cost" at the beginning, concepts $\xi_k$ don't "interact" 
  cost(x) = 1 $\rightarrow$ score = $\int dx$ = x
- a *condensed phase* - linear cost for adding new concepts in the "conceptual structure" of the understanding of the game.
  cost(x) = x $\rightarrow$ score = $\int \frac{dx}{x} = \log(x)$

Take the *Hopfield Network* framework as a *general guideline* to describe a framework that describes this phase transition.
Key recommended simplifications:
- $f_\theta(x)$ decision field (policy function)
- $\hat p (x)$ optimal move (target policy)
- $\mathcal X = \{0,1\}^M$ domain (representative points) 
- $\mathcal Y = \{0,1\}$ codomain
- $H(f_\theta(x),\hat p(x))$ Hamiltonian as a function of the model output rather than explicitly the model parameters $\theta$

Quantities
- $M$ input dimension
- $P$ number of concepts
- $\mu$ concept index
- $C_{eff}$ effective capacity
- $\alpha=\frac{P}{C_{eff}}​$ load parameter
- $\alpha_c$ Critical Concept Density
- $q$ self-overlap (glassiness)
- $s(t)$ score
- $\epsilon$ Effective exploration noise

The **goal** is to explain the with a TD framework the *phase transition* in a *policy function*, given only input-output pairs from the model, without having the correct answers $\hat p$.

Keywords: #Hopfield_Network #Random_Features_Hopfield_Model

---
