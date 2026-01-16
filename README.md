# Markov Chain Monte Carlo

This repository contains implementations from scratch of core **Markov Chain Monte Carlo (MCMC)** methods for Bayesian inference and model selection.  
The focus is on understanding how different samplers work in practice, how they compare, and how they are used in realistic statistical problems.

## Contents

### 1. Gibbs Sampling
**File:** `Gibbs sampling.ipynb`  
Implements a Gibbs sampler for a bivariate Gaussian distribution, illustrating:
- Conditional distributions
- Iterative sampling
- Convergence behaviour and mixing in low dimensions

This notebook demonstrates how Gibbs sampling exploits conditional conjugacy to produce efficient draws from a joint distribution.

---

### 2. Posterior Sampling with Metropolis–Hastings
**File:** `Posterior sampling.ipynb`  
Implements posterior sampling using a Metropolis–Hastings style algorithm, including:
- Proposal distributions
- Acceptance–rejection logic
- Trace plots and empirical posterior summaries

This notebook highlights the generality of MH methods when conditional sampling is not available.

---

### 3. Model Selection via Perfect Monte Carlo
**File:** `Model Selection via Perfect Monte Carlo.ipynb`  
Uses perfect Monte Carlo techniques to estimate marginal likelihoods for Bayesian model comparison.  
Topics include:
- Exact (unbiased) sampling methods
- Stable computation of log-sum-exp expressions
- Using Monte Carlo estimates for Bayesian model selection

**Data file:** `y_perfect_mc.txt`  
Contains the observed data used in the perfect Monte Carlo experiments.

---

## Purpose of project

This project demonstrates:

- Core MCMC algorithms implemented from first principles  
- Understanding of:
  - Markov chains and stationary distributions  
  - Posterior simulation  
  - Monte Carlo estimation of evidence  
- Clean, readable code suitable for extension to more complex Bayesian models

---

## How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/markov-chain-monte-carlo.git
   cd markov-chain-monte-carlo
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS / Linux
   # or
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:
   ```bash
   pip install numpy scipy matplotlib jupyter
   ```
4. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
   

