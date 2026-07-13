# Smart Card Customer Segmentation using Machine Learning

A customer segmentation project that applies **unsupervised machine learning** to cluster Smart Card customers based on demographics, purchasing behavior, and spending patterns. The project includes complete data preprocessing, feature engineering, dimensionality reduction, and clustering analysis.

---

## Project Overview

Customer segmentation helps businesses better understand their customers by grouping similar users together. These segments can be used for:

- Personalized marketing campaigns
- Customer retention strategies
- Product recommendations
- Customer lifetime value analysis
- Business decision making

This project performs clustering using **K-Means** and **Agglomerative Clustering** after extensive preprocessing and feature engineering.

---

## Dataset

The project uses a customer dataset named:

```
smartcart_customers.csv
```

The dataset contains customer demographic information, purchase history, campaign responses, and spending across different product categories.

---

## Project Workflow

### 1. Data Preprocessing

- Load dataset
- Handle missing values
- Convert date columns
- Remove unnecessary columns
- Detect and remove outliers

---

### 2. Feature Engineering

New features created include:

- **Age**
- **Tenure Days**
- **Total Spending**
- **Total Children**
- Simplified Education Categories
- Living Status (Partner / Alone)

---

### 3. Data Encoding

Categorical variables are encoded using:

- One-Hot Encoding

---

### 4. Feature Scaling

Numerical features are standardized using:

- StandardScaler

---

### 5. Dimensionality Reduction

Principal Component Analysis (PCA) is applied to reduce dimensionality while preserving most of the dataset variance.

- PCA Components: **3**

---

### 6. Clustering Algorithms

The following clustering techniques are implemented:

- K-Means Clustering
- Agglomerative Hierarchical Clustering

The optimal number of clusters is evaluated using:

- Elbow Method (WCSS)
- Silhouette Score

Final clustering uses:

```
Number of Clusters = 4
```

---

## Visualizations

The notebook includes several visualizations, such as:

- Pair plots
- Correlation heatmap
- PCA 3D visualization
- Elbow Curve
- Silhouette Score Curve
- Cluster visualization
- Cluster distribution count plot

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed

---

##  Required Libraries

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kneed
```

---

##  Project Structure

```
.
├── Samrt_Card_Clustering.ipynb
├── smartcart_customers.csv
├── README.md
└── requirements.txt (optional)
```

---

##  Machine Learning Pipeline

```
Dataset
    │
    ▼
Data Cleaning
    │
    ▼
Feature Engineering
    │
    ▼
Encoding
    │
    ▼
Feature Scaling
    │
    ▼
PCA
    │
    ▼
K-Means & Agglomerative Clustering
    │
    ▼
Customer Segments
```

---

##  Applications

The generated customer segments can be used for:

- Targeted marketing
- Customer profiling
- Product recommendation
- Loyalty programs
- Campaign optimization
- Customer behavior analysis

---

## Future Improvements

- DBSCAN clustering
- Gaussian Mixture Models (GMM)
- Interactive dashboards with Plotly
- Cluster profiling reports
- Model deployment using Streamlit
- Automated hyperparameter tuning

---

## License

This project is intended for educational and learning purposes.

---

## Author

Developed as a machine learning project for customer segmentation using unsupervised learning techniques.
