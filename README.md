# Portuguese Bank Marketing Campaign Analysis

This project analyzes the **Portuguese Bank Marketing dataset**, which contains details about customer interactions during telemarketing campaigns. The main goal is to understand which factors influence whether a client subscribes to a term deposit and to build predictive models for classification.

## Project Structure
- `Portuguese bank notebook.ipynb` – main notebook containing data exploration, visualization, and model building.
- `bank-full.csv` – dataset used in the analysis (UCI Bank Marketing Dataset).

## Steps Covered
1. **Data Loading & Cleaning**  
   - Loaded the dataset into Pandas.  
   - Checked missing values, data types, and performed preprocessing (label encoding categorical variables).  

2. **Exploratory Data Analysis (EDA)**  
   - **Univariate analysis** – distribution of categorical and numerical features.  
   - **Bivariate analysis** – relationship between features (e.g., balance, previous contacts) and the target variable.  
   - Visualized patterns using bar plots and count plots.  

3. **Key Insights from EDA**  
   - Customers with higher account balances are more likely to subscribe.  
   - Clients contacted multiple times in previous campaigns show higher conversion rates.  
   - Duration of the last call is strongly correlated with subscription outcome.  

4. **Modeling**  
   Implemented multiple classification models:  
   - Logistic Regression  
   - Decision Tree Classifier  
   - Random Forest Classifier  
   - XGBoost Classifier  

   Features were scaled where necessary using `StandardScaler`.

5. **Model Evaluation**  
   - Accuracy Score  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-score)  

   Models were compared to find the best-performing one.

## Tools & Libraries
- Python (Pandas, NumPy, Matplotlib, Seaborn)  
- scikit-learn  
- XGBoost  

## Results
- Tree-based models (Random Forest, XGBoost) performed better than Logistic Regression in terms of accuracy and recall.  
- The analysis highlights key factors (balance, previous contacts, call duration) that strongly influence subscription likelihood.  

## How to Run
1. Clone this repository.  
2. Install required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook:  
   ```bash
   jupyter notebook "Portuguese bank notebook.ipynb"
