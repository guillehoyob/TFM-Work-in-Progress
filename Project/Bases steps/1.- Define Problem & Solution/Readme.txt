ChatGPT
	Define Problem and how to solve it
	State of Art


TITULO TFM: ------------

El problema al que nos enfrentamos es al predecir el comportamiento futuro de un usuario en una plataforma según su antiguo comportamiento.
En el caso de este TFM, el problema va a ser mediante una plataforma de streamings (Spotify), y las reproducciones del usuario desde su suscripción.
Es decir, este problema puede extenderse a otros hábitos que sean del tipo: Empresa/Tienda/Negocio -- Productos/Servicios que ofrece -- Consumo del usuario.

Para resolver este problema necesitamos:
	- Recolectar los datos del usuario
		- Entender estos datos
		- Limpair o tratar elementos Outlayer o Anomalies
		- WebScraping para obtener mas datos

	- Preprocesado & Limpieza
		- Limpiar Elementos Nan
		- Transformar o Genrar Nuevos (Feature Engineering) -- All apply functions - TimeDelta - Daily/Hourly dataset 
		- Treat Error Data (TimeDelta) - Generar Prueba de Spotify para 
		
	- Exploratoy Data Analysis (EDA)
		- Create Visualization
		- Summaries

	- Time Serie Analysis
		- Plot Series
		- Plot ACF & PACF for each T.S. (What about Only same day??)
		- Is Stationary? 
			- Plot Rolling mean for Stationarity
			- Making DICKEY & KPSS Tests
			- Recursive process to Transform

		- Conclusion about Stationarity, Trends and Seasonability

		- What about User Parameters as Churn-Rate

	- Data Modeling & Analysis + Model Evaluation + Prediction
		- Prepare Models 4 Prediction:
			- Select Evaluation Method

			- Baseline Model (lag-1): Predic using last value
				- If any MAE/MSE < 1 -- Remove that data serie
			
			- Random Forest Regressor / Classifier:
				- Variables Importance different Lags
				- Variables Importance different Time Features
				- Variables Importances different Cyclical Time Features

				- Simulate with list of lags dataset -> Find Best Lag
				- Simulate with list of different t.f-> Finde Best TF
				- Simulate with cyclical time feature-> Finde Best CY

				- Comapre Results - Get best Model

				- Use 2 Cross Validation methods:
					- tscv 
					- bcv
						
					- Compare Result of results, wich is the best & how it differs from original prediction

				- Use Grid Search 4 hyperparameter tunning

			- Arima
				- AUTOARIMA FOR REGRESSIN --- Need to be implemented


	- Conclusion:
		- Which are the best features for each model?
			- For RF & For ARIMA

		- Wich is the best CV Methods
			- For RF & For ARIMA

		- Which is the best model? -- RF VS ARIMA
			- Results
			- Training Time
			- Hyperparameter Tunning
			- Difficoulties

		
	
	- What About Classification Embedings...
		
