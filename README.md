Customer-Personality-Segmentation-using-K-Means-Clustering-for-Targeted-Marketing-Strategies
Data-driven customer segmentation using K-Means clustering on behavioral and demographic data. Identifies distinct customer groups to enable targeted marketing, improve personalization, and optimize business decision-making through actionable insights.

Project Overview
Customer Personality Analysis involves understanding customer behavior to enable targeted marketing and personalization.

This project applies K-Means Clustering on a real-world dataset (2240 customers, 29 features) to identify meaningful customer segments based on demographics, spending habits, and campaign responses.

Problem Statement:
Businesses often rely on generic marketing strategies that fail to capture diverse customer behavior.

This project aims to:
1.Segment customers into distinct groups
2.Identify high-value and potential customers
3.Enable data-driven marketing strategies

Gaps in Existing System:
1.No personalized marketing strategy
2.Underutilization of customer data
3.Lack of behavioral segmentation
4.Inefficient marketing spend
5.No insight into campaign effectiveness

Dataset Description:
📊 Records: 2240 customers
📈 Features: 29 variables

Feature Categories:
Demographics: Age, Education, Income
Household: Kidhome, Teenhome
Spending: Wines, Fruits, Meat, Fish, Sweets, Gold
Purchases: Web, Store, Catalog
Engagement: Recency, Web Visits
Campaigns: AcceptedCmp1–5, Response

flowchart 
A[Dataset] --> B[Data Preprocessing]
B --> C[Feature Engineering]
C --> D[EDA]
D --> E[Feature Scaling]
E --> F[K-Means Clustering]
F --> G[Evaluation]
G --> H[Visualization]
H --> I[Business Insights]


Project Workflow:
1.Data Preprocessing
Handling missing values (Income)
Removing outliers
Encoding categorical variables
Feature scaling using StandardScaler

2.Feature Engineering
Age = Current Year - Year_Birth
Total Spending = Sum of all spending features
Total Purchases = Sum of all purchase features
Customer Tenure from joining date
Model Used:
K-Means Clustering (Unsupervised Learning)

3.Choosing Optimal Clusters:(EDA):
Elbow Method
Silhouette Score

4.Evaluation Metrics
Inertia (WCSS) → Cluster compactness
Silhouette Score → Cluster separation

5.Visualizations
1.Elbow Method
2.Cluster Visualization
3.PCA Projection

Key Insights:
1.High Income + High Spending → Premium Customers
2.Low Income + High Spending → Deal Seekers
3.High Income + Low Spending → Potential Customers
4.Low Income + Low Spending → Low Value Customers
5.Frequent Buyers → Loyal Customers

Business Recommendations:
1.Target premium customers with exclusive offers
2.Retain loyal customers using reward programs
3.Convert potential customers with personalized campaigns
4.Optimize marketing budget using segmentation

Project Structure:
customer-personality-segmentation/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── clustering.py
│   ├── evaluation.py
│
├── outputs/
│   ├── plots/
│   ├── cluster_results.csv
│
├── app/
│   └── streamlit_app.py
│
├── README.md
├── requirements.txt
└── .gitignore

How to Run:
# Clone the repo
git clone https://github.com/your-username/customer-segmentation.git

# Navigate to project
cd customer-segmentation

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook

Technologies Used
1.Python
2.Pandas, NumPy
3.Scikit-learn
4.Matplotlib, Seaborn
5.PCA
6.(Optional) Streamlit

Future Improvements:
1.Compare with DBSCAN & Hierarchical Clustering


Author
Afra Fathima
Data Analysis Enthusiast

⭐ If you like this project

Give it a ⭐ on GitHub and share it!
