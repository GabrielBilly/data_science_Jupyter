# Airbnb Rio Project - Data Science


## Warning and Recommended:
	I used Google Colab for this project because it is a lot of complex and heavy files, I ended up using it to do the Deploly too (app.py)
	The files for carrying out this project must be downloaded and pushed to your Drive, and will be available in the "Folders and Files" block
	Here on GitHub I left the ProjetoAirbnb.ipynb file, which is the source code with the data analysis/visualization and machine training,
	app.py is the project deploy on streamlit(localhost)


### Project's goal:
	Property Price Prediction Tool for common people,
	Build a price prediction model that allows the average person to
	who own a property can find out how much they should charge for the daily rate of their property.
	Or even, for the common landlord, given the property he is looking for, help to know if that property is at an attractive price (below the average for properties with the same characteristics) or not.

### Description:
	On Airbnb, anyone who owns real estate of any kind
	You can offer your property to be rented per day.
	Just create your host profile (person who makes a property available per day) and create your property ad.
	In this advertisement, the host must describe the characteristics of the property as completely as possible,
	in order to help landlords choose the best property for them (and in order to make your advertisement more attractive)
	There are dozens of possible customizations in your ad, from the minimum number of nights, price, number of rooms, extra fee for extra guests, requirement to verify the identity of the landlord...
	For the forecasting model we will analyze the data ("dataset" available in the drive), and for the forecasting we will use the ExtraTrees Model,
	Model with the best R² and RSME results (R²: statistical measure that indicates how well a linear regression model performs with the data
	RSME: is a measure to assess the accuracy of regression models)


## Inspirations and Credits:
	The databases were removed from the site: [kaggle](https://www.kaggle.com/allanbruno/airbnb-rio-de-janeiro)
	Curso Python Impressionador - Prof Jõao Paulo Lira
	https://www.hashtagtreinamentos.com/


## Requirements:
### Libraries Used:
	from google.colab import drive
	from pyngrok import ngrok
	import joblib
	import streamlit as st
	import pathlib
	import pandas as pd


## Used folders and files:
	dataset (Folder with all Excel files with indicators for each year and month between 2018-2020,
	https://drive.google.com/drive/folders/1yJDXnx8fIXgi6GZQLtZHkF6Cjozy56R9?usp=share_link
	Lembrando que essa pasta dataset deve estar em seu Google Drive.
	The files created by the project ("dados.csv", "modelo.joblib") must be inserted in the Driver
	
	
### Att, Gabriel Souza
