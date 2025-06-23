# Lunar Lander AI Agent (Deep Q-Learning)

This project implements a Deep Q-Learning (DQN) agent to solve the LunarLander-v3 environment from OpenAI Gymnasium.  
The agent learns how to land a lunar module safely by maximizing cumulative rewards through trial and error.

Built and trained entirely in Google Colab using PyTorch.

---

How It Works

- The agent uses a simple fully connected neural network (2 hidden layers) to approximate Q-values.
- A Replay Memory stores past experiences for better learning stability.
- Soft updates are applied to the target network.
- Trained with:
  - State size: 8
  - Action size: 4
  - Discount factor γ = 0.99
  - Learning rate = 5e-4

---

Libraries & Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

Running the Code

Since this was built and trained in Google Colab, to reproduce results:

1. Open the notebook in Colab: Google Colab Link

2. Run all cells (runtime ≈ should take few mins depending on your GPU)

3. The trained agent will save a video of successful landings in /results/.

Results

The agent was able to achieve an average score of 200+, meaning the environment is considered "solved."

Example landing videos can be found in /results/.

Project Structure

```

├── src/ # Main Python training script
├── results/ # Landing videos (mp4)
├── requirements.txt # Python dependencies
└── README.md # Project documentation
```

Author

Built with ❤️ by Ritesh

Note

This project was entirely implemented line-by-line — not generated — and trained/tested by the author in Colab.
