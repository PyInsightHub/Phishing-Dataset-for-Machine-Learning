# Phishing-Dataset-for-Machine-Learning

About Dataset
Context
Anti-phishing refers to efforts to block phishing attacks. Phishing is a kind of cybercrime where attackers pose as known or trusted entities and contact individuals through email, text or telephone and ask them to share sensitive information. Typically, in a phishing email attack, and the message will suggest that there is a problem with an invoice, that there has been suspicious activity on an account, or that the user must login to verify an account or password. Users may also be prompted to enter credit card information or bank account details as well as other sensitive data. Once this information is collected, attackers may use it to access accounts, steal data and identities, and download malware onto the user’s computer.

Content
This dataset contains 48 features extracted from 5000 phishing webpages and 5000 legitimate webpages, which were downloaded from January to May 2015 and from May to June 2017. An improved feature extraction technique is employed by leveraging the browser automation framework (i.e., Selenium WebDriver), which is more precise and robust compared to the parsing approach based on regular expressions.

Anti-phishing researchers and experts may find this dataset useful for phishing features analysis, conducting rapid proof of concept experiments or benchmarking phishing classification models.

🧠 Goal: To develop a Machine Learning model that accurately identifies phishing websites by analyzing URL-based features — strengthening cybersecurity and user trust through data-driven insights.

Inquiry Pipeline:

1️⃣ Imports & Config:
Set up Python environment with essential ML and visualization libraries to ensure a reproducible workflow.

2️⃣ Load Data:
Loaded the Phishing vs Legitimate Websites dataset for analysis and model building.

3️⃣ Quick Data Audit:
Checked missing values, data types, and overall dataset health before processing.

4️⃣ Target Column Detection:
Identified the dependent variable (phishing / legitimate) to guide model training.

5️⃣Features & Basic Cleaning:
Cleaned, encoded, and standardized the feature set to ensure quality model inputs.

6️⃣ EDA: Class Balance:
Visualized data imbalance to understand distribution of phishing vs legitimate samples.

7️⃣ EDA: Correlations (Numeric):
Explored numerical feature relationships using heatmaps to detect strong correlations.

8️⃣ EDA: Top Feature Distributions:
Plotted key feature trends distinguishing phishing from legitimate URLs.

9️⃣ Feature Selection (Optional):
Retained the most informative predictors to reduce noise and improve accuracy.

🔟Train/Validation Split:
Split data into training and testing sets to enable unbiased performance evaluation.

1️⃣1️⃣ Model Pipelines:
Built modular pipelines for multiple models — Logistic Regression, Decision Tree, and Random Forest.

1️⃣2️⃣ Train & Evaluate (Holdout):
Evaluated models on holdout data.RandomForestClassifier delivered the highest F1-score and ROC-AUC — proving most reliable for phishing detection.

1️⃣3️⃣ Cross-Validation Leaderboard:
Compared models via cross-validation to confirm RandomForest’s consistent performance.

1️⃣4️⃣ Feature Importance (Tree-Based):
Visualized top predictive factors — URL length, HTTPS presence, and domain features were key indicators.

1️⃣5️⃣ Save Best Model (Optional):
Saved the final trained model for deployment and real-time phishing detection use.

Random Forest outperformed all models in both F1-score and ROC-AUC, proving ideal for security-based ML detection.
