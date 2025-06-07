# Project Title
customer-credit-default-prediction
# Objective of README.md
This readme file is regarding the static data files used or created while data preparation, data analysis and feature selection

# Data Dictionary of the static files 

| Files | Link | Description |
| ------ | ------ | -------
| train_data.csv | [https://drive.google.com/file/d/1cq82NiPXy_q0Z2QMndO3-IOvvS7XQrtM/view?usp=drive_link] | Raw train dataset (~70k records), customer_ID (primary key), and target (target variable)
| test_data.csv | [https://drive.google.com/file/d/1pTMwDq_kFajr6npg-AaAJ0V1937ewbZ5/view?usp=drive_link]|   Raw test dataset (~33k records), customer_ID (primary key)
| processed_train_data.csv | [https://drive.google.com/file/d/1X1oX14hq2fe8zaGnyDcNGNzIqlJ6_vYy/view?usp=drive_link] | Processed or updated train dataset, after applying EDA and feature selection
| processed_test_data.csv | [https://drive.google.com/file/d/1POTdB98u2E5xw-u70rnY0bJ__GEyOl2A/view?usp=drive_link] | Processed or updated test dataset, after applying EDA and feature selection
| IV_result.csv | [https://drive.google.com/file/d/149r22r62s6WC56RNpzBQx07x-UfmJ19I/view?usp=drive_link]] | Information-value file, having feature name and IV-value 
| null_percentage_df.csv | [https://drive.google.com/file/d/1ABF8TC-0OZLI0syAI_Sy5MF0GdmrTnyM/view?usp=drive_link] | The file contains the null percentage of all the 190 columns in raw train dataset
| zero_percentage_df.csv | [https://drive.google.com/file/d/1NagoSpvowbFSJFTjYxZZBh5HMagvlmAX/view?usp=drive_link] | The file contains the zero value percentage of all the 190 columns in in raw train dataset
| train_labels.csv | [https://drive.google.com/file/d/1szRLpSJJLT33GVhK6mjLIiVkfTKD4aYl/view?usp=drive_link] | The file contains the target variable corresponding to every custoemr_ID, the raw train_data.csv is created by merging it with this file 


# Note: 
- The column names within the raw train/test dataset have been renamed and hidden from the Amex end due to security reasons within Kaggle, hence there are in the form of D_64, P_2, etc.
- Total columns present within train_data.csv (i.e raw train data file) are 191 , excluding the customer_ID and target variable , total feature columns were 189
- After performing EDA (exlopratory data analysis) i.e from null percentage distribution (removing 90% or more null valued columns) , total feature columns were 176
- From zero percentage distribution, i.e columns which are more than 90% values as zero only, (means no variance witihn those columns), total feature columns were 175
- From feature selection techniques like IV (Information value) , we removed 85 columns , total feature columns were 90
- From person correlation technique we dropped 16 highly correlated variables , total feature columns were 72
