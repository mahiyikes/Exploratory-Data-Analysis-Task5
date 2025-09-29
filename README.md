📊 Titanic Dataset - Exploratory Data Analysis (EDA)



📌 Project Overview:-



This project performs an Exploratory Data Analysis (EDA) on the Titanic dataset from Kaggle’s Titanic Competition. 

The goal is to understand patterns in the data, identify key factors that influenced survival, handle missing values, engineer useful features, and summarize insights through visualizations.



🗂️ Repository Structure:-



titanic-eda/

├── notebook/

│   └── titanic\_eda\_colab.ipynb     # Main Jupyter/Colab notebook

├── outputs/

│   └── titanic\_eda.pdf             # Exported PDF report

├── figures/                        # Saved plots

│   ├── survived\_count.png

│   ├── survival\_by\_sex.png

│   └── ...

├── data/

│   └── train.csv                   # Kaggle dataset (not always uploaded to GitHub)

├── requirements.txt                 # Dependencies

└── README.md                        # Project documentation



⚙️ Installation \& Setup :-



Run in Google Colab (recommended)



* Open titanic\_eda\_colab.ipynb
* &nbsp;in Google Colab.
* Upload train.csv when prompted.
* Run all cells: Runtime → Run all.
* Export notebook to PDF: File → Print → Save as PDF.   



📈 Key Steps in Analysis:-



* Data Overview: Loaded and inspected Titanic dataset (train.csv), 891 rows × 12 columns.
* Missing Values: Identified missing data in Age, Cabin, and Embarked.
* Univariate Analysis: Distribution of Survived, Sex, Pclass, Age, Fare.
* Bivariate Analysis: Relationship of Sex, Pclass, Age with Survival.
* Feature Engineering: Created new features (Title, FamilySize, IsAlone, Deck).
* Handling Missing Data: Imputed Age using median per Sex \& Pclass, filled Embarked and Fare.
* Correlation Analysis: Heatmap and VIF to detect multicollinearity.
* Statistical Tests: Chi-square test for association between Sex and survival.
* Outliers: Examined Fare distribution and applied log transformation.



🔑 Insights:-



* The overall survival rate in the training set ≈ is approximately 38%.
* Sex is the strongest predictor: ~74% of females survived vs ~19% of males.
* Class matters: 1st class passengers had much higher survival rates than 3rd passengers.
* Younger passengers (children) tended to have better chances.
* Being alone (IsAlone=1) generally reduced survival probability.
* Cabin is mostly missing → limited value, but Deck can provide some information.



📦 Dependencies:-



* Python 3.8+
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* statsmodels
* missingno

(See requirements.txt for exact versions)



🚀 How to Contribute:-



* Fork the repo
* Create a feature branch (git checkout -b feature-name)
* Commit changes (git commit -m "Add feature")
* Push branch (git push origin feature-name)
* Open a Pull Request



