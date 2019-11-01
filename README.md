# Capstone
This repository contains all the information required to replicate the unsupervised classification model I apply to game names and game descriptions in an attempt to categorize similar themed games.

In order to run this model, you will need to download the following software and create connections between different services. The data required to replicate the model will be provided as a separate file.

## Github:
You will need to store the script to be run in a Github repository. In order to do this, create a free personal Github account by navigating to https://github.com/ and following the prompts on the right hand side of your screen. You will need a current email address to complete the verification step. An email with an account verification link will be sent to your email address. Once you click this link, you can then begin using your Github account. In order to create a Github repository, navigate to the top left hand corner of your homepage and beside the word Repositories, click the green button with the words "New". Name the repository and provide a brief description of your repository. Finally, click the "Create Repository" button and you will have completed this step. 

## Airflow: 
Airflow is a platform to programmatically author, schedule and monitor workflows. Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed.

Navigate to the command line interface on your local terminal or the terminal on the notebook you are working in and download Apache Airflow using the following commands

`pip install apache-airflow[all]`
This will download all API libraries 

For now, we will not connect a database to the Airflow, but we will use the default SQLite option. 

After connecting to your database, you will need to initialize the database by running the following command in your terminal 

`airflow initdb`



## Setting up Travis CI:
## Setting up Google Cloud Platform (GCP):
## Connecting GCP, Github and Travis CI:
