
# React Weather Application Project

## Project Title
Modern Weather Forecast Web App

---

# Project Objective

The goal of this project is to build a **modern Weather Forecast Web Application** using:

- React.js
- Tailwind CSS
- Public Weather API

The application will allow users to **search for any city and view detailed weather information on a separate page with a modern UI design.**

This project will help students understand:

- React component structure
- API integration
- Routing between pages
- State management
- Responsive UI with Tailwind CSS
- Error handling and loading states

---

# Application Flow

1. User opens the **Home Page**
2. User enters a **City Name**
3. User clicks **Search**
4. App fetches weather data from API
5. App redirects to **Weather Details Page**
6. Weather information is displayed with modern UI

---

# Technologies Required

- React.js
- JavaScript (ES6+)
- Tailwind CSS
- React Router
- Public Weather API

Recommended API:

OpenWeatherMap API

https://openweathermap.org/api

---

# Features

## 1 Home Page (City Search)

The landing page should contain:

- App title
- City search input
- Search button
- Clean modern design

### UI Layout Example

Weather App

[ Enter City Name ]   [ Search ]

Example input:

Delhi  
London  
Tokyo

When the user clicks **Search**, redirect to the Weather Details page.

---

# 2 Weather Details Page

After searching, the application should display:

- City Name
- Temperature
- Weather Condition
- Weather Icon
- Feels Like Temperature
- Humidity
- Wind Speed
- Pressure
- Visibility

Example Output:

City: Delhi  
Temperature: 30°C  
Condition: Clear Sky  
Feels Like: 32°C  
Humidity: 45%  
Wind Speed: 12 km/h  
Pressure: 1012 hPa

---

# 3 Modern UI Design

The UI should look modern and clean.

Recommended UI features:

- Gradient background
- Glassmorphism card design
- Large weather icon
- Responsive layout
- Smooth hover effects

Example Layout:

-------------------------------------------------

            Weather Forecast

         [ Enter City Name ]
              [ Search ]

-------------------------------------------------

Weather Details Card

City: Delhi  
Temperature: 30°C  
Condition: Clear Sky  

Humidity: 45%  
Wind: 12 km/h  
Pressure: 1012 hPa

-------------------------------------------------

---

# 4 Loading State

When the API request is running, display:

Loading weather data...

---

# 5 Error Handling

If the user enters an invalid city name, show:

City not found  
Please enter a valid city name

---

# Project Setup

## Step 1 Create React App

npx create-react-app weather-app
cd weather-app

---

# Step 2 Install Tailwind CSS

npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

Update tailwind.config.js

content: [
"./src/**/*.{js,jsx,ts,tsx}"
]

Add Tailwind to index.css

@tailwind base;
@tailwind components;
@tailwind utilities;

---

# Step 3 Install React Router

npm install react-router-dom

---

# Suggested Folder Structure

weather-app

public/

src/

components/
SearchBox.js
WeatherCard.js

pages/
Home.js
WeatherDetails.js

App.js
index.js
index.css

---

# Example API Request

https://api.openweathermap.org/data/2.5/weather?q=Delhi&appid=YOUR_API_KEY&units=metric

---

# Expected Components

## SearchBox Component

Handles:

- User input
- Search button
- API call

---

## WeatherCard Component

Displays:

- Weather icon
- Temperature
- City name
- Weather description

---

# Pages

## Home Page

Contains:

- Title
- Search box
- Navigation to weather page

---

## Weather Details Page

Displays full weather information.

---

# Bonus Features (Optional)

Students can add:

- 5 Day Forecast
- Dark Mode
- Current Location Weather
- Weather Animations
- Search History
- Background change based on weather

---
