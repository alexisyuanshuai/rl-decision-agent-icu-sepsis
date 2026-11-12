# RL Decision Agent for ICU-Sepsis Benchmark

This project compares tabular and deep reinforcement-learning methods on the ICU-Sepsis benchmark, a discrete sequential-decision environment with 716 states and 25 actions.

## Project scope

- Implemented Q-learning and SARSA with epsilon-greedy exploration
- Tuned learning rate and exploration-decay schedules
- Evaluated tabular agents across multiple random seeds
- Implemented a Deep Q-Network with PyTorch, experience replay, and a target network
- Compared Q-learning, SARSA, and DQN across learning stability and sample efficiency

## Saved experiment results

The saved notebook run reports the following final average returns:

- Q-learning: 0.7867 +/- 0.0015
- SARSA: 0.7896 +/- 0.0014
- DQN: 0.7891 +/- 0.0032

These results reflect a course-scale implementation and should not be interpreted as a clinical evaluation.

## Technologies

- Python
- NumPy
- PyTorch
- Matplotlib
- Gymnasium
- ICU-Sepsis benchmark environment

## Running the notebook

Install the required packages:

```bash
pip install icu-sepsis gymnasium numpy matplotlib torch
```

Then open and run `RL Decision Agent for ICU-Sepsis Benchmark.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.

Some experiments run hundreds of thousands of episodes across multiple random seeds and may require substantial execution time.

## Disclaimer

This repository is an educational reinforcement-learning project. It is not a clinical decision-support system and must not be used to guide patient care.

