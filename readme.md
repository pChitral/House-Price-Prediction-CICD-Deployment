# House Price Prediction CICD Deployment

This project is an end-to-end machine learning web application that predicts the prices of houses in Boston, Massachusetts. The application uses a linear regression model that was trained on the [Boston Housing dataset](https://archive.ics.uci.edu/ml/datasets/housing) to predict house prices based on various features such as the number of rooms, crime rate, and pupil-teacher ratio. The model is based on Linear Regression, and the predictions are made using Flask API.

## Table of Contents

- [House Price Prediction CICD Deployment](#house-price-prediction-cicd-deployment)
  - [Table of Contents](#table-of-contents)
  - [Boston House Pricing Prediction](#boston-house-pricing-prediction)
  - [Software and Tools Requirements](#software-and-tools-requirements)
  - [Files](#files)
  - [Dependencies](#dependencies)
  - [Running the Application](#running-the-application)
  - [Deploying the Application](#deploying-the-application)
  - [Usage](#usage)
  - [License](#license)

---

## Boston House Pricing Prediction

This project focuses on predicting the prices of houses in the Boston area based on various factors such as the number of rooms, area, location, and other factors. The trained machine learning model can be deployed using the Flask API provided in this repository.

<img width="569" alt="Screenshot 2023-04-16 at 2 46 33 PM" src="https://user-images.githubusercontent.com/69043137/232903712-5037d3ce-d7f7-4056-bc9f-1dc2e237c33e.png">


---

## Software and Tools Requirements

To run and deploy this project, you will need the following software and tools:

1. [Github Account](https://github.com)
2. [Heroku Account](https://heroku.com)
3. [VSCode IDE](https://code.visualstudio.com/)
4. [Git CLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)

Create a new environment using conda:

```
conda create -p venv python==3.9 -y
```


---

## Files

The following files are included in this project:

| File | Description |
| --- | --- |
| `app.py` | This file contains the Flask API code that loads the trained model and serves the predictions. |
| `Dockerfile` | This file contains the configuration for building the Docker container for deployment. |
| `Linear_Regression.ipynb` | This Jupyter notebook contains the code for training the machine learning model and generating the two pickle files (`scaling.pkl` and `regmodel.pkl`). |
| `LICENSE` | This file contains the license information for the project. |
| `Procfile` | This file contains the command to run the Flask app on Heroku. |
| `regmodel.pkl` | This file contains the trained machine learning model saved in a pickle format. |
| `requirements.txt` | This file contains the list of Python packages required to run the Flask app. |
| `scaling.pkl` | This file contains the fitted StandardScaler object saved in a pickle format. |
| `templates` | This directory contains the HTML templates for the Flask app. |
| `venv` | This directory contains the Python virtual environment. |

---

## Dependencies

The following Python packages are required to run the Flask app:

- Flask
- scikit-learn
- pandas
- numpy
- matplotlib
- gunicorn
- sklearn

---

## Running the Application

To run the application, activate the virtual environment using the following command:

```
source venv/bin/activate
```


Install the required packages using the following command:

```
pip install -r requirements.txt
```


Then, start the Flask app using the following command:

```
python app.py
```


The app should now be running on `http://localhost:5000/`.

---

## Deploying the Application

To deploy the application on Heroku, follow these steps:

1. Create a new Heroku app using the Heroku CLI or the Heroku Dashboard.
2. Set up a new Git repository for the project using the following

---

## Usage 
- The application can be run locally by running the ```app.py``` file. 
- The application can be accessed by navigating to ```http://localhost:5000``` in a web browser.

---

## License 


This project is licensed under the MIT License. See the `LICENSE` file for details.
