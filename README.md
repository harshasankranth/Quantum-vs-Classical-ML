# Quantum vs Classical Neural Network — Binary Classification

A hands-on comparison of a Variational Quantum Circuit (VQC) against 
a Classical Neural Network on a non-linearly separable dataset.

Built as part of my exploration into Quantum Machine Learning.

## Results

| Metric | Classical NN | Quantum NN |
|--------|-------------|------------|
| Accuracy | 90.00% | 72.50% |
| Parameters | 50+ | 6 |
| Training Speed | Fast | Slow |
| Hardware | Classical CPU | Simulated QPU |
| Scalability | High | Promising |

## Key Observations

- Classical NN achieved higher accuracy with more parameters
- Quantum NN used only 6 trainable parameters — significantly fewer
- The quantum model exhibited a different decision strategy entirely
- Cost curve showed oscillation — likely due to Barren Plateau phenomenon
- Quantum advantage not yet realized on classical simulation hardware

## What I Learned

Quantum ML is not yet superior to classical ML for standard tasks.
However the fundamental difference in HOW the two models learn
is the real insight. Quantum circuits explore solution spaces
differently through superposition and entanglement — which may
prove advantageous for specific problem types in the future.

## Tech Stack

- PennyLane — Quantum circuit design and training
- scikit-learn — Classical neural network and dataset
- matplotlib — Visualization
- Python 3.x

## How to Run

Open in Google Colab or locally:
```bash
pip install pennylane scikit-learn matplotlib numpy
jupyter notebook quantum_vs_classical_classification.ipynb
```

## Dataset

Make Moons — a non-linearly separable binary classification dataset
with 200 samples and 0.1 noise factor.

## References

- PennyLane Documentation
- Cerezo et al. — Variational Quantum Algorithms (2021)
- Schuld & Petruccione — Machine Learning with Quantum Computers
