<img width="1275" alt="image" src="https://github.com/Lens101/snake_pygame/assets/21340292/50f6b3f8-9048-4f20-8072-fb29bdbb07fd">

Snake AI Training Script
This Python script implements an artificial intelligence agent to play the classic Snake game using deep reinforcement learning. The agent utilizes a deep Q-learning approach with a neural network model.

Files Description
agent.py
This file contains the main logic for training the Snake AI. It defines the Agent class, which encapsulates the AI's decision-making process, memory management, and training procedures. Key methods include get_state for obtaining the game state, remember for storing experiences in memory, and train_long_memory for training the neural network with a batch of experiences.

model.py
This file defines the neural network model (Linear_QNet) used by the AI agent. The model is a simple feedforward network with one hidden layer, and it is responsible for approximating the Q-values for different actions.

game.py
The game.py file contains the implementation of the Snake game environment. It defines the game logic, including the Snake's movement, collisions, food generation, and the game board.

helper.py
This script provides utility functions, such as plotting the game scores over time. The plot function helps visualize the agent's learning progress.

Training Procedure
The train function is the entry point for training the Snake AI. It initializes the game environment and the AI agent, and then runs a continuous training loop. The agent plays the game, collects experiences, and periodically trains its neural network using both short-term and long-term memory.

Usage
Environment Setup:

Install Anaconda.
Create a virtual environment and activate it:
bash
Copy code
conda create -n pygame_env python=3.8
conda activate pygame_env
Install Dependencies:

bash
Copy code
pip install pygame torch matplotlib ipython
Run the Training Script:

bash
Copy code
python agent.py
Watch as the Snake AI learns to play the game and achieves higher scores over time. The script also saves the best model, updating it whenever a new high score is achieved.

Feel free to experiment with the code, tune hyperparameters, and observe how the Snake AI improves its gameplay through reinforcement learning!
