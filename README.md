# 📊 Clustering Analysis: Understanding and Implementing K-Means, Hierarchical, and DBSCAN

## 🎯 Objective

The objective of this project is to gain hands-on experience with various **clustering algorithms**—specifically **K-Means**, **Hierarchical**, and **DBSCAN**—by applying them to a real-world airline customer dataset. This project aims to identify meaningful customer segments to uncover insights from customer behavior.

---

## 📂 Dataset

The dataset used is from `EastWestAirlines.xlsx`, containing frequent flyer information for airline customers. Key files include:

- `data.csv`: Sheet from the Excel file with the actual customer data.
- `Description.csv`: Column descriptions for understanding dataset variables.

---

## 🧾 Columns Description

| Column | Description |
|--------|-------------|
| `ID#` | Unique identifier for each customer |
| `Balance` | Miles eligible for award travel |
| `Qual_miles` | Qualifying miles for top-tier status |
| `cc1_miles`, `cc2_miles`, `cc3_miles` | Miles from 3 credit card programs (rated 1 to 5) |
| `Bonus_miles` | Non-flight bonus miles |
| `Bonus_trans` | Non-flight bonus transactions |
| `Flight_miles_12mo` | Flight miles in the last 12 months |
| `Flight_trans_12` | Flight transactions in the last 12 months |
| `Days_since_enroll` | Days since customer enrollment |
| `Award?` | Whether the customer redeemed an award in the last 12 months |

---

## 📁 Repository Contents

- `Clustering.ipynb`: Jupyter Notebook with full implementation—EDA, clustering (K-Means, Hierarchical, DBSCAN), visualization, and evaluation.
- `EastWestAirlines.xlsx`: Dataset source file.
- `Clustering Analysis.docx`: Project documentation.
- `data.csv` and `Description.csv`: Extracted sheets for analysis.

---

## 🛠️ Tools and Libraries

- `pandas`, `numpy`: Data handling and manipulation
- `matplotlib`, `seaborn`: Visualization
- `scikit-learn`: Clustering algorithms, scaling, PCA, evaluation metrics
- `scipy`: Dendrograms for hierarchical clustering
- `openpyxl`: Reading `.xlsx` files

---

## 🔄 Project Workflow

1. **Data Loading & Cleaning**  
   - Load data and inspect (`head`, `info`, `describe`)
   - Handle missing values and outliers  
   - Normalize data using `StandardScaler`

2. **EDA**  
   - Histograms, boxplots, scatter plots  
   - Correlation heatmaps  

3. **Clustering Algorithms**  
   - **K-Means**: Optimal K via Elbow method  
   - **Hierarchical**: Linkage + Dendrogram visualization  
   - **DBSCAN**: Tune `eps` and `min_samples`  

4. **Visualization**  
   - 2D PCA projection of clusters  
   - Colored scatter plots  

5. **Evaluation**  
   - Internal evaluation using **Silhouette Score**

---

## 🚀 How to Run

### 🖥️ Step-by-step (Bash)


### 1. Clone the repository
git clone https://github.com/your-username/clustering-analysis.git
cd clustering-analysis

### 2. Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn scipy openpyxl

### 3. Launch Jupyter Notebook
jupyter notebook
Then open and run Clustering.ipynb in your browser.


## 📌 Insights & Interpretation
Cluster Profiles: Each clustering technique yields distinct groups of customers based on features like balance, award redemption, and flight frequency.

PCA Visualization: Helps in understanding cluster separation and data spread.

Evaluation: Silhouette Score guides which algorithm performs best.

## 🧠 Conclusion
This project demonstrates the practical application of clustering for customer segmentation in a frequent flyer context. It also highlights how data preprocessing, algorithm selection, and parameter tuning critically affect clustering performance.

## 📬 Contact
For feedback, suggestions, or collaboration, feel free to reach out via GitHub or email.
