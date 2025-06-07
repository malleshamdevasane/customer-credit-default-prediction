# Project Title
customer-credit-default-prediction
# Objective of README.md
This readme file is explanation of data_prep_and_analysis.ipynb file

# Note: 
- The column names within the raw train/test dataset have been renamed and hidden from the Amex end due to security reasons within Kaggle, hence there are in the form of D_64, P_2, etc.
- Total columns present within train_data.csv (i.e raw train data file) are 191 , excluding the customer_ID and target variable , total feature columns were 189
- After performing EDA (exlopratory data analysis) i.e from null percentage distribution (removing 90% or more null valued columns) , total feature columns were 176
- From zero percentage distribution, i.e columns which are more than 90% values as zero only, (means no variance witihn those columns), total feature columns were 175
- From feature selection techniques like IV (Information value) , we removed 85 columns , total feature columns were 90
- From person correlation technique we dropped 16 highly correlated variables , total feature columns were 72
