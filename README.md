# BUILDING AND DEPLOYMENT OF SENTIMENT ANALYSIS MODEL USING SAGEMAKER




## Project Overview:

In this project, I have used Amazon SageMaker to complete building and deploying of a sentiment analysis model(i.e entire machine learning workflow). The goal is to build a very simple web app in which a user can enter a movie review and the prediction model behind the scenes will predict whether it is Positive or Negative review. The prediction model is implemented using Pytorch framework and trainned on IMDB dataset.

## Project Instruction:

This entire project is done on Amazon sagemaker.I Used heavy GPU instances like ml.p2.xlarge in sagemaker for training the models. If you want execute this on local machine, you might want to train the model on subset of the training data from IMDB dataset. Also there are steps where we upload the data to amazon S3 instances in order to train using aws instances which you can totally ignore on local machines.To deploy the model we need amazon lambda service and API Gateway services also.

### Executions instructions:


**1.Clone the repository:**

* `git clone https://github.com/SRIHARSHA786/SENTIMENT-ANALYSIS-USING-LSTM-SAGEMAKER-DEPLOYMENT.git`

**2.Open the SageMaker Project.ipynb file:**

**3.Read and follow the instructions! You can find and download the dataset for this project in the notebook.**

### General Outline:

* Download the data.
* Preparing and Processing the data.
* Upload the data to S3.
* Build and Train the PyTorch Model.
* Testing the Model.
* Deploying the model for testing.
* Use the model for testing.
* Deploy the model for the web app.
* Use the model for the web app.


### Libraries:

The list below represents main libraries and its objects for the project.
* Amazon SageMaker (Build, train, and deploy a model)
* pytorch (LSTM classifier)

### Delete the Endpoint:

Remember to always SHUT DOWN YOUR ENDPOINT if you are no longer using it. You are charged for the length of time that the endpoint is running so if you forget and leave it on you could end up with an unexpectedly large bill.

`predictor.delete_endpoint()`