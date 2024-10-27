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

