Youtube link:https://youtu.be/lxyI9S-M0Y8
Project Overview
  This project implements a Q-Learning-based artificial intelligence (AI) to control a player character in a simple 2D space shooter game. The goal of the AI is to learn how to defeat enemy ships by moving left/right and shooting. The game is built using the Pygame library, and the Q-Learning algorithm is used to train the agent to make optimal decisions based on the current state of the game.

Key Features
  Q-Learning Algorithm: The core of the project is the Q-Learning algorithm, which enables the agent to learn the optimal policy through trial and error.
  Game Environment: A simple 2D space shooter game where the player must defend against enemy ships.
  State Representation: The state of the game is represented by the relative positions of the player and enemies.
  Action Space: The agent can take four possible actions: move left, move right, shoot, or wait.
  Reward Mechanism: The reward function is designed to encourage hitting enemies while penalizing unnecessary movements and collisions.

Installation
  To run this project, you need to have Python installed along with the following libraries:
  pygame: For creating the game environment.
  numpy: For numerical computations.
  matplotlib: For plotting the training curve.
  dill: For saving/loading the Q-table.

Running the Code
  Clone the repository (if you downloaded it as a ZIP file, extract it).
  Open a terminal and navigate to the project directory.
  Run the main script:
  python main.py  

Optional Parameters
  Visual Mode: To enable visual mode (showing the game window during training), modify the show variable in the code.
  Training Episodes: The number of training episodes is set to 20,000 by default. You can adjust this value in the code.

  Code Structure
The project consists of the following files:

  main.py: The main script that initializes the game, trains the agent, and saves the trained Q-table.
  Player.py: Defines the Player class, which represents the player character.
  Enemy.py: Defines the Enemy class, which represents enemy ships.
  Bullet.py: Defines the Bullet class, which represents bullets fired by the player.
  qtable_*.pickle: Saved Q-table files generated during training.
  Results
  After training, the agent should be able to consistently defeat all enemies. The training progress is visualized using a moving average of rewards over 2000 episodes. The final Q-table is saved as a pickle file for future use.

Training Curve
  The training curve is saved as train_curve.png, showing the mean reward over 2000 episodes. This curve helps visualize how the agent's performance improves over time.

Q-Table
  The trained Q-table is saved as qtable_<timestamp>.pickle, where <timestamp> is the time when the training finished. This file can be loaded to reuse the trained model without retraining.

Contributing
  Contributions are welcome! If you have suggestions or improvements, feel free to fork this repository and submit a pull request. You can also open issues to report bugs or suggest features.


