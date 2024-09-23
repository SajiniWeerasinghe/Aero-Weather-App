# Aero Weather App

Aero Weather App is a simple weather forecasting web application that allows users to search for the current weather conditions of any city in the world. The app fetches data from the OpenWeatherMap API and displays details such as temperature, humidity, wind speed, and weather conditions using visually appealing icons.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [How It Works](#how-it-works)
- [Screenshots](#screenshots)
- [API Reference](#api-reference)
- [License](#license)

## Features

- Users can search for the weather of any city.
- Displays temperature, humidity, and wind speed.
- Dynamically changes the weather icon based on current conditions (e.g., Clouds, Rain, Clear, etc.).
- Error handling for invalid city names.

## Installation

### Prerequisites

- A text editor like Visual Studio Code
- A modern web browser (Chrome, Firefox, etc.)
- Node.js (optional if you want to use a server)
- Internet connection (for fetching the weather data)

### Steps to Run Locally

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/aero-weather-app.git
    ```

2. Navigate to the project folder:
    ```bash
    cd aero-weather-app
    ```

3. Open the `index.html` file in your browser, or run a local server to serve the app:
    ```bash
    open index.html
    ```

4. Start searching for the weather of any city!

## Technologies Used

- **HTML5**: For creating the structure of the web page.
- **CSS3**: For styling the app and creating the layout.
- **JavaScript (ES6)**: For adding interactivity and making API calls.
- **OpenWeatherMap API**: For fetching real-time weather data.

## How It Works

- The user enters the city name in the search bar.
- The app makes an asynchronous API request to the [OpenWeatherMap API](https://openweathermap.org/current) using JavaScript's `fetch` function.
- If the city is found, the app displays the current weather data (temperature, humidity, wind speed) and updates the weather icon based on the data received.
- If the city is not found (invalid city name), an error message is displayed.

### Code Explanation

- **HTML**: Structure of the app, including the search bar, error messages, and weather display card.
- **CSS**: Styles for making the UI visually appealing, such as gradient text, icons, and responsive layout.
- **JavaScript**: Handles the weather API calls and updates the DOM with the fetched data.

## Screenshots

![Screenshot of Aero Weather App](images\Screenshot 1.png)(images\Screenshot 2.png)

## API Reference

- **Base URL**: `https://api.openweathermap.org/data/2.5/weather`
- **API Key**: You can obtain your API key from [OpenWeatherMap](https://home.openweathermap.org/users/sign_up).
- **Parameters**:
  - `q` (City Name): The name of the city to search for.
  - `units`: Set to `metric` for Celsius temperature.
  - `appid`: Your unique API key.

Example API call:
