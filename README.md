# ACIS Car Insurance Analytics Project

This repository contains data analysis, statistical testing, and predictive modeling for AlphaCare Insurance Solutions (ACIS). The goal is to identify low-risk customers and help ACIS develop better pricing strategies.

## Tasks

- Task 1: Exploratory Data Analysis  
- Task 2: Data Version Control (DVC)  
- Task 3: Hypothesis Testing  
- Task 4: Predictive Modeling  

## Tools Used

- Python  
- Git & GitHub  
- DVC  
- Pandas, Seaborn, Scikit-learn  

---

## Data Version Control (DVC)

This project uses DVC to manage and version control datasets, ensuring reproducibility and auditability of all analyses.

### Setup

1. Install DVC

```
pip install dvc
```
2. Initialize DVC

```
dvc init
```
3. Configure local remote storage

```
mkdir -p dvc_storage
dvc remote add -d localstorage ./dvc_storage
```
4. Track datasets

```
Add your dataset(s) to DVC:
```
5. dvc add data/MachineLearningRating_v3.csv

```
git add data/MachineLearningRating_v3.csv.dvc .gitignore dvc.yaml dvc.lock
git commit -m "Track dataset with DVC"
git push origin task-2
```
6. Push data to remote

```
dvc push
```
7. Reproducing the Environment

To reproduce the project and retrieve data files:

```
git clone https://github.com/saron03/acis-insurance-analytics.git
cd acis-insurance-analytics
pip install dvc
dvc pull
```
```
vbnet

Just replace your current README contents with this, and you’re good to go! 
```

