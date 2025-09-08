# weather-dashboard-Power-BI
Real-time weather and air quality dashboard built in Power BI using live API data for multiple cities with dynamic visualizations and automated refresh workflows.

# Real-Time Weather Dashboard in Power BI 🌦️📊

This repository showcases a **real-time weather and air quality dashboard** built with **Power BI**. It integrates live weather data from APIs and presents key metrics such as temperature, humidity, wind speed, air quality index (AQI), sunrise/sunset times, and more. The dashboard is interactive, dynamic, and designed with user experience in mind.

It covers data from the following cities:
✅ Ranchi  
✅ New Delhi  
✅ Noida  
✅ Ajmer  
✅ Hyderabad  
✅ Lucknow

---

## 🚀 Features
- 🌐 Live weather data pulled via APIs  
- ⏱️ Scheduled refresh in Power BI Service  
- 🔄 Dynamic selection of cities and metrics  
- 🎨 Custom UI with dark themes, Figma-designed backgrounds, and clear icons  
- 📊 Trend lines, KPIs, and data labels for quick insights  
- 📈 Scalable design with advanced DAX formulas

---

## 📂 Project Files
- **Weather Dashboard.pbix** – The Power BI report file  
- **Data/sample-weather-data.csv** – Mock data for local testing (optional)  
- **API Setup Guide.md** – Instructions for connecting APIs and setting up authentication  
- **README.md** – Documentation and overview  
- **.gitignore** – To exclude unnecessary files when uploading  

---

## 🛠 Technologies Used
- Power BI Desktop  
- Power BI Service (for scheduled refresh)  
- REST APIs (weather and air quality data providers)  
- DAX for calculations  
- Figma for custom visuals and design assets  

---

## 📖 Key Learnings
✔ Integrating APIs and handling authentication  
✔ Creating dynamic measures and calculations in DAX  
✔ Designing intuitive dashboards with conditional formatting  
✔ Automating data refresh workflows for real-time reporting  
✔ Implementing user-friendly navigation and responsive visuals  

---

# API Setup Guide – Real-Time Weather Dashboard

This guide helps you configure the API connection in Power BI to fetch live weather and air quality data.

## ✅ Step 1 – Choose a Weather API Provider
You can use providers like:
- OpenWeatherMap (https://openweathermap.org/api)
- WeatherAPI (https://www.weatherapi.com/)
- AccuWeather API

Sign up and generate an API key.

## ✅ Step 2 – Create API Query in Power BI
1. Go to **Home → Get Data → Web**.
2. Enter the API URL with your API key:

https://api.openweathermap.org/data/2.5/weather?q=Noida&appid=YOUR_API_KEY

3. Click **OK** and transform the JSON data into a table.

4. Repeat this for other cities or create parameters to dynamically switch between cities.

---

## ✅ Step 3 – Authentication
- If the API requires authentication via headers or parameters, configure it in the query editor.
- Example:  
- URL: `https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY&q=Noida&aqi=yes`

---

## ✅ Step 4 – Schedule Refresh
1. Publish the report to Power BI Service.
2. Go to **Datasets → Settings → Scheduled refresh**.
3. Enter your API credentials and set refresh intervals.

---

## ✅ Step 5 – Testing
- Validate that data updates when switching cities.
- Check that values like temperature, humidity, and AQI are loaded and formatted correctly.

---

## 📌 Notes
- Keep your API key private and do not upload it to GitHub.
- Use Power BI parameters to handle API keys securely.


