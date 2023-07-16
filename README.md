# future_prediction_facebook_prophet

steps to use Prophet and output them in markdown:

Import the necessary libraries and modules:
# Python
import pandas as pd
from prophet import Prophet
Read the data into a pandas DataFrame:
# Python
df = pd.read_csv('example.csv')
Instantiate a Prophet object:
# Python
m = Prophet()
Fit the model with the historical data:
# Python
m.fit(df)
Create a future DataFrame for making predictions:
# Python
future = m.make_future_dataframe(periods=365)
Make predictions using the Prophet model:
# Python
forecast = m.predict(future)
Plot the forecast:
# Python
fig1 = m.plot(forecast)
Plot the forecast components:
# Python
fig2 = m.plot_components(forecast)
Find more details and options in the Prophet documentation.
