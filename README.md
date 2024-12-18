# AWS SageMaker XGBoost Deployment for Predicting Online Retail Metrics

This project demonstrates how to train, deploy, and invoke an XGBoost machine learning model using AWS SageMaker to predict online retail metrics. The input data is preprocessed from a CSV file and deployed as an endpoint for real-time predictions.

---

## **Project Overview**

### **Key Steps**
1. **Data Preparation**
   - The dataset (`Preprocessed_Online_Retail.csv`) contains preprocessed numeric features for online retail transactions.
   - Non-numeric columns are dropped, and the dataset is formatted for training.

2. **Model Training**
   - The XGBoost algorithm is used to train the model in AWS SageMaker.
   - Training is performed using SageMaker’s managed infrastructure.

3. **Model Deployment**
   - The trained model is deployed as a real-time endpoint in AWS SageMaker.

4. **Prediction**
   - A CSV-formatted payload is sent to the endpoint using `boto3` SageMaker runtime.
   - The endpoint returns predictions for single and multiple rows.

---

## **Technologies Used**
- **Python**: Programming language.
- **Pandas**: For data processing and CSV file handling.
- **AWS SageMaker**: For model training, deployment, and inference.
- **XGBoost**: Machine learning algorithm for regression tasks.
- **Boto3**: AWS SDK for interacting with SageMaker endpoints.

---

## **Prerequisites**
Before running this project, ensure you have:
1. An **AWS account** with the following services:
   - SageMaker
   - S3 bucket access
2. AWS credentials configured on your system.
3. **Python 3.x** installed.
4. Necessary libraries: `boto3`, `pandas`, `sagemaker`.

---

## **Setup Instructions**

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/aws-sagemaker-xgboost-retail.git
cd aws-sagemaker-xgboost-retail
