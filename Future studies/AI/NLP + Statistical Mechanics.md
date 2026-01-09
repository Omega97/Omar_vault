

Below is a sampler of recent (and a few classic) papers that make an **explicit bridge between large-scale language modelling and ideas from statistical mechanics or thermodynamics**. I’ve grouped them by the flavour of the connection so you can decide where to dive first.

---

## 1 Thermodynamic state-functions for LLMs

|Paper|Key idea|Why it matters|
|---|---|---|
|**Yang, 2024 – _Entropy, Thermodynamics and the Geometrization of the Language Model_** ([arxiv.org](https://arxiv.org/html/2407.21092v1 "1 Introduction"))|Defines partition-, free- and internal-energy for any causal LM; introduces a “Boltzmann manifold” where LLMs live.|Gives a first-principles map from cross-entropy ↔ Helmholtz free energy and argues that emergent LLM abilities appear near zeros of an entropy function.|
|**Liu et al., 2025 – _Neural Thermodynamic Laws for Large Language Model Training_** ([arxiv.org](https://arxiv.org/html/2505.10559v1?utm_source=chatgpt.com "Neural Thermodynamic Laws for Large Language Model Training"))|Treats SGD as a heat bath and derives analogues of Fourier conduction & the Second Law for parameter flow.|Offers scaling-law predictions for learning curves and a thermodynamic view of optimiser hyper-parameters.|
|**Carson & Reisizadeh, 2025 – _A Statistical Physics of Language Model Reasoning_** ([arxiv.org](https://arxiv.org/abs/2506.04374 "[2506.04374] A Statistical Physics of Language Model Reasoning"))|Fits chain-of-thought hidden-state trajectories with a drift–diffusion (Langevin) model and detects phase transitions between reasoning “regimes”.|Gives empirical evidence that LM reasoning hops between metastable basins, mirroring critical phenomena.|

---

## 2 Energy-based language modelling

|Paper|Angle|Highlights|
|---|---|---|
|**Gladstone et al., 2025 – _Energy-Based Transformers (EBT)_** ([arxiv.org](https://arxiv.org/html/2507.02092v1 "Energy-Based Transformers are Scalable Learners and Thinkers"))|Re-casts autoregressive Transformers as EBMs whose Boltzmann density is minimised at inference by gradient descent.|Achieves “System-2” reasoning by energy minimisation and reports better OOD generalisation.|
|**Carbone, 2024 – _Hitchhiker’s Guide on the Relation of Energy-Based Models with Generative Models & Statistical Physics_ (review)** ([arxiv.org](https://arxiv.org/html/2406.13661v2 "Hitchhiker’s guide on the relation of Energy-Based Models with other generative models, sampling and statistical physics: a comprehensive review"))|Pedagogical tour of EBMs, sampling, and Boltzmann–Gibbs ensembles; positions LMs as special EBMs.|Great entry point if you want the full stat-mech dictionary (partition functions, Langevin sampling, etc.).|
|**Arora et al., 2016 – _RAND-WALK: A Latent-Variable Model Approach to Word Embeddings_** ([arxiv.org](https://arxiv.org/pdf/1502.03520?utm_source=chatgpt.com "[PDF] RAND-WALK: A latent variable model approach to word embeddings"))|Treats a “discourse vector” as a Brownian particle drifting through embedding space.|Classic paper that first made the Brownian/Ising analogy precise for word embeddings.|

---

## 3 Training dynamics & critical phenomena

|Paper|What it shows|
|---|---|
|**Ambrogioni, 2023/24 – _Statistical Thermodynamics of Generative Diffusion Models_ (phase transitions)** ([arxiv.org](https://arxiv.org/abs/2310.17467 "[2310.17467] The statistical thermodynamics of generative diffusion models: Phase transitions, symmetry breaking and critical instability"))|Reformulates diffusion models in equilibrium terms and proves they undergo mean-field second-order phase transitions.|
|**Sohl-Dickstein et al., 2015 – _Deep Unsupervised Learning Using Nonequilibrium Thermodynamics_** ([arxiv.org](https://arxiv.org/abs/1503.03585 "[1503.03585] Deep Unsupervised Learning using Nonequilibrium Thermodynamics"))|Original diffusion-model paper; forward noise + reverse denoise mapped to non-equilibrium thermodynamic cycles.|
|**Liu et al., 2025 – _Neural Thermodynamic Laws…_** (see §1)|Predicts Mpemba-like effects (hot-start training converging faster) and matches them to coarse-grained free-energy landscapes.|

---

## 4 Free-energy principle & active inference with LLMs

|Paper|Contribution|
|---|---|
|**Prakki, 2024 – _Active Inference for Self-Organising Multi-LLM Systems_** ([arxiv.org](https://arxiv.org/html/2412.10425v1 "Active Inference for Self-Organizing Multi-LLM Systems: A Bayesian Thermodynamic Approach to Adaptation"))|Wraps multiple LLMs in a variational free-energy loop that adaptively rewrites prompts; casts prompting as Bayesian thermodynamics.|

---

## 5 Useful survey / perspective pieces

- **“Deep generative models, sampling and statistical physics”** (Carbone 2024, review) – unifies EBMs, VAEs, GANs, flows and diffusion under stat-mech tools. ([arxiv.org](https://arxiv.org/html/2406.13661v2 "Hitchhiker’s guide on the relation of Energy-Based Models with other generative models, sampling and statistical physics: a comprehensive review"))
    
- **“Neural Thermodynamic Laws…”** (Liu 2025) doubles as a tutorial on how to coarse-grain SGD into Langevin dynamics. ([arxiv.org](https://arxiv.org/html/2505.10559v1?utm_source=chatgpt.com "Neural Thermodynamic Laws for Large Language Model Training"))
    

---

### How to use this reading list

1. **Pick your lens.**  
    _If you care about the loss function ↔ free energy analogy_, start with Yang 2024 → Liu 2025.  
    _If you’re building new model classes_, the EBM papers (Gladstone et al. 2025, Carbone 2024) are most actionable.  
    _For dynamics & phase transitions_, Ambrogioni 2024 and Carson 2025 give concrete empirical/analytical results.
    
2. **Cross-pollinate methods.**  
    Many of these works import tools like _specific heat, susceptibility, Langevin samplers_, or _Jarzynski equalities_. Those same diagnostics can be applied to embedding trajectories, cross-platform post “gases”, or fine-tuning logs.
    
3. **Watch the empirical side.**  
    Nearly all 2025 papers validate their physics analogies on large-scale runs (billions of tokens, multiple checkpoints). Re-using their open-source notebooks is a quick way to test the theory on your own corpora.
    

Enjoy the dive—statistical mechanics can be a surprisingly precise language for talking about LLMs, once you match the right variables!