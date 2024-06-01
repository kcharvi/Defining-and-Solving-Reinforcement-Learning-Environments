# Defining and Solving Reinforcement Learning Environments

## 📋 Project Description

This project involves defining and solving various reinforcement learning (RL) environments using SARSA and tabular methods such as Q-learning and Double Q-learning. We explore both deterministic and stochastic environments across different scenarios: Frozen Lake, Lawn Mower, and Squirrel Maze. And we apply these techniques to a stock trading environment to demonstrate the versatility of these algorithms.

## 💻 Team Members

-   Charvi Kusuma [GitHub](https://github.com/kcharvi)
-   Tarun Reddi [GitHub](https://github.com/REDDITARUN)

## 🎯 Objective

The primary objective is for the agent to learn a policy that maximizes the cumulative reward over time in various grid-world environments. Each environment is designed with unique states, actions, and rewards to test the robustness of RL algorithms.

## 📁 Repository Structure

-   `environments/`: Source code for the environments.
-   `images/`: Images used in the environments.
-   `models/`: Saved models and results.
-   `reports/`: Project reports and documentation.
-   `README.md`: Project overview and instructions.

## 📚 Environments

### 1. Frozen Lake

The Frozen Lake environment is a 4x4 grid where the agent (a skater) must navigate from the start to the goal while avoiding holes and collecting gems.

#### Key Features:

-   **States**: Positions on the grid, including start, goal, holes, and gems.
-   **Actions**: Move left, right, up, or down.
-   **Rewards**: Positive rewards for reaching the goal and collecting gems; negative rewards for falling into holes or moving away from the goal.

### 2. Lawn Mower

The Lawn Mower environment simulates a mower navigating a lawn to cut grass while avoiding obstacles.

#### Key Features:

-   **States**: Grid positions representing lawn mower agent, battery and rock locations along with goal state.
-   **Actions**: Move left, right, up, or down.
-   **Rewards**: Positive rewards for reaching battery; negative rewards for hitting obstacles.

### 3. Squirrel Maze

The Squirrel Maze environment involves a squirrel navigating a grid to collect acorns and avoid hunters.

#### Key Features:

-   **States**: Positions on the grid, including start, acorns, hunters, and home.
-   **Actions**: Move left, right, up, or down.
-   **Rewards**: Positive rewards for collecting acorns and reaching home; negative rewards for encountering hunters.

### 4. Stock Trading

The Stock Trading environment simulates trading in a stock market, where the agent learns to buy and sell stocks to maximize profit.

#### Key Features:

-   **States**: Market conditions and portfolio status.
-   **Actions**: Buy, sell, hold.
-   **Rewards**: Profit or loss from trades.

## ❗Importance of This Project

1. **Technical Proficiency with Algorithms Implemented**: The project involves the implementation of advanced RL algorithms such as Q-learning and Double Q-learning, a quick start to understand and apply sophisticated reinforcement learning techniques. The custom design of multiple RL environments (Frozen Lake, Lawn Mower, Squirrel Maze, and Stock Trading) gives the capability to create and manipulate simulations, an essential skill in many AI and data science roles.

2. **Problem-Solving Skills with Deterministic and Stochastic Approaches and Reward Optimization**: By addressing both deterministic and stochastic environments, the project improves our ability to tackle uncertainty and variability, which are common in real-world scenarios. The strategic design of reward systems to guide agent behavior gives an understanding of optimization and objective-driven development.

3. **Data Analysis and Visualization**: Detailed analysis and comparison of different algorithms provide insights and gives us the ability to draw meaningful conclusions from data. The use of matplotlib for environment visualization and results plotting enhances our proficiency in presenting data clearly and effectively.

4. **Versatility with ease of Extending Application to Diverse Domains**: The application of RL to both grid-world scenarios and a stock trading environment gives the versatility and ability to adapt RL techniques to various domains, from robotics to finance.

5. **Innovation and Creativity with Custom Environments**: Creating unique environments like Lawn Mower and Squirrel Maze increases our creativity and ability to think outside the box, essential for innovation in technology roles. The inclusion of safety measures ensures ethical considerations are addressed, reflecting a responsible approach to AI development.

## 🌟 Features

-   **Defining RL Environments - Frozen Lake, Law Mower, Squirrel Maze and Stock Trading**: Detailed creation of both deterministic and stochastic environments.
-   **SARSA Implementation**: Step by Step solving with SARSA algorithm.
-   **Q-Learning Implementation**: In-depth application of Q-learning to solve creative environments.
-   **Other Tabular Method - Double Q Learning**: Exploration of different tabular methods for RL problem-solving.
-   **Stock Trading Environment**: Unique application of Q-learning in a simulated stock trading scenario.
-   **Comprehensive Analysis**: Extensive evaluation and comparison of different RL methods.

## 📈 Results Overview

### Frozen Lake

-   **Deterministic Q-Learning**: Showed a smooth decrease in epsilon and a steady increase in total rewards per episode, stabilizing at higher values indicating effective learning.
-   **Stochastic Q-Learning**: Demonstrated more fluctuations in rewards due to randomness, with epsilon decay less smooth compared to deterministic.
-   **Deterministic Double Q-Learning**: Performed slightly better than Q-Learning, with higher and more stable rewards.
-   **Stochastic Double Q-Learning**: Similar fluctuations as stochastic Q-Learning, but generally showed better performance over time.

1. Epsilon Decay Plot

-   **Description**: This plot shows how the epsilon value decreases over episodes, indicating the agent's transition from exploration to exploitation.

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/ef84589b-9b5d-47ab-8ac2-5c093ff96d9e)


2. Total Rewards per Episode

-   **Description**: This plot illustrates the cumulative rewards obtained by the agent in each episode, showing the learning progress over time.

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/bdf10023-f9a4-4aee-8b39-6975288589bc)


3. Q-Learning vs. Double Q-Learning Comparison

-   **Description**: A comparison of the performance of Q-Learning and Double Q-Learning algorithms in the Frozen Lake environment.

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/9681d2f8-6546-4f62-9d7c-6528f865472a)


### Lawn Mower

-   **SARSA**: Steady increase in rewards indicating effective policy learning. Performance might vary if adapted to stochastic environments.
-   **Double Q-Learning**: Achieved higher rewards compared to SARSA, showing improved learning efficiency. Potential for robust policy in stochastic environments.
-   **N-Step Bootstrapping**: Outperformed SARSA with a steady increase in rewards, showing the benefit of multi-step updates. Can handle stochasticity with more robustness.

1. Epsilon Decay Plot

<p align="center">
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/7c856c99-c183-4200-afdc-043da83758d1" alt="SARSA Epsilon Decay" width="300"/>
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/6c034df0-fc1a-45b9-a44d-c6bffe493308" alt="Q Learning Epsilon Decay" width="300"/>
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/eaef9a85-7b21-40cd-b877-854b048ecd59" alt="Double Q Epsilon Decay" width="300"/>
</p>
<p align="center">
  <b>SARSA Epsilon Decay</b> &nbsp;&nbsp;&nbsp;&nbsp; <b>Q Learning Epsilon Decay</b> &nbsp;&nbsp;&nbsp;&nbsp; <b>Double Q Epsilon Decay</b>
</p>


3. Total Rewards per Episode

<p align="center">
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/66611548-edf9-427f-8ff5-71b8810f95bf" alt="SARSA Total Rewards" width="300"/>
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/1eca5c95-087a-40c5-bb30-95c05249d548" alt="Q Learning Total Rewards" width="300"/>
  <img src="https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/0d8f5d2a-d265-4fa2-ab2a-095689921ec7" alt="Double Q Total Rewards" width="300"/>
</p>
<p align="center">
  <b>SARSA Total Rewards</b> &nbsp;&nbsp;&nbsp;&nbsp; <b>Q Learning Total Rewards</b> &nbsp;&nbsp;&nbsp;&nbsp; <b>Double Q Total Rewards</b>
</p>


5. SARSA vs. Double Q-Learning Comparison

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/bf78cf38-86a1-4fca-8f48-d35a65945fa9)


### Squirrel Maze

-   **Deterministic Q-Learning**: Showed steady increase in rewards with a smooth epsilon decay.
-   **Stochastic Q-Learning**: High variance in rewards due to environment randomness, less smooth epsilon decay.
-   **Deterministic Double Q-Learning**: Higher and more stable rewards compared to Q-Learning, better handling of state-action space.
-   **Stochastic Double Q-Learning**: High variance similar to stochastic Q-Learning, but occasionally higher peaks in rewards.

1. Epsilon Decay Plot

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/0063a9d5-4083-4337-ad09-9498abb604f5)


2. Total Rewards per Episode

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/e1361577-49c8-4ee6-94a1-0d2cba7b034c)


3. Comparison

    | Algorithm | Environment | Model Variation | Max Reward (Episode) | Episode 1000 Reward | Epsilon Decay Trend |
| --- | --- | --- | --- | --- | --- |
| Q-learning | Deterministic | Base Model | 400+ | 390 | Slow Decline |
| Q-learning | Deterministic | Hyperparameter Tuning (Max Timestamp, Decay Rate: 20, 0.75) | 800+ | 765 | Slow Decline |
| Q-learning | Deterministic | Hyperparameter Tuning (Max Timestamp, Decay Rate: 20, 0.995) | 800+ | 765 | Slow Decline |
| Q-learning | Stochastic | Base Model | 400+ | 305 | Slow Decline |
| Q-learning | Stochastic | Hyperparameter Tuning (Max Timestamp, Decay Rate: 20, 0.995) | 800+ | 660 | Slow Decline |
| Double Q-learning | Deterministic | Base Model | 400 | - | - |
| Double Q-learning | Stochastic | Base Model | 400+ | - | - |

### Stock Trading

-   **Q-Learning**: Demonstrated gradual increase in account value over episodes with expected fluctuations, indicating effective learning despite market volatility. Can be adapted to stochastic market conditions, reflecting real-world market dynamics, useful in algorithmic trading.

1. Epsilon Decay Plot

   ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/7bbacddf-d9f7-429c-b781-4f5a85648071)


2. Total Rewards per Episode

    ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/a8e5efa8-559b-4457-b1e8-fac392a73b54)


3. Account Value Over Time

-   **Description**: This plot shows how the agent's account value changes over time, indicating the profitability of the trading strategy.

   ![image](https://github.com/REDDITARUN/Defining-and-Solving-Reinforcement-Learning-Environments/assets/53268025/70f9baa4-4fe1-43fa-95c3-522d9a436014)


### Summary of Results for Each Environment

| Environment       | Algorithm            | Deterministic Environment Results                                                  | Stochastic Environment Results                                               |
| ----------------- | -------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **Frozen Lake**   | Q-Learning           | - Epsilon Decay: Smooth exponential decay                                          | - Epsilon Decay: Fluctuating due to randomness                               |
|                   |                      | - Total Rewards per Episode: Gradually increasing, stable at higher values         | - Total Rewards per Episode: Fluctuating with occasional high rewards        |
|                   | Double Q-Learning    | - Epsilon Decay: Smooth exponential decay                                          | - Epsilon Decay: Fluctuating due to randomness                               |
|                   |                      | - Total Rewards per Episode: Gradually increasing, slightly higher than Q-Learning | - Total Rewards per Episode: Fluctuating, generally lower than deterministic |
|                   |                      | - Comparison: Double Q-Learning performs slightly better in stable environments    | - Comparison: More variance observed, with occasional high rewards           |
| **Lawn Mower**    | SARSA                | - Total Rewards per Episode: Increasing steadily                                   | - Performance might vary if adapted to stochastic                            |
|                   | Double Q-Learning    | - Total Rewards per Episode: Higher rewards compared to SARSA                      | - Potential for robust policy in stochastic environment                      |
|                   | N-Step Bootstrapping | - Total Rewards per Episode: Steady increase, higher than SARSA                    | - Can handle stochasticity with more robustness                              |
|                   |                      | - Comparison: Double Q-Learning achieves better long-term rewards                  | - Higher variance expected with stochastic adjustments                       |
| **Squirrel Maze** | Q-Learning           | - Epsilon Decay: Smooth exponential decay                                          | - Epsilon Decay: Fluctuating due to randomness                               |
|                   |                      | - Total Rewards per Episode: Increasing steadily                                   | - Total Rewards per Episode: Fluctuating with high variance                  |
|                   | Double Q-Learning    | - Epsilon Decay: Smooth exponential decay                                          | - Epsilon Decay: Fluctuating due to randomness                               |
|                   |                      | - Total Rewards per Episode: Higher and more stable compared to Q-Learning         | - Total Rewards per Episode: Fluctuating, generally lower than deterministic |
|                   |                      | - Comparison: Double Q-Learning shows better reward dynamics                       | - Comparison: High variance with occasional peaks in rewards                 |
| **Stock Trading** | Q-Learning           | - Epsilon Decay: Smooth exponential decay                                          | - Adapts well to deterministic trading strategies                            |
|                   |                      | - Total Rewards per Episode: Initial fluctuations, eventually stabilizing          | - Can be adapted to stochastic market conditions                             |
|                   |                      | - Evaluation: Account value increases over time with fluctuations                  | - Reflects real-world market dynamics, useful in algorithmic trading         |

## 🖥️ Technologies Used

-   Python
-   Gymnasium Library
-   Matplotlib (for visualizations)
-   Various RL Algorithms
