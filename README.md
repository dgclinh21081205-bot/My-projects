# My-projects
A few of my projects during the academic year

# Selected Projects

I can only publish two of my projects publicly. The following projects showcase my experience in **machine learning, credit risk analysis, data preprocessing, exploratory data analysis, and model interpretation**.

## 1. Debt Group Classification with Machine Learning

An end-to-end machine learning pipeline for classifying Vietnamese loan records into **5 debt-risk groups** using `NHOMNO` and `NHOMNOMOI` as target variables.

### Key Work

* Cleaned and standardized approximately 27,000 labeled loan records, including mixed date formats, locale-specific numerical formats, inconsistent labels, duplicates, and logical inconsistencies.
* Engineered credit-risk features including loan term, loan age, remaining days, utilization, and log-transformed balances.
* Applied **leakage-safe feature selection** using VIF and mutual information on the training set only.
* Compared Logistic Regression, Random Forest, XGBoost, and SVM using cross-validation and validation-set model selection.
* Applied **SMOTE within cross-validation folds** and class weighting to address severe class imbalance.
* Used per-class threshold tuning to improve minority-class F1 performance.
* Applied **SHAP** to interpret model predictions and identify key credit-risk drivers.
* Selected XGBoost as the best-performing model, achieving a test F1-macro of **0.630 for NHOMNO** and **0.606 for NHOMNOMOI**.

### Key Findings

The most important predictors included **remaining days to maturity, loan purpose, product type, utilization, loan age, and exposure size**. Misclassifications were concentrated between adjacent debt groups, reflecting the continuous nature of debt-risk boundaries.

### Technologies

**Python, pandas, NumPy, scikit-learn, XGBoost, imbalanced-learn, SHAP, statsmodels, Jupyter Notebook**

---

## 2. Spotify Track Popularity & Trends Visualization

An exploratory data analysis and visualization project investigating factors associated with **Spotify track popularity and music trends** using a dataset of more than 8,500 tracks.

### Key Work

* Cleaned and prepared Spotify track data, including missing-value treatment and outlier detection.
* Applied log transformation to highly skewed variables such as artist follower counts.
* Encoded categorical variables using one-hot encoding.
* Conducted distribution analysis using histograms, KDE plots, and boxplots.
* Examined relationships between track popularity, artist popularity, artist followers, album characteristics, and track duration.
* Used correlation analysis and pairplots to identify relationships among key variables.
* Compared average track popularity across album types.

### Key Findings

* `artist_popularity` showed a moderate positive relationship with `track_popularity` (**r = 0.47**).
* `artist_followers` was strongly correlated with `artist_popularity` (**r = 0.64**) but had only a weak relationship with `track_popularity` (**r = 0.23**).
* Album tracks had the highest average popularity (**55.66**), followed by singles (**46.36**) and compilations (**40.54**).
* Track duration showed no meaningful relationship with popularity.

### Technologies

**Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook**

---

## Project Focus

These projects demonstrate practical experience in:

* Data cleaning and preprocessing
* Feature engineering
* Exploratory data analysis
* Machine learning classification
* Imbalanced-data handling
* Cross-validation and model selection
* Data leakage prevention
* Model interpretation with SHAP
* Statistical analysis and visualization
* Translating analytical results into actionable insights
