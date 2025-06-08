# Abnormal Traffic Detection using Double Deep Q-Network (DDQN)

This project applies **Reinforcement Learning**—specifically, a **Double Deep Q-Network (DDQN)**—to detect abnormal (malicious) traffic within network data. It leverages a custom OpenAI Gym environment built on top of the **NSL-KDD** dataset, a standard benchmark in intrusion detection systems (IDS).

## 📌 Overview

- **Dataset**: [NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html)
- **Algorithm**: Double Deep Q-Learning (DDQN)
- **Environment**: Custom Gym Environment simulating network traffic behavior
- **Goal**: Classify each traffic record as normal or abnormal using reinforcement learning

## 🚀 Key Features

- Preprocessing pipeline for NSL-KDD data (label encoding, normalization)
- Custom OpenAI Gym environment
- Double DQN with experience replay and target network updates
- Evaluation using accuracy, reward trends, and confusion matrix

## 🧠 DDQN Concept

- Uses **two networks**: one to select the action (policy) and one to evaluate it (target)
- Addresses overestimation bias found in standard DQN
- Reinforces learning through rewards based on classification accuracy

## 🗂️ Files

- `Abnormal_Traffic_Detection_DDQN.ipynb` – Main Colab notebook
- `environment.py` (within the notebook) – Contains custom Gym environment class
- `data` – Loaded programmatically (NSL-KDD train/test datasets)

## 📈 Results

- Agent learns to distinguish between normal and abnormal traffic over episodes
- Rewards per episode increase, indicating improved performance
- Accuracy and confusion matrix show effective classification

## 🔧 Requirements

This runs in **Google Colab**. If running locally, install:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow keras gym
