# 🧮 AI Engineering Math Roadmap

A phase-wise, checkbox-driven math curriculum mapped to an AI Engineering learning path — from arithmetic basics to LLM/transformer math.

> Tip: Track progress by checking boxes as you complete each topic. For every topic, follow the micro-plan at the bottom: **Concept → Formulas → 1 Derivation → 2–5 Practice Problems → 1 Mini Project**.

---

## 📌 Phase 0 — Preliminaries (Before AI Math)

### 1. Arithmetic & Number System
- [ ] **NUMBERS**
- [ ] Natural Numbers
- [ ] Whole Numbers
- [ ] Integers
- [ ] Rational Numbers
- [ ] Irrational Numbers
- [ ] Real Numbers

- [ ] **FRACTION**
- [ ] Proper fractions
- [ ] Improper fractions
- [ ] Mixed fractions
- [ ] Fraction operations (add, subtract, multiply, divide)
- [ ] Decimal ↔ fraction conversion
- [ ] Operations with decimals
      
- [ ] Percentage calculation, % increase, % decrease
- [ ] Ratios & proportions
- [ ] Direct variation
- [ ] Inverse variation
- [ ] Scientific notation (standard form ↔ scientific form, e.g. `2,500,000 = 2.5 × 10^6`)

### 2. Exponents & Powers
- [ ] Laws of exponents: `a^m × a^n`, `a^m / a^n`, `(a^m)^n`, `(ab)^n`
- [ ] Zero exponent
- [ ] Negative exponent
- [ ] Fractional exponent (e.g. `16^(1/2)`, `27^(1/3)`)
- [ ] Square root, cube root, nth root

### 3. Logarithms
- [ ] Definition: `log_a(b) = x ⟺ a^x = b`
- [ ] Log rules: `log(ab)`, `log(a/b)`, `log(a^n)`
- [ ] Common log (`log10`)
- [ ] Natural log (`ln`) — very important for AI

### 4. Algebra
- [ ] Simplifying expressions, expanding brackets (e.g. `(a+b)^2`)
- [ ] Factorization (e.g. `x² + 5x + 6`, `a² - b²`)
- [ ] Linear equations (e.g. `2x + 3 = 11`)
- [ ] Simultaneous equations (e.g. `2x + y = 5`, `x - y = 1`)
- [ ] Quadratic equations — factorization method & quadratic formula
- [ ] Inequalities (e.g. `x > 5`, `x ≤ 10`)
- [ ] Algebraic manipulation / rearranging formulas (e.g. solve `y = mx + b` for `m`)

### 5. Sets
- [ ] Set notation & elements
- [ ] Union, intersection, difference, complement
- [ ] Cartesian product (`A × B`)

### 6. Relations
- [ ] Ordered pairs, relation, domain, range, codomain
- [ ] Reflexive, symmetric, transitive (basic understanding)

### 7. Functions ⭐ (very important)
- [ ] Function concept `f(x)` and evaluation (`f(2)`, `f(5)`)
- [ ] Constant, linear, quadratic, polynomial, rational, exponential, logarithmic functions
- [ ] Function composition `f(g(x))` (foundation for chain rule)
- [ ] Inverse functions (basic understanding)

### 8. Graphs of Functions
- [ ] Linear `y = mx + b`
- [ ] Quadratic `y = x²`
- [ ] Cubic `y = x³`
- [ ] Exponential `y = e^x`
- [ ] Logarithmic `y = ln(x)`

### 9. Matrix Basics (light introduction)
- [ ] Matrix definition: rows, columns
- [ ] Matrix types: row, column, square, identity, zero
- [ ] Addition, subtraction, scalar multiplication
- [ ] Matrix multiplication (basic understanding)
- [ ] Determinant (2×2 only)
- [ ] Inverse (2×2 only)

> ⭐ **Highest priority in Phase 0:** Algebra, Functions, Exponents, Logarithms, Matrix Basics. If short on time, put 60% of effort into **Algebra + Functions** — nearly everything in Calculus, Linear Algebra, and AI math builds on these.

---

## 🌱 Phase 1 — Solid Foundations (Months 1–2)

### Linear Algebra (beginner)
- [ ] Vectors: definition, addition, scalar multiplication
- [ ] Dot product, norm (length), angle between vectors
- [ ] Matrices: addition, multiplication, transpose
- [ ] Identity matrix, zero matrix
- [ ] Solving simple linear systems (`Ax = b`)
- [ ] Determinant & inverse (2×2, 3×3)
- [ ] Eigenvalues & eigenvectors — basic intro (simple 2×2 examples)

### Probability & Statistics (basics)
- [ ] Sample space, events, conditional probability
- [ ] Bayes' rule (basics)
- [ ] Random variables: discrete vs continuous
- [ ] PMF / PDF
- [ ] Distributions (basic): Bernoulli, Binomial, Normal (Gaussian)
- [ ] Mean, variance, standard deviation
- [ ] Descriptive statistics: median, mode, quartiles, skewness, histogram intuition

### Calculus (light intro)
- [ ] Derivatives basics
- [ ] Chain rule
- [ ] Partial derivatives (very basic)
- [ ] Gradient concept
- [ ] Limits (short refresher)

*You don't need Hessians, full multivariable calculus, or optimization theory yet — that's Phase 2.*

---

## 🤖 Phase 2 — Machine Learning Core (Months 2–4)

### Linear Algebra (deeper)
- [ ] Rank, column space, null space, linear independence
- [ ] Matrix factorizations — intro: LU decomposition (basic idea), QR decomposition (orthonormal bases)
- [ ] SVD (`U Σ Vᵀ`) — concept, low-rank approximation ⭐ very important
- [ ] Eigenvalues/eigenvectors — full: characteristic polynomial, diagonalization, spectral theorem
- [ ] PCA intuition (via eigen-decomposition and via SVD)
- [ ] Linear transformations, change of basis
- [ ] Norms: operator norm, Frobenius norm; condition number & stability

### Probability & Statistics (deeper)
- [ ] Maximum Likelihood Estimation (MLE)
- [ ] Full distribution list: Poisson, Exponential, Uniform, Gaussian (in detail)
- [ ] Covariance & correlation
- [ ] Joint, marginal, conditional distributions
- [ ] Multivariate Gaussian: density, mean vector, covariance matrix, contours ⭐ important
- [ ] Central Limit Theorem (concept) & Law of Large Numbers
- [ ] Bayesian thinking: prior, likelihood, posterior, MAP vs MLE
- [ ] Estimation theory: point estimators, bias vs variance, consistency
- [ ] Hypothesis testing: null/alternative, Type I/II errors, p-values
- [ ] z-test, t-test, confidence intervals

### Calculus (multivariable + optimization)
- [ ] Multivariable functions `f(x₁, …, xₙ)`
- [ ] Gradient `∇f`, directional derivative, Jacobian
- [ ] Hessian matrix & its role in curvature
- [ ] Convexity: convex sets/functions, why it matters
- [ ] Stationary points, second-derivative test
- [ ] Gradient descent (full): update rule, learning rate, momentum, convergence intuition
- [ ] Newton's method (idea using the Hessian)
- [ ] Loss function derivatives: MSE, cross-entropy, logistic regression gradient
- [ ] Regularization gradients (L1/L2 intuition)

### Applied ML Math
- [ ] Linear regression: normal equations, gradient descent, Ridge/Lasso
- [ ] Logistic regression: likelihood + gradient derivation
- [ ] PCA: SVD vs covariance eigen-decomposition
- [ ] Kernel trick — intuition only (no heavy proofs yet)

---

## 🧠 Phase 3 — Deep Learning & NLP (Months 4–6)

### Calculus (advanced for DL)
- [ ] Jacobian (deeper)
- [ ] Hessian matrix (intuition for DL)
- [ ] Backpropagation — full chain-rule walkthrough on a tiny neural net
- [ ] Activation function derivatives: sigmoid, tanh, ReLU
- [ ] Vanishing/exploding gradients — intuition

### Probability (DL-focused)
- [ ] Softmax distribution
- [ ] Cross-entropy loss
- [ ] KL divergence
- [ ] Entropy (information theory basics)

### Linear Algebra (DL-focused)
- [ ] Tensor basics (multi-dimensional arrays)
- [ ] Matrix calculus: derivative of `Wx + b`
- [ ] Convolution math: kernel, stride, padding

---

## 🤯 Phase 4 — Generative AI & LLMs (Months 6–8)

### Linear Algebra for Transformers
- [ ] Dot-product attention math
- [ ] Queries, Keys, Values as matrices
- [ ] Vector embeddings + cosine similarity
- [ ] SVD intuition (revisited in the embeddings/attention context)

### Information Theory (full)
- [ ] Entropy, cross-entropy, KL divergence — full treatment
- [ ] Mutual information (intuition)
- [ ] Perplexity

### Probability (LLM-heavy)
- [ ] Autoregressive modeling
- [ ] Likelihood of sequences
- [ ] Log-likelihood

### Optimization Extensions
- [ ] Constrained optimization
- [ ] Lagrange multipliers

---

## 🦾 Phase 5 — Autonomous Agents (Months 8–10)

*Light math phase — mostly logic + programming.*

- [ ] Markov chains (intro), state transitions
- [ ] Expectations in planning
- [ ] Graph theory basics: nodes, edges
- [ ] BFS/DFS ideas
- [ ] Combinatorics basics: counting, permutations, combinations (if not covered earlier)
- [ ] Discrete probability: indicator variables, union bound

---

## 💬 Phase 6 — Real-World Chatbots (Months 10–11)

*Almost no new math — mostly implementation.*

- [ ] Probability for intent classification (light)
- [ ] Vector embeddings recap (already learned in Phase 4)

---

## ☁️ Phase 7 — Deployment & Scaling (Month 12)

*Mostly DevOps/backend — minimal math.*

- [ ] Light statistics for logging & performance monitoring

---

## 🔧 Cross-Cutting: Numerical Methods & Computational Math

*Applied throughout Phases 2–3 wherever algorithms are implemented.*

- [ ] Numerical linear algebra stability
- [ ] Iterative methods (conjugate gradient, gradient methods)
- [ ] Basic numerical differentiation & integration
- [ ] Floating point basics, overflow/underflow, rounding errors

---

## 🎓 Phase 8 — Optional / Research-Ready (Later, if needed)

- [ ] Measure theory basics (only if going deep into probabilistic theory)
- [ ] Convex optimization: duality, KKT conditions
- [ ] Manifold learning & differential geometry basics
- [ ] Stochastic calculus (for RL or specialized topics)

---

## 🔁 How to Study Each Topic (Repeatable Micro-Plan)

For every topic above:

1. [ ] **Concept read** — short intro + intuition
2. [ ] **Key formulas** — write them on a cheat sheet
3. [ ] **Short derivation** — do 1 derivation by hand
4. [ ] **Practice problems** — 2–5 problems (compute, small proofs, toy implementations)
5. [ ] **Applied mini-project** — e.g. implement PCA on images; derive & train logistic regression on a toy dataset

---

## ✅ Immediate Starter Practice Tasks

- [ ] Compute dot product, norm, and projection for 3D vectors
- [ ] Solve a 2×2 linear system and compute its inverse
- [ ] Differentiate `f(x,y) = 3x²y + sin(xy)` w.r.t. `x` and `y` (chain rule practice)
- [ ] Derive the gradient descent update for `f(x) = ax² + bx + c` and run 5 iterations by hand
- [ ] Bayes coin-flip update: prior `Beta(2,2)`, observe 3 heads / 1 tail → find posterior

---

## 📋 Quick Study Order

1. Preliminaries: arithmetic, exponents, logs, algebra, sets, relations, functions, graphs, matrix basics
2. Vectors → Matrices → Matrix factorizations (SVD) → Eigenvalues
3. Single-variable calculus → Multivariable calculus (gradients/Jacobian/Hessian)
4. Gradient descent & convexity → backprop intuition
5. Probability basics → distributions → multivariate Gaussian
6. Bayesian basics + MLE/MAP → estimation & hypothesis testing
7. Numerical methods + condition numbers
8. Applied ML math (regression, logistic regression, PCA, tiny NN)
9. Information theory & constrained optimization
10. Advanced (optional): convex optimization / manifolds / measure theory
