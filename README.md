# 🪨 Rock vs Mine Prediction

A machine learning project that uses sonar data to classify underwater objects as either **rocks** or **mines** (metal cylinders). Built with Python and Logistic Regression using the classic SONAR dataset.

---

## 📌 Overview

Submarines and underwater vehicles use sonar signals to detect objects. This project trains a classification model on sonar frequency response data to distinguish between rocks and mines — a binary classification problem with real-world safety implications.

---

## 📊 Dataset

- **Source:** UCI Machine Learning Repository — SONAR Dataset
- **Samples:** 208 total
- **Features:** 60 numeric features representing energy levels at different sonar frequencies
- **Labels:**
  - `R` → Rock
  - `M` → Mine

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| NumPy | Numerical operations |
| Pandas | Data loading and exploration |
| Scikit-learn | Model training and evaluation |

---

## 🔁 Workflow

1. **Data Collection** — Load the sonar CSV dataset into a Pandas DataFrame
2. **Exploratory Analysis** — Inspect shape, statistics, and label distribution
3. **Preprocessing** — Separate features (X) and labels (Y)
4. **Train/Test Split** — Split data into training and testing sets
5. **Model Training** — Train a Logistic Regression classifier
6. **Evaluation** — Measure accuracy on both training and testing data
7. **Prediction** — Feed new sonar readings to get Rock or Mine output

---

## 📈 Results

| Dataset | Accuracy |
|---|---|
| Training | ~83.4% |
| Testing | ~76.2% |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas scikit-learn
```

### Run the Notebook

```bash
git clone https://github.com/adam109alt/rock-vs-mine-prediction.git
cd rock-vs-mine-prediction
jupyter notebook Rock_vs_mine_prediction.ipynb
```

Make sure the sonar dataset CSV file is placed in the correct path referenced in the notebook.

---

## 🔮 Making a Prediction

Pass 60 sonar frequency values as input and the model will output:

```
Rock   →  if the object is a rock
Mine   →  if the object is a metal cylinder (mine)
```

---

## 📁 Project Structure

```
rock-vs-mine-prediction/
│
├── Rock_vs_mine_prediction.ipynb   # Main notebook
├── sonar_data.csv                  # Dataset
└── README.md                       # Project documentation
```

---

## 🙌 Acknowledgements

- Dataset originally collected by R. Paul Gorman and Terrence J. Sejnowski and published on the [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/Connectionist+Bench+(Sonar,+Mines+vs.+Rocks)).
