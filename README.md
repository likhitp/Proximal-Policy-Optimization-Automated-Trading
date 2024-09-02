# Proximal Policy Optimization for Automated Trading

This repository contains an ongoing project aimed at building an automated trading bot using the Proximal Policy Optimization (PPO) algorithm. The bot is specifically designed to trade Tesla (TSLA) stock based on historical data and a variety of technical indicators.

## 📋 Project Overview

### Objectives

1. **Data Acquisition**: Gather historical stock data for TSLA, focusing on preparing the data with relevant technical indicators for training and testing.
2. **Environment Setup**: Define the trading environment, including the state and action spaces, and implement a reward function tailored for trading performance.
3. **PPO Implementation**: Develop and train the PPO agent using the prepared data and environment.
4. **Testing and Evaluation**: Evaluate the trained model on unseen data to gauge its performance.
5. **Visualization and Analysis**: Provide comprehensive visualizations and analyses to understand the bot's behavior and effectiveness.
6. **Final Delivery**: Ensure the project is well-documented, with clean and optimized code for easy replication and further development.

## 🛠️ Project Phases

### Phase 1: Data Acquisition
- **Objective**: Obtain and preprocess historical TSLA stock data.
- **Steps**:
  - Download 1-hour interval data for TSLA from Yahoo Finance.
  - Define the training period (July 1, 2023 - December 31, 2023) and testing period (January 1, 2024 - June 30, 2024).
  - Calculate key technical indicators: Moving Averages (short-term and long-term), RSI, and MACD.
  - Clean the data to ensure it's ready for the reinforcement learning (RL) environment.

### Phase 2: Environment Setup
- **Objective**: Create a trading environment for the PPO agent.
- **Steps**:
  - Define action space: Buy, Sell, Hold.
  - Define state space: Price data (OHLCV) and technical indicators.
  - Implement a reward function with components for profit, risk-adjusted return, and a penalty for inactivity.
  - Initialize the environment with $10,000 capital and other parameters.

### Phase 3: PPO Implementation
- **Objective**: Implement and train the PPO algorithm.
- **Steps**:
  - Design a neural network model appropriate for trading tasks.
  - Configure PPO with suitable hyperparameters and optimization techniques.
  - Train the model using the training data, saving intermediate models and logs.

### Phase 4: Testing and Evaluation
- **Objective**: Test the PPO agent on the testing dataset.
- **Steps**:
  - Run the trained model on the testing data (January 1, 2024 - June 30, 2024).
  - Record actions and associated states and rewards.
  - Compare the bot’s performance against benchmarks like the buy-and-hold strategy.

### Phase 5: Visualization and Analysis
- **Objective**: Analyze and visualize the performance of the trading bot.
- **Steps**:
  - Visualize training metrics using tools like TensorBoard or Matplotlib.
  - Plot trading actions on TSLA's price chart.
  - Summarize the findings in a report, discussing strengths, weaknesses, and future improvements.

### Phase 6: Final Delivery
- **Objective**: Deliver a polished, well-documented project.
- **Steps**:
  - Review and clean the code, ensuring adherence to Python best practices.
  - Deliverables:
    - Jupyter notebook (`PPO_trading_.ipynb`) with the full implementation.
    - Model weights (`evaluations.npz`).
    - DataFrame containing actions and related data.
    - Visualizations and a brief analysis report.

## 📂 Repository Contents

- `PPO_trading_.ipynb`: The main Jupyter notebook containing the implementation of the PPO trading bot.
- `evaluations.npz`: Saved model weights for testing and evaluation purposes.
- **Data**: Historical TSLA data with calculated technical indicators (to be generated and processed as part of the project).

## 🚧 Project Status

This project is currently under active development. The primary goal is to refine the PPO model and improve its trading performance. Future updates will include more robust testing, additional technical indicators, and expanded evaluation metrics.

## 📊 Future Work

- Incorporating additional financial instruments and broader market data.
- Enhancing the reward function for better performance under different market conditions.
- Extending the model to support multi-asset portfolios.

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙌 Contributions

Contributions are welcome! If you have ideas for improvements, feel free to fork the repository and submit a pull request.

---

**Developed with a passion for AI and Finance by Likhit**
