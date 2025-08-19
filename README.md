
# Deploy Random Forest Model in Azure

In this project, I will build and deploy a Random Forest machine learning model using the Titanic dataset to predict whether a passenger survived or not. The Titanic dataset is a classic dataset in machine learning, containing information about passengers such as age, gender, class, and other features.

The primary objective of this project is to create a web application that allows users to input passenger details and get predictions in real time. I will implement the application using Flask, a lightweight Python web framework, and deploy it on Microsoft Azure as a cloud-based service.

Once deployed, the web application will have a publicly accessible URL, providing an interactive interface where users can input data and see survival predictions instantly. This project demonstrates end-to-end machine learning workflow — from data preprocessing and model training to cloud deployment and web integration.


## About files

* titanic_survive_model_for_api.py: This file is used for data preprocessing and model training. A Random Forest model is trained on the preprocessed Titanic dataset and then saved as a pickle file for later deployment in the API.

* Front-End Development: The HTML and CSS files for the web application’s interface were created and organized into templates and static folders, respectively. The templates folder contains the HTML files that define the structure of the web pages, while the static folder holds the CSS files to style the application, providing a clean and user-friendly interface

* The app.py file serves as the main Flask application for the Titanic survival prediction project. It loads the pre-trained Random Forest model from the titanic_model.pkl pickle file and provides both a web interface and an API endpoint for making predictions. The root route (/) renders the home page (home.html) where users can input passenger details. The /predict route processes these inputs, converts them into a format suitable for the model, predicts whether the passenger survived or not, and displays the result on the web page. Additionally, the /predict_api route allows direct API calls using JSON data, returning survival predictions programmatically. This setup enables seamless interaction with the model, both through a user-friendly web interface and via API requests, making it ready for deployment on Azure with a public URL
