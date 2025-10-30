Data preprocessing, preparation, and feature reduction are among the most critical steps before applying any Machine Learning (ML) model — they often determine 70–80% of the success of your model’s performance.

# Preprocessing	- Essential to ensure data quality and consistency
# Preparation	- Critical for representativeness and feature engineering
# Feature Reduction	- Important for efficiency and avoiding overfitting

# Data-Preprocessing-Preparation-and-Feature-reduction
This work is about creating AI Solution to learn  data preprocessing, preparation and Singular Value Decomposition for feature reduction using Using the UCI Communities &amp; Crime dataset. 

Here we have 128 columns total:
•	122 predictive features
•	5 non-predictive features 
•	1 goal/target variable

## 🧹 Data Preprocessing
  Load the dataset
  Find the numeric, non numeric , predictive and non-predictive
  non-predictive attributes such as state, county, community, communityname
  Split predictive columns by data type into numeric and categorical - these columns are needed further for processing.
  Filter only those columns for numeric data.
  Encode categorical columns
  Handle Missing Values 

## 🧩 Data Preparation
  Identify Key Predictive Factors using correleation
  Correlation gives both positive and negative correlated columns for the target
  
<img width="1026" height="814" alt="image" src="https://github.com/user-attachments/assets/966d4876-5449-4362-98cf-1619bb9a82d6" />

   Top 5 positively correlated features are choosen which are more affected by the target
<img width="1489" height="990" alt="image" src="https://github.com/user-attachments/assets/680417ff-3f56-423c-8298-7af7d39dca8a" />

   Spliting into training and testing to apply randon forest R² Score: 0.9999600609068787
   And gives key predictive features
ViolentCrimesPerPop    0.999918
LemasPctOfficDrugUn    0.000003
racepctblack           0.000003
population             0.000003
PctTeen2Par            0.000003
PctBSorMore            0.000003
PctYoungKids2Par       0.000003
PctKids2Par            0.000003
NumInShelters          0.000003
MedRentPctHousInc      0.000002
MalePctDivorce         0.000002
PctNotHSGrad           0.000002
PctWOFullPlumb         0.000002
racePctWhite           0.000002
TotalPctDiv            0.000002

# ⚙️ Feature Reduction
 # Prepare data for Singular Value Decomposition (SVD) 
   Analyse the components obtained and interpret their significance in relation to target prediction.
   SVD helps to find which feature contributes more to each compoenents
   High values shows more contribution

<img width="1489" height="790" alt="image" src="https://github.com/user-attachments/assets/7b6fdd26-a50d-41cc-9ef5-c6a416f03b68" />

  
  

   

