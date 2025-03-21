# Churn Telco Project

# 📌 Project Overview  
This project focuses on enhancing **customer churn prediction** for a telecommunications company by leveraging **machine learning** to detect high-risk customers. By improving the accuracy of churn prediction, the model helps businesses reduce customer attrition and optimize retention strategies.  

## 🚀 Key Contributions  
- **Developed a predictive model** to classify customers based on churn risk, increasing early detection and customer retention efforts.  
- **Implemented multiple machine learning models**, including **Logistic Regression, Random Forest, XGBoost, and LightGBM**, achieving an **AUC score of 0.85** and improving churn detection accuracy by **20%**.  
- **Visualized feature importance** using **SHAP values** to interpret model predictions and understand key drivers of customer churn.  

## 🛠 Technologies Used  
- **Machine Learning Models**: Logistic Regression, Random Forest, XGBoost, LightGBM  
- **Libraries**: Pandas, NumPy, Scikit-learn, LightGBM, XGBoost, SHAP, Seaborn, Matplotlib  
- **Data Processing**: PySpark for handling large datasets and performing data transformations  

## 📈 Business Impact  
✅ **Enhanced customer churn evaluation**: Improved churn detection accuracy, reducing customer attrition.  
✅ **Data-driven retention strategies**: Enabled targeted interventions by identifying key factors contributing to churn.  
✅ **Scalable and automated process**: Streamlined churn prediction without manual intervention.  

## 🔜 Next Steps  
🔹 Further **model tuning** to improve predictive accuracy and interpretability.  
🔹 **Deploying the model** as an API for real-time access via web applications.  
🔹 **Monitoring model performance** using drift detection techniques to maintain accuracy over time.  

## Prerequisites

- **Python 3.10**: Ensure Python 3.10 is installed on your system.
- **UV**: Used for managing project dependencies.

## Set up virtual env 
To set up your environment variables, you need to install prerequisites python and uv 

### 2. **Install UV**

#### On macOS and Linux.

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### On Windows.
```bash
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```
#### With pip.
```bash
# With pip.
pip install uv
```
### 3. **Package Management**
We use [UV](https://docs.astral.sh/uv/getting-started/features/) as a package management tool. Follow these steps

#### Create Virtual Environment (if not exist)
```bash
uv venv
```

### If pyproject.toml is not given or you want to modify packages
#### Create a new Python project 
```bash
uv init
```
This will create a pyproject.toml Add this text at the end of pyproject.toml in order to manage dependency in development environment.

Use uv to create a virtual environment named venv:

```bash
uv venv venv
```
#### Activate venv
Activate the virtual environment you just created:
```bash
source venv/bin/activate
```
#### Install requirements into a lockfile.
```bash
uv pip install -r requirements.txt pyproject.toml
```
#### Set up Juypter notebook kernel.
Run the following command to register your virtual environment as a kernel in Jupyter:
```bash
python -m ipykernel install --user --name=home_credit_risk --display-name "Python (home_credit_risk)"
```
## Notebooks

- **Churn_notebook.ipynb**: Notebook that cover part 1 Data Quality & EDA and Part 2 Model prediction workflow


## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── README.md          <- The top-level README for developers using this project
├── data
│   ├── external       <- Data from third party sources
│   ├── interim        <- Intermediate data that has been transformed
│   ├── processed      <- The final, canonical data sets for modeling
│   └── raw            <- The original, immutable data dump
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
└── src                         <- Source code for this project
    │
    ├── __init__.py             <- Makes src a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    │    
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    ├── plots.py                <- Code to create visualizations 
    │
    └── services                <- Service classes to connect with external platforms, tools, or APIs
        └── __init__.py 
```

--------