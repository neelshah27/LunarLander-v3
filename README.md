# 🚀 LunarLander-v3: Reinforcement Learning in Action

This project explores the use of Reinforcement Learning algorithms to solve the classic control problem in the OpenAI Gym environment: **LunarLander-v3**. Our goal was to train an agent capable of landing a lunar module safely using various RL strategies and compare their performance visually.

## 🎯 Problem Statement

Train an agent to land a lunar module between flags on rugged terrain by learning from interaction through rewards and penalties — using:

- **REINFORCE**: A Monte Carlo policy-gradient method.
- **Advantage Actor-Critic (A2C)**: Combines policy and value learning to improve stability and sample efficiency.

# 📂 Project Structure

LunarLander/
├── A2C_Latest.mp4                # Latest A2C model demo
├── A2C_best.mp4                  # Best-performing A2C agent demo
├── A2C_Reinforce_models.zip      # Trained model weights (A2C + REINFORCE)
├── ActorCritic_lunar_lander.zip  # Actor-Critic model snapshot
├── LunarLander_REINFORCE.ipynb   # Training notebook for REINFORCE
├── LunarLanderSAC.ipynb          # SAC implementation or placeholder
├── REINFORCE.mp4                 # REINFORCE agent demo video
├── Un-Trained.mp4                # Baseline video of random (untrained) agent
├── logs/
│   ├── best_model/
│   │   └── best_model.zip        # Best A2C model (stable-baselines3 format)
│   ├── best_model.zip            # Backup or flattened best model
│   └── evaluations.npz           # Evaluation metrics
├── policy.pth                    # Trained policy (PyTorch format)
├── ppo_logs/                     # PPO training logs (if applicable)
└── LunarLander_Slides.pdf        # Final presentation slides



## 🧠 Algorithms Used

### ✅ REINFORCE
- Pure policy-gradient method.
- High variance but intuitive and simple.
- Slower convergence but stable toward the end.

### ✅ A2C (Advantage Actor-Critic)
- Combines actor (policy) and critic (value function).
- Reduces variance and improves learning speed.
- Shows fluctuations during training but reaches convergence faster.

## 🎥 Model Comparisons

| Environment | Video Demo |
|-------------|------------|
| 🟥 **Untrained** | [Watch Untrained Agent](./Un-Trained.mp4) |
| 🟩 **REINFORCE (1000 Episodes)** | [Watch REINFORCE Agent](./REINFORCE.mp4) |
| 🟦 **A2C Best (100K Timesteps)** | [Watch A2C Agent](./A2C_best.mp4) |

> Tip: For a visual overview, check out the comparative slides [here](./LunarLander_Slides%20(2).pdf).

## 📊 Observations

- **REINFORCE** showed high variance but improved steadily across episodes.
- **A2C** learned faster but showed instability mid-training due to hyperparameter sensitivity.
- Reward and loss metrics were used to track convergence and learning behavior.

## 🔧 How to Use

1. Clone the repo
2. Install dependencies (`gym`, `torch`, `numpy`, etc.)
3. Run the notebooks to reproduce results or modify training
4. Play back demos via any video player

## 📎 Resources

- [OpenAI Gym: LunarLander-v3](https://www.gymlibrary.dev/environments/box2d/lunar_lander/)
- [REINFORCE paper](https://link.springer.com/article/10.1007/BF00992696)
- [Actor-Critic methods](https://medium.com/intro-to-artificial-intelligence/the-actor-critic-reinforcement-learning-algorithm-c8095a655c14)

---

## 📌 Author

**Neel Shah**  
Graduate Researcher – AI and Human-Computer Interaction  
📧 [LinkedIn](https://www.linkedin.com/in/neelshah27) | [Portfolio](#)

---

## ⭐️ Star this repo if you found it useful!
