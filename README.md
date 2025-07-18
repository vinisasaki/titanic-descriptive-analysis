# Titanic Descriptive Statistics

Exploratory analysis of the Titanic dataset (Kaggle) in Google Colab, using descriptive statistics and visualizations (histograms and boxplots) to explore age, fares, social class, and their interrelationships.

---

## 📁 Repository Structure

- **titanic-descriptive-analysis/**
  - **titanic_dataset/**
    - `gender_submission.csv`
    - `test.csv`
    - `train.csv`
  - `titanic_descriptive_analysis.ipynb`
  - `README.md`

---

## 📖 Data Source

The dataset was obtained from the Kaggle “Titanic: Machine Learning from Disaster” competition:  
https://www.kaggle.com/competitions/titanic/overview

---

## 🚀 How to Use in Google Colab

1. **Open the notebook in Colab**  
   - Go to https://colab.research.google.com  
   - Select **GitHub**, paste the repository URL: 
     ```
     https://github.com/vinisasaki/titanic-descriptive-analysis
     ```  
   - Open `titanic_descriptive_analysis.ipynb`.

2. **Load the dataset**  
   - Upload `train.csv` (located in `titanic_dataset/`) via the Files panel on the left, or
   - Mount your Google Drive and load it via code:
     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     df = pd.read_csv('/content/drive/MyDrive/data/train.csv')
     ```

3. **Run the cells**  
   - Execute each cell in order.
   - Pandas, Seaborn and Matplotlib are already pre-installed on Colab.

---

## 📊 Notebook Contents

1. **Initial inspection**: `df.info()`, `df.describe()`  
2. **Handling missing data** (`Age`, `Cabin`, `Embarked`)  
3. **Central tendency**: (mean, median, mode) 
4. **Dispersion**: (range, standard deviation, IQR, CV)
5. **Distribution shape**: (skewness, kurtosis)
6. **Visualizations**: (histograms, boxplots) 
7. **Key conclusions**  

---

## 📝 Key Findings

- **Typical profile**: 3rd-class passenger, 20–38 years old, fare around £14.45
- **Age**: slight right skew (skew ≈ 0.5), kurtosis ≈ 0.18 (near normal)  
- **Fare**: strong positive skew and very high kurtosis (excess ≈ 33.4), CV ≈ 1.54
- **Recommendation**: apply a logarithmic transformation to `Fare` for future analyses

---

>  
> [LinkedIn](https://www.linkedin.com/in/vinicius-sasaki) • [GitHub](https://github.com/vinisasaki)  
