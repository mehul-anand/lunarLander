# lunarLander

## Overview
This project implements a reinforcement learning agent using the TD3 (Twin Delayed Deep Deterministic Policy Gradient) algorithm to solve the LunarLanderContinuous-v3 environment from OpenAI Gym. The agent is trained to land a lunar module safely using continuous control.

## Features
- Uses Stable Baselines3's TD3 algorithm
- Action noise for exploration
- Video recording of training and evaluation episodes
- Logging of training progress
- Evaluation in both headless and GUI modes

## Project Structure

```
lander_td3/
    lander_td3.ipynb         # Main Jupyter notebook for training and evaluation
    td3_lander.zip           # Saved model checkpoint
    logs/
        monitor.csv          # Training logs
        videos/              # Recorded videos of agent performance
            test_lander-step-0-to-step-600.mp4
            train_lander-step-0-to-step-10000.mp4
            ...
```

## Getting Started

### Prerequisites
- Python 3.8+
- [gymnasium](https://github.com/Farama-Foundation/Gymnasium)
- [stable-baselines3](https://github.com/DLR-RM/stable-baselines3)
- [pygame](https://www.pygame.org/)

Install dependencies:

```bash
pip install gymnasium[box2d] stable-baselines3 pygame
```

### Running the Notebook
Open `lander_td3/lander_td3.ipynb` in Jupyter and run all cells to train and evaluate the agent. Training videos and logs will be saved in the `logs/` directory.

### Viewing Results
- Training and evaluation videos are saved in `logs/videos/`.
- Training metrics are logged in `logs/monitor.csv`.

## References
- [Stable Baselines3 Documentation](https://stable-baselines3.readthedocs.io/)
- [OpenAI Gymnasium LunarLanderContinuous-v3](https://gymnasium.farama.org/environments/box2d/lunar_lander/)
