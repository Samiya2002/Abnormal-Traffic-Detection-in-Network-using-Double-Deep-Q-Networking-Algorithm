# 🚦 Abnormal Traffic Detection in Network using Double Deep Q-Networking Algorithm

This project implements a Deep Reinforcement Learning (DRL) approach to detect abnormal network traffic using a **Double Deep Q-Network (DDQN)**. It utilizes a network traffic dataset, processes the data, and applies a reinforcement learning-based classifier to distinguish between normal and abnormal traffic patterns — which is crucial in cybersecurity for intrusion detection systems (IDS).

---

## 🧠 Overview

Traditional machine learning methods may struggle with dynamically adapting to new types of threats in network traffic. This project leverages a **DDQN-based agent**, which learns an optimal policy to identify malicious traffic by maximizing cumulative rewards over time.

---

## 🗂️ Project Structure

```
.
├── MajorProject_phase2.ipynb    # Main Jupyter notebook with data processing, model training, and evaluation
├── README.md                    # Project documentation (this file)
```

---

## 📊 Dataset

- **Source**: [CICIDS2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html)
- The dataset includes both benign and malicious traffic types (DoS, PortScan, Botnet, etc.)
- Preprocessing steps include feature selection, normalization, and label encoding.

---

## 🧪 Model

### Double Deep Q-Network (DDQN)

- A variation of Deep Q-Network (DQN) that reduces overestimation of Q-values.
- Uses two networks:
  - Online Q-Network (for selecting action)
  - Target Q-Network (for stable value estimation)

**State Space**: Selected network features  
**Action Space**: Binary classification (0 = normal, 1 = abnormal)  
**Reward**: +1 for correct classification, -1 otherwise

---

## 🛠️ Requirements

```bash
pip install pandas numpy scikit-learn tensorflow keras matplotlib
```

Or use:

```bash
conda install pandas numpy scikit-learn matplotlib
pip install tensorflow keras
```

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/Samiya2002/Abnormal-Traffic-Detection-in-Network-using-Double-Deep-Q-Networking-Algorithm.git
cd Abnormal-Traffic-Detection-in-Network-using-Double-Deep-Q-Networking-Algorithm
```

2. Open the notebook:

```bash
jupyter notebook MajorProject_phase2.ipynb
```

3. Run all cells sequentially to preprocess data, train the agent, and evaluate performance.

---

## 📈 Results

- The DDQN agent improves classification accuracy over time by learning from interaction with the environment.
- Performance is evaluated using accuracy, confusion matrix, and reward convergence plots.

---

## 📌 Key Libraries Used

- `TensorFlow` / `Keras` – Neural Network and DDQN implementation
- `sklearn` – Data preprocessing and metrics
- `pandas` – Data manipulation and analysis
- `matplotlib` – Data visualization

---


## 👩‍💻 Authors

- **Samiya Sadiq**
- [LinkedIn](https://www.linkedin.com/in/samiya-sadiq/)

---

## 📄 License

This project is licensed under the MIT License.
