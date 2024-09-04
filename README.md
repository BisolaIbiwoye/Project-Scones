## Project Scones Unlimited

# OVERVIEW
This project involves building an image classification model using AWS resources such as
(lambda, S3, Amazon sagemaker studio, step functions and CloudWatch) for Scones Unlimited 
(a scone-delivery-focused logistics). This model automatically detect which kind of vehicle 
delivery drivers have (bicycles and motorcycles) in order to route them to the correct loading bay and orders. 

Assigning delivery professionals who have a bicycle to nearby orders and giving motorcyclists orders
that are farther can help Scones Unlimited optimize their operations.

## Project Steps
1. Data Preparation

2. Model Training

3. Model Deployment

4. Creation of Lambda and step function workflow

5. Testing and evaluation

# Data Preparation
The data was prepared by extracting dataset from hosting service, transform it into a 
usable shape and format and loaded into a production system

# Model Training
Amazon SageMaker was utilized to train the image classification model using the prepared dataset. 
The model was fine-tuned to meet the specific requirements of Scones Unlimited, ensuring optimal performance.

# Model Deployment
The trained model with validation accuracy of above 80% was deployed and endpoints was generated
for real-time inferences. 

# Creation of Lambda and step function workflow
Three Lambda functions have been created, and the Step Functions visual editor was utilized to link them together. 
The first Lambda function handles data generation, the second manages image classification, and the third is tasked
with filtering out inferences with low confidence. Together, they facilitate the orchestration of serverless workflows.

# Testing and Evaluation
Several step function invocations were performed using data from the test dataset. 
Additionally, the data captured by SageMaker Model Monitor was utilized to create a visualization for monitoring the model.
