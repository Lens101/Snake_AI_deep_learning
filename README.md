<img width="1275" alt="image" src="https://github.com/Lens101/snake_pygame/assets/21340292/50f6b3f8-9048-4f20-8072-fb29bdbb07fd">

# Snake AI

Welcome to Snake AI, a Python implementation of the classic Snake game with an artificial intelligence agent. This project utilizes Pygame for the game interface and PyTorch for the AI agent.

## Setup Instructions

To run the Snake AI, follow the steps below:

1. Install [Anaconda](https://www.anaconda.com/): https://www.anaconda.com/

2. Open a terminal and check if Anaconda is installed by running:
    ```bash
    conda --version
    ```

3. Create a virtual environment using conda:
    ```bash
    conda create -n pygame_env python=3.8
    ```

4. Activate the virtual environment:
    ```bash
    conda activate pygame_env
    ```

5. Install required dependencies:
    ```bash
    pip install pygame torch matplotlib ipython
    ```

6. Run the Snake AI:
    ```bash
    python agent.py
    ```

Now you're ready to experience the Snake AI in action!

## Project Structure

### `agent.py`

This is the main script that initiates and runs the Snake AI. It handles the game loop, user input, and interaction with the AI agent.

### `Linear_QNet.py`

The file contains the definition of the neural network model (`Linear_QNet`) used by the AI agent. It implements the required forward pass function.

### `DQNAgent.py`

This script implements the Deep Q-Learning agent (`DQNAgent`) that learns to play the Snake game using the defined neural network model.

### `game.py`

The Snake game environment is defined in this file. It includes the game logic, such as updating the game state, handling collisions, and managing the game board.

### `utils.py`

This file contains utility functions used throughout the project, such as converting the game state to a tensor.

Feel free to explore the code and experiment with the Snake AI. Enjoy playing and learning from the implementation!
