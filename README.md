# Capstone
This repository contains all the information required to replicate the unsupervised classification model I apply to game names and game descriptions in an attempt to categorize similar themed games.

In order to run this model, you will need to download the following software and create connections between different services. The data required to replicate the model will be provided as a separate file.

## Github:
You will need to store the script to be run in a Github repository. In order to do this, create a free personal Github account by navigating to https://github.com/ and following the prompts on the right hand side of your screen. You will need a current email address to complete the verification step. An email with an account verification link will be sent to your email address. Once you click this link, you can then begin using your Github account. In order to create a Github repository, navigate to the top left hand corner of your homepage and beside the word Repositories, click the green button with the words "New". Name the repository and provide a brief description of your repository. Finally, click the "Create Repository" button and you will have completed this step. 

## Airflow: 
Airflow is a platform to programmatically author, schedule and monitor workflows. Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed.

Before we download Airflow, you will need to ensure that you have Python and MySQL installed and running on your local machine in the same environment you are working in.

Some operating systems come with Python pre-installed, in order to check this, type the following command on your terminal and it should print out the version of Python you are currently running

`python`

If you do not have Python installed, in order to download Python, navigate to the Python downloads page here https://www.python.org/downloads/ and download Python 3.8. Follow the installation instructions and reopen your terminal and run the command above again.

In order to download MySQL, navigate to the MySQL downloads page here https://www.python.org/downloads/ and follow the installation instructions. Once you have MySQL properly download, return to your terminal and run the commands below

`cd /usr/local/mysql`

to navigate to the path where you MySQL installation was saved and finally run

`sudo bin/mysql_secure_installation` to install My SQL on your local environment. 

You will be presented with the following prompts, first your computer password. While typing it no characters will be displayed which is normal so don’t worry. Press Enter when finished. This will start a script which will ask you several questions and then reconfigure MySQL.

`Set root password? [Y/n]`
Select `Y` and press Enter. After that enter a password for MySQL and press Enter. Re-enter the password and press Enter again. This will be the password that IncoPOS will need when connecting to MySQL server.

`Remove anonymous users? [Y/n]`
Select `Y` and press Enter. You don’t need anyone but you or someone you told your password to touch your data.

`Disallow root login remotely? [Y/n]`
This information will be accessed only from your computer so select `Y`. In all cases this can later be changed by using the same commands.

`Remove test database and access to it? [Y/n]`
Select `Y` and press Enter. You don’t need that test database so it is safe to remove it.

`Reload privilege tables now? [Y/n]`
Select `Y` and press Enter. This will make the changes you did effective now. Now you have MySQL installed and secured on your Mac.

Now navigate to the command line interface on your local terminal or the terminal on the notebook you are working in and download Apache Airflow using the following commands

`pip install apache-airflow[all]`

This will download all API libraries 

If you encounter any errors that indicate MySQL hasn't been found try running the following commands 
`export PATH="/usr/local/mysql/bin/:$PATH"`

`pip install mysqlclient`

`brew install freetds` for Mac users and finally rerun the following command 

`pip install apache-airflow[all]`

In order to test the Airflow connection we will require a database, for now, we will not connect any project specific database to the Airflow instance, but instead, we will use the default SQLite option. 

After connecting to your database, you will need to initialize the database by running the following command in your terminal 

`airflow initdb`


## Setting up Travis CI:


## Setting up Google Cloud Platform (GCP):
## Connecting GCP, Github and Travis CI:
