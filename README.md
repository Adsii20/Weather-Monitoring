# Weather-Monitoring
This project is a weather monitoring application that fetches real-time weather data from the OpenWeatherMap API, stores it in a SQLite database, and visualizes daily weather summaries. Additionally, it includes alerting mechanisms for temperature thresholds and calculates daily summaries for predefined cities in India.
# Table of Contents
- Project Overview
- Features
- Installation
- Usage
- Configuration
- Functions Overview
- Dependencies
- License
# Project Overview
This application retrieves and processes weather data from the OpenWeatherMap API for specific cities in India (Delhi, Mumbai, Bangalore, Kolkata, and Hyderabad). It stores daily weather data and provides visualizations of temperature trends. The application is designed to run continuously, checking for new data and updating the database hourly.
# Features
- Fetch Real-Time Weather Data: Retrieves temperature and weather conditions for multiple cities.
- Database Storage: Stores daily weather summaries in an SQLite database.
- Temperature Threshold Alerts: Prints alerts if the temperature exceeds a predefined threshold.
- Data Visualization: Visualizes average temperature trends using Matplotlib.
- Hourly Data Collection: Runs hourly to refresh data and store updated records.
# Installation
1. Clone the repository:
```
git clone <https://github.com/Adsii20/Weather-Monitoring>
cd weather monitoring
```
2. Install required dependeries
```
pip install requests sqlite3 matplotlib
```
3. Setup OpenWeatherMap API Key: Replace API_KEY in the script with your actual OpenWeatherMap API key.
# Usage
Run the main script to start the application:
```
python weather_monitoring.py
```
The application will automatically fetch data for the configured cities, save summaries in a SQLite database (weather_data.db), and print temperature alerts if conditions exceed specified thresholds.
To visualize the collected data:
```
visualize_weather_data()
```
# Configuration
- API Key: Replace API_KEY in the script with your OpenWeatherMap API key.
- City IDs: Predefined city IDs are provided for specific cities in India. Update CITY_IDS dictionary to monitor other cities if desired.
- Temperature Threshold: Modify TEMP_THRESHOLD in the script to adjust the temperature alert level (default is set to 15°C).
# Functions Overview
- get_weather_data(city_id): Fetches weather data from OpenWeatherMap API for a specified city.
- calculate_daily_summary(weather_data): Computes the average, maximum, and minimum temperatures for the day, along with the dominant weather condition.
- store_daily_summary(daily_summary): Saves the daily summary into the SQLite database.
- check_alerting_thresholds(weather_data): Checks if the temperature exceeds a predefined threshold and triggers an alert.
- visualize_weather_data(): Plots the temperature trends from the database.
# Dependencies
- requests - For API requests to OpenWeatherMap.
- sqlite3 - For database operations.
- matplotlib - For data visualization.
- datetime - For handling dates

