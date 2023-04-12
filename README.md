# Projeto Airbnb Rio - Ciência de Dados


## Aviso e Recomendados:
	Utilizei o Google Colab para este projeto pois se trata de vários arquivos complexos e pesados,
	Os Arquivos devem estar baixados em seu Drive, e estarão disponíveis aqui: https://drive.google.com/drive/folders/1yJDXnx8fIXgi6GZQLtZHkF6Cjozy56R9?usp=share_link
	Aqui no GitHub deixei 2 arquivos, O ProjetoAirbnb.ipynb que é o código fonte com o treinamento dos modelos para previsão de preço,
	e o DeployProjetoAirbnb.ipynb que é o Deploy do programa onde é feito a previsão de preço com os indicadores inseridos pelo usúario.
	Devemos rodar primeiro o ProjetoAirbnb.ipynb para treinamento do modelo, após isso rodamos o DeployProjetoAirbnb.ipynb 
	
 
### Objetivo do Projeto:
	Ferramenta de Previsão de Preço de Imóvel para pessoas comuns,
	Construir um modelo de previsão de preço que permita uma pessoa comum
	que possui um imóvel possa saber quanto deve cobrar pela diária do seu imóvel.
	Ou ainda, para o locador comum, dado o imóvel que ele está buscando, ajudar a saber se aquele imóvel está preço atrativo (abaixo da média para imóveis com as mesmas características) ou não.

### Descrição:
	No Airbnb, qualquer pessoa que tenha um imóvel de qualquer tipo (apartamento, casa, chalé, pousada, etc.)
	pode ofertar o seu imóvel para ser alugado por diária.
	Você cria seu perfil de host (pessoa que disponibiliza um imóvel para aluguel por diária) e cria o anúncio do seu imóvel.
	Nesse anúncio, o host deve descrever as características do imóvel da forma mais completa possível,
	de forma a ajudar os locadores/viajantes a escolherem o melhor imóvel para eles (e de forma a tornar o seu anúncio mais atrativo)
	Existem dezenas de personalização possíveis no seu anúncio, desde quantidade mínima de diária, preço, quantidade de quartes, até regras de cancelamento, taxa extra para hóspedes extras,
	exigência de verificação de identidade do locador, etc.

	Para o modelo de previsão analisaremos os dados ("dataset" disponíveis no drive), e para a previsão usaremos o Modelo ExtraTrees,
	Modelo com os melhores resultados de R² e RSME (R²: medida estatística que indica o quão bem um modelo de regressão linear se performa com os dados
	RSME: é uma medida para avaliar a precisão de modelos de regressão)


## Inspirações e Créditos:
	As bases de dados foram retiradas do site: [kaggle](https://www.kaggle.com/allanbruno/airbnb-rio-de-janeiro)
	Curso PythonImpressionador - Professor Jõao Paulo Lira
	https://www.hashtagtreinamentos.com/


## Requisitos:
### Bibliotecas Utilizadas:
	import pandas as pd
	import pathlib
	from google.colab import drive
	import numpy as np
	import seaborn as sns
	import matplotlib.pyplot as plt
	import plotly.express as px
	from sklearn.metrics import r2_score, mean_squared_error
	from sklearn.linear_model import LinearRegression
	from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor
	from sklearn.model_selection import train_test_split
	import joblib


## Pastas e Arquivos Utilizados no Projeto:
	dataset (Pasta com todos arquivos Excel com indicadores de cada ano e mês entre 2018-2020,
	Lembrando que essa pasta deve estar em seu Google Drive).
	Os arquivos que o Projeto criar ("dados.csv", "primeiros_registros", "modelo.joblib") devem ser inseridos no driver
	

### Att, Gabriel Souza