# **Traffic Accident Hotspot Prediction**

A real-world, data-driven Smart City solution to support safer roads and better decision-making.

---

## **Project Overview**
This project applies **Machine Learning and Data Science techniques** on a Road Traffic Accident (RTA) dataset to identify **high-risk accident patterns (hotspots)** and predict **accident severity**.

The goal is to:  
- Understand accident trends based on **time, road, driver, and environment conditions**  
- Detect **high-risk hotspot-like conditions** that contribute to severe accidents  
- Build a model to **predict accident severity** for better safety planning  

---

## **Tech Stack** 
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**  
- **Seaborn**  
- **Scikit-Learn** (RandomForest, OneHotEncoder, DBSCAN optional)  

---

## **Steps Performed ** 

### **Data Cleaning & Preprocessing**  
- Removed/handled missing values (`na`, nulls)  
- Converted the **Time** column into a usable format  
- Created a new feature: **Hour** (extracted from Time)  
- Prepared data for Machine Learning using encoding techniques  

---

### **Exploratory Data Analysis** (EDA)  
- Accident severity distribution analysis  
- Severity comparison across:  
  - **Day of week**  
  - **Hour of day (peak accident times)**  
  - **Road surface type**  
  - **Weather and light conditions**  
- Identified major contributing accident causes  

---

### **Hotspot / Risk Pattern Identification**  
Since the dataset does not contain GPS coordinates, hotspots are analyzed as:  
 **High-risk conditions** rather than location-based map hotspots  

Examples:  
- High-risk accident hours  
- Road surface types leading to severe injuries  
- Driving conditions that increase fatal/serious accident probability  

---

### **Feature Encoding & Model Preparation**  
Used:  
- **OneHotEncoder** for categorical features  
- Train-test split with stratification for balanced evaluation  

---

### **Machine Learning Model Training**  
Trained a classification model using:  
- **Random Forest Classifier**  

The model predicts accident severity levels:  
- Slight Injury  
- Serious Injury  
- Fatal Injury  

---

## **Results**  
- Built a working ML pipeline to predict accident severity  
- Discovered high-risk patterns such as:  
  • Peak risk hours during the day  
  • Road surface conditions linked to higher severity  
  • Top accident causes contributing to severe outcomes  

---

## **What I Learned**  
- How to build an end-to-end ML pipeline on real-world accident data  
- Handling categorical-heavy datasets using OneHotEncoding  
- Importance of EDA to uncover meaningful safety insights  
- Model evaluation using classification report and confusion matrix  
- Identifying real-world accident risk patterns for Smart City applications  

---

## **Future Improvements**  
- Add **latitude/longitude** to perform true map-based hotspot detection  
- Integrate **weather + traffic APIs** for real-time risk forecasting  
- Improve minority class prediction using **SMOTE / XGBoost / LightGBM**  
- Deploy as a **Smart City Road Safety Dashboard** using Streamlit  
- Provide automated **prevention recommendations

- 
