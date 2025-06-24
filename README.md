# Task-2: Exploratory Data Analysis (EDA)

###  **Dataset**

* **File:** `heart.csv`
* **Location:** Local upload
* **Target Variable:** `target` (0 = no heart disease, 1 = has heart disease)

### **Tools & Libraries**

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly

### **Steps Performed**

1. **Loaded the dataset**
   Displayed shape, `head()`, and `info()` for initial understanding.
2. **Generated summary statistics**
   Used `describe()` and `isnull().sum()` to check data distribution and missing values.
3. **Visualized numeric features**
   * **Histograms** to see distributions
   * **Boxplots** to detect outliers
4. **Explored feature relationships**
   * **Correlation Matrix Heatmap** using `sns.heatmap()`
   * **Pairplot** with hue as `target` to visualize group-wise relationships
5. **Identified patterns, trends, and anomalies**
   * **Target distribution**
   * **Age vs. target**
   * **Chest pain type vs. target**
   * **Heart rate, ST depression, ECG, and other features vs. target**
   * **Outliers** in `chol` and `trestbps` identified via boxplots
6. **Plotted comparisons using countplots and boxplots**
   * Grouped comparisons: `sex`, `cp`, `fbs`, `restecg`, `thalach`, `oldpeak`, etc.

### **Feature-Level Inferences**

* **Age:** Heart disease common in age group 50–60
* **Chest Pain (cp):** Types 1 & 2 strongly linked with disease
* **Thalach:** Higher heart rates → less disease
* **Oldpeak:** Higher values → more likely to have disease
* **Sex:** Males more prone to heart disease
* **Fbs, Chol, Trestbps:** Weak predictors with outliers

### **Output**

* Clean visuals: histograms, boxplots, countplots, heatmap, pairplot
* Basic understanding of important vs. less important features
* Dataset now ready for model building with relevant insights
