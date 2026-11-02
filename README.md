# Connect Four AI

An experimental Connect Four agent exploring supervised learning and deep reinforcement learning, including a Dueling Double DQN approach and self-play.

## Project highlights

- Human-versus-agent gameplay.
- Baseline random and neural-network agents.
- Deep Q-Network (DQN) training.
- Dueling network architecture.
- Experience replay and target-network techniques.
- Self-play experiments and evaluation against baseline agents.

## Reported results

The original project notes report:
- Near-100% win rate against random agents.
- Approximately 83% win rate for the Dueling Double DQN agent.

These are project-reported results; evaluation details such as number of games, opponent policy, seeds and confidence intervals should be added before treating them as benchmark results.

## Technology

- Python
- TensorFlow / Keras
- NumPy
- Jupyter Notebook

## Repository contents

| File | Description |
|---|---|
| `main 1 - Copy 1.ipynb` | Main notebook containing implementation / experiments |
| `README.md` | Project documentation |

## Run locally

```bash
git clone https://github.com/Sandeep-kumar-IITR/connect-4.git
cd connect-4
python -m venv .venv
# Windows: .venv\\Scripts\\activate
# macOS/Linux: source .venv/bin/activate
pip install numpy tensorflow jupyter
jupyter notebook
```

Open the notebook and execute its cells in order. The exact dependency versions and execution entry point have not yet been formalized in this repository.

## How the agent learns

A DQN agent estimates action values for the available columns. During training, experience replay samples past transitions and a target network stabilizes temporal-difference updates. A dueling architecture separates state-value estimation from action advantages.

## Engineering improvements

- Add a clean Python package structure and a command-line training entry point.
- Pin tested dependencies in `requirements.txt`.
- Add deterministic evaluation scripts and report the number of test games.
- Include learning curves, ablation studies and example gameplay.
- Separate training, evaluation and interactive gameplay code.

## Author

**Sandeep Kumar** · [GitHub](https://github.com/Sandeep-kumar-IITR)
