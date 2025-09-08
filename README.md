# Crashing-to-Cruising
A Reinforcement Learning Project

---
Here the AI agent learns to drive in the CarRacing environment using the **Proximal Policy Optimization (PPO)** algorithm with **Stable-Baselines3** and **Gymnasium**.

This notebook demonstrates how to set up the CarRacing environment, shape rewards, train an agent using PPO, and evaluate its performance.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Environment Setup](#environment-setup)
- [Algorithm Used](#algorithm-used)
- [Installation](#installation)
- [Usage](#usage)
- [Training & Evaluation](#training--evaluation)
- [Results](#results)
- [Demo GIF](#demo-gif)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

---

## 📒 Project Overview

The goal of this project is to train an AI agent to drive a car smoothly and efficiently on a race track using reinforcement learning.

Key features:

* Reward shaping to encourage smoother steering and better control.
* Parallel environments for faster training.
* Visualization with TensorBoard and Matplotlib.
* Training using the PPO algorithm for stable and effective learning.

---

## 🏑 Environment Setup

The environment is based on the **CarRacing-v2** environment from Gymnasium, with the following enhancements:

* Custom reward shaping for smoother driving.
* Vectorized environments for parallel training.
* Logging and monitoring for better analysis.

---

## ⚙️ Algorithm Used

### Proximal Policy Optimization (PPO)

PPO is a reinforcement learning algorithm that balances exploration and exploitation while ensuring stable updates. It’s widely used due to its reliability and performance in continuous control tasks like CarRacing.

---

## 💻 Installation

### Clone this repository:

```bash
git clone <your-repository-url>
cd RL_Racing_car
```

### Install dependencies:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install gymnasium[box2d] stable-baselines3[extra] tensorboard opencv-python
```

For Google Colab users, the notebook includes setup cells to install these packages automatically.

---

## ▶ Usage

1. Open the notebook in **Google Colab** or **Jupyter Notebook**.
2. Mount Google Drive to save models and logs.
3. Run environment setup cells.
4. Train the PPO agent with specified hyperparameters.
5. Evaluate the agent’s performance and visualize the results.

---

## 📊 Training & Evaluation

* Monitor training with TensorBoard:

```bash
tensorboard --logdir=<your-log-directory>
```

* Save and reload models to test performance.
* Visualize rewards and gameplay using plots.

---

## 👥 Results

* The PPO algorithm provided stable learning and improved driving performance.
* Reward shaping encouraged smooth steering and efficient driving behavior.
* Training logs and evaluation plots help analyze agent improvements.

---

## 🎥 Demo GIF

Here’s how the trained car drives on the race track:

![Car Driving Demo](path/to/car_demo.gif)

*(Replace `path/to/car_demo.gif` with the actual path to your GIF in the repository.)*

---

## 📦 Dependencies

* Python 3.8+
* [Gymnasium](https://gymnasium.farama.org/)
* [Stable-Baselines3](https://stable-baselines3.readthedocs.io/)
* TensorBoard
* OpenCV
* NumPy
* Matplotlib
* PyTorch

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

* Experiment with different reward shaping methods.
* Improve visualizations and analysis.
* Optimize hyperparameters for better performance.

Please fork the repository and create a pull request.

---

## 📓 License

This project is open-source and available under the MIT License. See the [LICENSE](LICENSE) file for more details.
