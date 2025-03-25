# CLA-2

# Weather App

## Overview
This Weather App is a simple web-based application that provides current weather conditions and a 5-day forecast for a specified city. It fetches real-time weather data using the OpenWeatherMap API and updates the UI dynamically based on the fetched information.

## Features
- Fetches real-time weather data based on user input
- Displays the current temperature and weather description
- Provides a 5-day weather forecast
- Dynamically updates the background based on weather conditions
- Responsive and user-friendly interface

## Technologies Used
- **HTML**: Structure of the application
- **CSS**: Styling and layout
- **JavaScript**: Logic and API calls
- **OpenWeatherMap API**: Fetching weather data

## How It Works
1. The user enters a city name in the input field and clicks the "Get Weather" button.
2. The JavaScript function `getWeather()` is triggered.
3. The function makes asynchronous API calls to OpenWeatherMap:
   - `https://api.openweathermap.org/data/2.5/weather` (for current weather)
   - `https://api.openweathermap.org/data/2.5/forecast` (for the 5-day forecast)
4. The responses are processed:
   - The current weather temperature and description are displayed.
   - A 5-day forecast is generated and displayed.
5. The `changeBackground()` function updates the background image based on the weather condition.

## Code Breakdown
### HTML Structure
- A text input field for entering the city name.
- A button to trigger the weather search.
- A container to display current weather details.
- A separate container for the 5-day forecast.

### CSS Styling
- A gradient background for a visually appealing design.
- Containers styled with a blurred background effect.
- Buttons styled with hover effects.

### JavaScript Implementation
#### `getWeather()` Function
- Reads user input (city name).
- Constructs API URLs and makes `fetch` requests.
- Updates the UI with weather data if the request is successful.
- Displays an error message if the city is not found or data fetch fails.

#### `changeBackground(weatherCondition)` Function
- Maps weather conditions to background images.
- Updates the background dynamically using `style.background`.

## API Key Configuration
- The API key (`apiKey = '297fb03bf4dab10e0d8c969ec45a128c'`) is required for fetching weather data.
- Users should replace this with their own API key from OpenWeatherMap.

## Installation & Usage
1. Download the project files.
2. Open the `index.html` file in a web browser.
3. Enter a city name and click "Get Weather" to see the results.
