import requests
import matplotlib.pyplot as plt
import seaborn as sns
import datetime

# Set Seaborn style
sns.set(style="whitegrid")

# OpenWeatherMap API key and city
API_KEY = '1b81fec5d9e4f964c749a2709fded546'
CITY = 'Delhi'
URL = f'https://api.openweathermap.org/data/2.5/forecast?q={CITY}&appid={API_KEY}&units=metric'

# Fetch data
response = requests.get(URL)
data = response.json()

# Optional: Check if API call was successful
if response.status_code != 200:
    print("Error fetching data:", data.get("message", "Unknown error"))
else:
    # Extract relevant data
    dates = []
    temps = []
    humidity = []

    for forecast in data['list']:
        dt = datetime.datetime.fromtimestamp(forecast['dt'])
        dates.append(dt)
        temps.append(forecast['main']['temp'])
        humidity.append(forecast['main']['humidity'])

    # Plotting
    plt.figure(figsize=(12, 6))

    # Temperature plot
    plt.subplot(2, 1, 1)
    sns.lineplot(x=dates, y=temps, color='red')
    plt.title(f'Temperature Forecast for {CITY}')
    plt.ylabel('Temperature (°C)')
    plt.xticks(rotation=45)

    # Humidity plot
    plt.subplot(2, 1, 2)
    sns.lineplot(x=dates, y=humidity, color='blue')
    plt.title(f'Humidity Forecast for {CITY}')
    plt.ylabel('Humidity (%)')
    plt.xlabel('Date and Time')
    plt.xticks(rotation=45)

    plt.tight_layout()
    plt.show()
