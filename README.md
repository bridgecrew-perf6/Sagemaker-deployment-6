# Sagemaker-deployment

This walkthrough notebook will take you through the steps required to build your model for sentiment analysis, deploy it using Amazon Sagemaker, test it on a separate data set, and build your web app to analyse sentiments without any pre-processing required. 

## Setting up a Notebook Instance
The deployment project you will be working on is intended to be done using Amazon's SageMaker platform. In particular, it is assumed that you have a working notebook instance in which you can clone the deployment repository.

Step 1. Go to AWS SageMaker
First, start by logging in to the AWS console, opening the SageMaker dashboard, and clicking on Create notebook instance.

Step 2. Create a notebook instance
The Create notebook instance wizard will come up, asking you the following information:

Notebook instance settings - In this section, you may choose the notebook instance name of your choice. By default, a ml.t2.medium type is available. But, we will use ml.p2.xlarge for training a model and ml.m4.xlarge for deployment. > Note that your notebook may have a different name than the one displayed here.
Permissions and encryption - Next, under IAM role field select Create a new role.
Create an IAM role - You should get a pop-up dialog box, where you have to select None radio-button under S3 buckets you specify field.
Network - optional - Choose the No VPC option.

Git repositories - Here you will clone the https://github.com/udacity/sagemaker-deployment.git repository to the current notebook instance only.

You're done! Click on Create notebook instance button.

The notebook provided in this reposity along with predict.py and train.py have the solutions. 
