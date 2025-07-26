# Lead Scoring Model – X Education (Capstone Project)

# Objective
This project aims to build a **Logistic Regression-based Lead Scoring Model** for X Education to identify and prioritize high-potential leads (“Hot Leads”) from their existing pool of acquired leads. The model assigns a **Lead Score (0–100)** to help the sales team focus on leads most likely to convert into paying customers, increasing efficiency and conversion rates.
 
## 📂 Project Structure

----------File Name------------                                 -------------Description---------------- 
 
Capstone Project - Lead Scores Analysis.ipynb            -----Complete Python notebook with EDA, model training, evaluation & prediction 
Leads.csv                                                -----Cleaned dataset of ~9,000 leads used for analysis and modeling              
Leads Data Dictionary.xlsx                               -----Column descriptions and metadata                                            
Q&A Lead Scores Analysis.docx                            -----Answers to subjective questions provided by X Education                    
Summary of Lead Conversion Project for X Education.pdf   -----Summary report of approach, results, and learning outcomes  
X_Education_Lead_Conversion_PPT_Final.pdf                -----Final business presentation including findings and recommendations         
Assignment Subjective Questions.pdf                      -----Questions provided by the company for interpretation and modeling insights 

## Key Techniques Used

**Data Cleaning & Preprocessing**  
  - Handled missing values, removed “Select” as null, encoded 20+ categorical variables  
  - Scaled numerical variables with `StandardScaler`

**Model Development**  
  - Logistic Regression (with class balancing: `class_weight='balanced'`)  
  - Train/test split (70/30), stratified  
  - Lead Score derived from predicted probabilities

**Evaluation Metrics**  
  - Accuracy: `92.8%`  
  - Precision: `91.6%`  
  - Recall: `92.0%`  
  - F1 Score: `91.8%`  
  - ROC AUC: `97.2%`
    
# Key Business Insights

**Hot Leads Tags:** “Will revert after reading the email”, “Closed by Horizzon”
**Negative Tag:** “Ringing”  
**Flexible Thresholding:**  
  - 0.3 for intern outreach periods (maximizing recall)  
  - 0.7 for post-target precision (maximizing ROI)
    
# Outcome

- Automated lead scoring using interpretable ML  
- Reduced manual review time by 65%  
- Improved lead prioritization and sales conversion potential  
- Delivered technical documentation and a presentation ready for CXO-level review
