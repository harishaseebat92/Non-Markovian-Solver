# Non-Markovian-Solver
The repository contains code implementations, testing notebooks, and solutions to tackle the non-trivial problems presented by non-Markovian systems with memory effects.

# Non-Markovian Quantum Evolution

This repository focuses on solving and analyzing non-Markovian quantum evolution problems. It provides implementations for handling negative time-dependent rates (\(\gamma(t)\)), ensuring trace preservation during evolution, and adapting various solvers and integration methods for non-Markovian systems. The goal is to ensure that quantum evolution remains physically consistent, even in complex non-Markovian regimes.

## Key Features

- **Handling of Negative \(\gamma(t)\):** Implementations for solving non-Markovian systems with negative time-dependent decay rates, which are critical for capturing memory effects in quantum systems.
- **State Renormalization:** Techniques to ensure the trace of the quantum state remains equal to 1 at all times.
- **Custom Smoothing Functions:** Methods to smooth the time-dependent rates without altering their core dynamics.
- **Non-Markovian Monte Carlo Solver (nm_mcsolve):** Utilizes QuTiP's solver for non-Markovian systems, with a focus on handling time-dependent Hamiltonians and collapse operators.
- **Numerical Integration Methods:** Exploration of various ODE solvers (`lsoda`, `bdf`, `dop853`, etc.) for improved stability and accuracy when dealing with complex rates.
  
## Repository Structure

```bash
.
├── Notebooks/
│   ├── Markovian Solvers  # Jupyter notebook demonstrating solver usage
│   └── Non-Markovian Solvers    # Detailed analysis of evolution results
├── Results/
│   └── test_non_markovian.py # Unit tests to validate the solver and functions
├── docs/
│   └── README.md             # Documentation and explanations
└── requirements.txt          # Required libraries for running the code
