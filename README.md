# 🛒 Market Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Machine%20Learning-f7931e?logo=scikit-learn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

> Segment customers into meaningful groups using unsupervised machine learning — helping businesses make smarter, data-driven marketing decisions.

---

## 📌 Overview

This project applies **K-Means Clustering** to customer purchase and behavioral data to identify distinct market segments. By grouping customers with similar characteristics, businesses can tailor their marketing strategies, improve customer experience, and maximize ROI.

The project includes:
- Exploratory data analysis (EDA) and preprocessing
- Optimal cluster selection using the **Elbow Method**
- K-Means model training and evaluation
- A deployable web application (`app.py`) for real-time customer segmentation

---

## 📁 Repository Structure

```
Market_Segmentation/
│
├── Market_Segmentation.ipynb       # Main Jupyter Notebook (EDA + Modeling)
├── Customer Data.csv               # Raw customer dataset
├── Clustered_Customer_Data.csv     # Dataset with assigned cluster labels
├── kmeans_model.pkl                # Trained K-Means model (pickle format)
├── final_model.sav                 # Final saved model (joblib format)
├── app.py                          # Web application for live predictions
└── README.md                       # Project documentation
```

---

## 🧠 How It Works

### 1. Data Preprocessing
- Load the customer dataset and handle missing values
- Encode categorical variables and scale numerical features

### 2. Exploratory Data Analysis (EDA)
- Visualize feature distributions
- Identify correlations and patterns in customer behavior

### 3. Finding Optimal Clusters
- Use the **Elbow Method** (Within-Cluster Sum of Squares) to determine the best value of *k*

### 4. K-Means Clustering
- Train the K-Means model on the processed data
- Assign cluster labels to each customer

### 5. Interpretation & Visualization
- Visualize clusters using 2D/3D plots
- Profile each segment (e.g., high-value customers, budget shoppers, etc.)

### 6. Web App Deployment
- `app.py` provides an interactive interface for predicting the segment of a new customer

---

## 📊 Dataset

| File | Description |
|---|---|
| `Customer Data.csv` | Raw input data with customer attributes |
| `Clustered_Customer_Data.csv` | Output data with cluster labels appended |

> **Note:** The dataset includes features such as customer demographics, spending scores, and purchase history.

---

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.8 or higher
- pip

### Clone the Repository

```bash
git clone https://github.com/Nishanta-13/Market_Segmentation.git
cd Market_Segmentation
```

### Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn streamlit joblib
```

---

## 🚀 Usage

### Run the Jupyter Notebook

Open and run the notebook step by step to reproduce the full analysis:

```bash
jupyter notebook Market_Segmentation.ipynb
```

### Launch the Web App

Run the interactive web application to segment new customers in real time:

```bash
streamlit run app.py
```

Then open your browser at `http://localhost:8501`.

---

## 📈 Results

The model successfully segments customers into **distinct clusters**, each representing a unique customer profile. Example segments might include:

| Cluster | Profile |
|---|---|
| 0 | Low income, low spending — Budget-conscious shoppers |
| 1 | High income, high spending — Premium customers |
| 2 | Medium income, high spending — Aspirational buyers |
| 3 | High income, low spending — Selective / conservative spenders |

> Actual clusters and labels depend on the trained model output.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Python** | Core programming language |
| **Pandas & NumPy** | Data manipulation |
| **Matplotlib & Seaborn** | Data visualization |
| **scikit-learn** | K-Means clustering |
| **Streamlit** | Web app deployment |
| **Jupyter Notebook** | Interactive development |

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Nishanta**  
🔗 [GitHub Profile](https://github.com/Nishanta-13)

---

> ⭐ If you found this project helpful, please consider giving it a star!
