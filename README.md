# Weather Dashboard

The Weather Dashboard is a responsive web application that provides real-time weather data for any location. It leverages the OpenWeatherMap API to display current weather conditions, a 5-day forecast, air quality index, and interactive weather maps. Additionally, users can save their favorite locations for quick access.

## Features

- **Real-Time Weather Updates**: Search for weather information in any city or by using your current location.
- **5-Day Forecast**: View a 5-day weather forecast, including temperature, humidity, wind speed, and precipitation.
- **Air Quality Index (AQI)**: See the current air quality index and pollution levels for a specific location.
- **Weather Maps**: Interactive maps with overlays for temperature, precipitation, and more.
- **Favorites**: Save your favorite cities for quick weather updates.
- **Location-based Weather**: Automatically fetches weather for the user's current location.
- **Responsive Design**: Optimized for mobile and desktop viewing.

## Tech Stack

- **Frontend**: React JS, CSS, and Bootstrap for UI and responsiveness.
- **API**:
  - [OpenWeatherMap API](https://openweathermap.org/api) for weather data, air quality index, and maps.
  - Browser's **Geolocation API** for detecting the user’s current location.

## API Integration

### OpenWeatherMap API Endpoints Used:

1. **Current Weather Data**: `GET https://api.openweathermap.org/data/2.5/weather`
   - Example: `https://api.openweathermap.org/data/2.5/weather?q={city name}&appid={API key}`
   
2. **5-Day Forecast**: `GET https://api.openweathermap.org/data/2.5/forecast`
   - Example: `https://api.openweathermap.org/data/2.5/forecast?q={city name}&appid={API key}`
   
3. **Air Pollution Data**: `GET https://api.openweathermap.org/data/2.5/air_pollution`
   - Example: `https://api.openweathermap.org/data/2.5/air_pollution?lat={latitude}&lon={longitude}&appid={API key}`
   
4. **Weather Maps**: `GET https://tile.openweathermap.org/map/{layer}/{z}/{x}/{y}.png`
   - Layers include: `temperature`, `precipitation`, `wind`, etc.

### Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/weather-dashboard.git
   cd weather-dashboard
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up your environment variables:
   - create a ```.env ``` file inthe project root and your OpenWeatherMap API key:
   ```bash
   REACT_APP_OPENWEATHER_API_KEY=your_openweathermap_api_key
   ```
4. Run the applicatio:
   ```bash
   npm start
   ```
   The application will be available at ```http:/localhost:3000```
### Usage
1. Search for Weather: Use the search bar to get weather information for any city.
2. Check Forecast: View the 5-day weather forecast.
3. Air Quality: Check the air quality index for the selected location.
4. Weather Maps: Toggle between weather overlays (temperature, wind, etc.) for the selected city.
5. Save Favorites: Add cities to your favorites and access them easily.
6. Get Current Location: Allow browser location access for instant weather details of your location.
### Dependencies
1. React - JavaScript library for building user interfaces.
2. Axios - For making HTTP requests to the OpenWeatherMap API.
3. Bootstrap - CSS framework for responsive design.
4. React Icons - For displaying icons throughout the app.
### Contributing
1. Fork the project.
2. Create your feature branch (git checkout -b feature/new-feature).
3. Commit your changes (git commit -m 'Add new feature').
4. Push to the branch (git push origin feature/new-feature).
5. Open a pull request.
### Licence
This project s licensed under the MIT License. See the (LICENSE)[] file for details.
