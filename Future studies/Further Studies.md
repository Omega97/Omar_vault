
# 1) Information Geometry (IG) & Natural Gradient

**Idea.** Treat a statistical model family {pθ}\{p_\theta\} as a Riemannian manifold with Fisher metric; optimization becomes geometry.

**Key equation.** 
$$gij(θ)=E[∂ilog⁡pθ ∂jlog⁡pθ]g_{ij}(\theta)=\mathbb{E}[\partial_i \log p_\theta\,\partial_j \log p_\theta]. $$
Natural-gradient step: 
$$Δθ=−η g(θ)−1∇θL\Delta \theta = -\eta\, g(\theta)^{-1}\nabla_\theta L.$$

**Why it’s cool.** Replaces “units of parameters” with an intrinsic notion of distance in distribution space. Dual connections yield mirror descent and exponential vs. mixture coordinates.

**Applications.** Faster, scale-invariant training; policy-gradient RL (natural policy gradient); variational inference; exponential families.

**Try this.** Implement natural gradient for a small variational autoencoder and compare steps-to-convergence vs. Adam; plot geodesic-ish trajectories of θ\theta.

---

# 2) Optimal Transport (OT), Wasserstein Geometry & Schrödinger Bridges

**Idea.** Distances between probability measures with a geometry that respects mass and space.

**Key equations.**  
Static: W22(μ,ν)=min⁡π∈Π(μ,ν)∫∥x−y∥2 dπW_2^2(\mu,\nu)=\min_{\pi\in\Pi(\mu,\nu)}\int \|x-y\|^2\,d\pi.  
Dynamic (Benamou–Brenier): min⁡ρ,v∫01 ⁣ ⁣∫12∥vt(x)∥2ρt(x) dx dt\min_{\rho,v}\int_0^1\!\!\int \tfrac12\|v_t(x)\|^2\rho_t(x)\,dx\,dt s.t. ∂tρ+∇ ⁣⋅(ρv)=0\partial_t\rho+\nabla\!\cdot(\rho v)=0.  
Entropic OT ↔ Schrödinger bridge: add KL regularization to the coupling/dynamics.

**Why it’s cool.** Interpolates distributions along meaningful “mass-preserving” geodesics; the entropic variant links to diffusion and control-as-inference.

**Applications.** Generative models, dataset alignment/domain adaptation, diffusion model theory, barycenters of datasets.

**Try this.** Compute Wasserstein barycenters of MNIST digits from two classes; compare to linear (Euclidean) barycenters—night and day.

---

# 3) Geometric Mechanics: Symplectic & Contact Views

**Idea.** Hamiltonian systems as flows preserving symplectic form ω\omega; thermodynamics & friction emerge in contact geometry.

**Key equations.** iXHω=dHi_{X_H}\omega = dH (Hamiltonian vector field); Poisson bracket {f,g}=ω(Xf,Xg)\{f,g\}=\omega(X_f,X_g). Contact: iXHdα=dH−(RαH) αi_{X_H}d\alpha = dH - (R_\alpha H)\,\alpha.

**Why it’s cool.** Noether’s theorem drops out cleanly; discrete symplectic integrators conserve invariants; contact systems provide clean “dissipation geometry”.

**Applications.** Hamiltonian neural nets, symplectic integrators for long-horizon simulation, energy-based modeling, reversible computing.

**Try this.** Train a Hamiltonian NN on a 2-body system and compare long-term energy drift to a vanilla ODE-NN.

---

# 4) Gauge Theory & Fiber Bundles (beyond EM)

**Idea.** Fields as connections on bundles; curvature F=dA+A∧AF=dA+A\wedge A. EM is U(1)U(1); non-abelian Yang–Mills generalizes interactions.

**Key equations.** Fμν=∂μAν−∂νAμ+[Aμ,Aν]F_{\mu\nu} = \partial_\mu A_\nu - \partial_\nu A_\mu + [A_\mu,A_\nu]; covariant derivative Dμ=∂μ+AμD_\mu = \partial_\mu + A_\mu.

**Why it’s cool.** “Forces” become geometry; parallel transport and holonomy unify local symmetries.

**Applications.** Gauge-equivariant neural nets, parallel transport on manifolds/graphs, learning on fiber bundles (features with frames).

**Try this.** Build a rotation- and reflection-equivariant CNN on CIFAR-10 and compare sample efficiency vs. vanilla CNN.

---

# 5) Category Theory for ML & Probability (Markov Categories, Optics)

**Idea.** Reason about systems compositionally with string diagrams; probability, learning, and control become algebra of morphisms.

**Key notions.** Monoidal categories for parallel/series composition; _Markov categories_ for stochastic maps; _lenses/optics_ for bidirectional update.

**Why it’s cool.** You get correctness-by-construction and reusable blocks; proofs become pictures; “learning = Bayesian inversion” becomes a typed pipeline.

**Applications.** Differentiable programming semantics, compositional causal models, safe systems integration.

**Try this.** Sketch your RL pipeline as string diagrams: environment, policy, posterior updates. You’ll see where assumptions hide.

---

# 6) Sheaves & Cosheaves for Consistency on Graphs

**Idea.** Assign local data to nodes/edges and enforce consistency via restriction maps; (co)homology detects global obstructions.

**Key equation.** Sheaf cohomology groups HkH^k quantify “inconsistency cycles”.

**Why it’s cool.** A principled way to fuse local, overlapping measurements (sensors, charts, submodels) into a globally consistent whole.

**Applications.** Multi-sensor fusion, graph ML with constraints, program analysis, NLP document graphs (section-to-document coherence).

**Try this.** Take a knowledge graph with noisy labels; impose sheaf constraints and watch inconsistency localize to culprit subgraphs.

---

# 7) Renormalization Group (RG) & Thermodynamic Formalism

**Idea.** Coarse-grain, track how parameters flow with scale Λ\Lambda; in dynamical systems, “pressure” and large deviations quantify complexity.

**Key equations.** RG flow: ∂ℓθ=β(θ)\partial_\ell \theta = \beta(\theta).  
Thermodynamic formalism: pressure P(ϕ)=sup⁡μ{hμ+∫ϕ dμ}P(\phi)=\sup_\mu\{h_\mu + \int \phi\,d\mu\}.

**Why it’s cool.** Deep nets often act like multiscale coarse-grainers; implicit biases resemble fixed points/attractors under training dynamics.

**Applications.** Understanding generalization via scales, curriculum as scale scheduling, pruning/distillation as RG flows.

**Try this.** Track layerwise spectrum under training and watch “relevant/irrelevant” directions emerge à la RG.

---

# 8) Mirror Descent & Bregman Geometry (dual to IG)

**Idea.** Optimize in a dual space via a convex potential ϕ\phi; Euclidean GD is just ϕ(x)=12∥x∥2\phi(x)=\tfrac12\|x\|^2.

**Key equation.** xt+1=∇ϕ∗(∇ϕ(xt)−η∇f(xt))x_{t+1}=\nabla\phi^*(\nabla\phi(x_t)-\eta\nabla f(x_t)). Bregman divergence Dϕ(x ⁣∥ ⁣y)=ϕ(x)−ϕ(y)−⟨∇ϕ(y),x−y⟩D_\phi(x\!\parallel\!y)=\phi(x)-\phi(y)-\langle\nabla\phi(y),x-y\rangle.

**Why it’s cool.** Picks the right geometry for the variable (simplex → KL; PSD cone → log-det). Explains softmax updates and “entropy-friendly” learning.

**Applications.** Policy optimization on simplices, multiplicative weights, sparse coding.

**Try this.** Swap your policy optimizer to mirror descent with KL geometry; measure stability vs. entropy-regularized PG.

---

# 9) Mean-Field Games & Control-as-Inference

**Idea.** Populations optimize jointly; equivalently, planning can be written as probabilistic inference with KL costs.

**Key equations.** HJB–Fokker–Planck system (backward–forward PDEs).  
Control-as-inference: minimize KL(q(trajectories) ∥ p(prior dynamics)⋅e−cost)\mathrm{KL}(q(\text{trajectories}) \,\|\, p(\text{prior dynamics}) \cdot e^{-\text{cost}}).

**Why it’s cool.** Unifies RL, diffusion, and OT; bridges Nash equilibria and entropy-regularized control.

**Applications.** Multi-agent RL, traffic/econ models, trajectory planning with constraints.

**Try this.** Solve a 1D Schrödinger bridge and compare its stochastic paths to deterministic OT geodesics.

---

# 10) Topological Data Analysis (TDA)

**Idea.** Extract shape from data via persistent homology; track birth/death of holes across scales.

**Key object.** Persistence diagram/barcode for a filtration.

**Why it’s cool.** Invariant to deformations and noise-robust; highlights global structure that statistics can miss.

**Applications.** Phase transitions (order parameters), anomaly detection, generative model evaluation (mode structure), protein geometry.

**Try this.** Compute persistence diagrams for embeddings of different text corpora; see topology shift across domains.

---

## How these plug into your interests

- **Semantic Dynamics:** OT for “semantic geodesics” between corpora; IG for temperature/natural metrics on distributions; thermodynamic formalism for pressure/entropy of trajectories; sheaves to enforce cross-section coherence (paragraph → document → corpus).
    
- **RL/game projects:** Mirror descent for simplex-valued strategies; mean-field games for population play; Hamiltonian/Contact nets to respect conserved (or dissipative) quantities in simulators.
    

If you want just one to dive into next, I’d pick **Optimal Transport + Schrödinger Bridges**: it’s geometrically clean, computationally practical (Sinkhorn), and sits at the intersection of diffusion models, control, and your thermodynamic lens.

Happy to go deep on any one—derivations, code, or a mini-research plan. Which one sparks?