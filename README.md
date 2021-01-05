# Kaggle-Kiva-Crowdfunding

## Introduction
Kiva is a non-profit organization that provides financial services to poor and financially excluded people around the world. It establishes a bilateral relationship between individual lenders and borrowers with 0 interest rate. Through Kiva's work, students can pay for tuition, women can start businesses, farmers are able to invest in equipment and families can afford needed emergency care.

The dataset we collected contains loans issued in 2016-2018. Via our analysis, we would like to develop a predictive model to assess if a loan requested will be funded. Our results shall benefit both lenders and borrowers. For prospective borrowers, given their demographic data and business nature, our model suggests if Kiva is an optimal platform for them to obtain financial support. As the platform aborts projects with insufficient funding, foreseeing if their invested projects will be delivered shall guide lenders to wisely allocate their investment.

This notebook uses XGBoost and AutoML machine learning methods to analyze how lenders choose to fund a particular loan request in addition to predicting whether a loan request will be funded. The final model achieved 99.99% accuracy, 99.95% f1-score.
## Data Source
- [Data Science for Good: Kiva Crowdfunding](https://www.kaggle.com/kiva/data-science-for-good-kiva-crowdfunding)
- [National MPI from Oxford Poverty & Human Development Initiative](https://ophi.org.uk/wp-content/uploads/Table-1-National-Results-MPI-2020_vs2.xlsx)
## Environment Setup
```
# AutoML setup
!sudo apt-get install build-essential swig
!curl https://raw.githubusercontent.com/automl/auto-sklearn/master/requirements.txt | xargs -n 1 -L 1 pip install
!pip install auto-sklearn==0.10.0

# nltk setup
!python -m nltk.downloader 'punkt'
!python -m nltk.downloader 'averaged_perceptron_tagger'
!python -m nltk.downloader 'universal_tagset'
!pip install category_encoders

# XGBoost 
!pip install xgboost
```
