# WeatherPro - Modern Weather Dashboard

![WeatherPro Screenshot](https://via.placeholder.com/800x450.png?text=Add+a+Screenshot+of+WeatherPro+Here)
*(Suggestion: Replace the placeholder above with a screenshot or a GIF of your application in action)*

A sleek, modern, and responsive weather dashboard built with vanilla HTML, CSS, and JavaScript. This project showcases a beautiful "glassmorphism" UI, dynamic backgrounds that change with the weather, smooth animations, and interactive elements.

**Note:** This project is a front-end demonstration and uses simulated API calls with demo data. It is designed to showcase UI/UX and front-end skills and can be easily hooked up to any real weather API.

---

## ✨ Features

* **City-Based Search**: Get the weather forecast for any city in the world.
* **Geolocation**: Instantly fetch weather data for your current location with a single click.
* **Detailed Current Weather**: Displays temperature, "feels like" temperature, humidity, wind speed, pressure, visibility, and UV index.
* **5-Day Forecast**: View a summarized weather forecast for the next five days.
* **Unit Toggling**: Seamlessly switch between Celsius (°C) and Fahrenheit (°F).
* **Dynamic Backgrounds**: The background gradient and theme change based on the current weather conditions (e.g., sunny, rainy, cloudy).
* **Responsive Design**: A mobile-first design that looks great on all devices, from phones to desktops.
* **Interactive UI**:
    * Smooth CSS transitions and hover effects.
    * An animated, bouncing weather icon.
    * A floating particle effect that reacts to mouse movement.
* **User Feedback**: Clear loading and error states to inform the user of the application's status.

---

## 🛠️ Tech Stack

* **HTML5**: For the structure and content of the application.
* **CSS3**: For styling, layout, animations, and responsive design.
    * **Flexbox & Grid**: Used for modern, flexible layouts.
    * **Glassmorphism Effect**: Achieved using `backdrop-filter: blur()`.
    * **Keyframe Animations**: For the loading spinner, bouncing icon, and particle effects.
* **Vanilla JavaScript (ES6+)**: For all the application logic, DOM manipulation, and event handling.
    * **Object-Oriented**: Logic is organized into a `WeatherApp` class.
    * **Async/Await**: Used for handling asynchronous operations like fetching data (simulated).

---

## 🚀 Getting Started

This is a pure front-end project and requires no special installation or build steps.

### Prerequisites

You only need a modern web browser that supports HTML5, CSS3, and ES6 JavaScript.

### Installation

1.  Clone the repository to your local machine:
    ```sh
    git clone [https://github.com/Muneeb80806/Weather-App.git]
    ```
2.  Navigate to the project directory:
    ```sh
    cd Weather-App
    ```
3.  Open the `index.html` file directly in your web browser.

That's it! The application will load with a default city (London) and is ready to use.

---

## 🔧 How to Use

* **Search for a City**: Type a city name into the search bar and press `Enter` or click the search icon (🔍).
* **Use Your Location**: Click the location pin icon (📍) to allow the browser to use your current location for the weather forecast.
* **Change Units**: Click the `°F` / `°C` button at the top right corner to toggle between Fahrenheit and Celsius.

---

## 🔌 Connecting to a Real API

This demo uses a `simulateAPICall()` function to return placeholder data. To connect it to a real weather service like [OpenWeatherMap](https://openweathermap.org/api), you would need to:

1.  **Get an API Key**: Sign up for a free API key from a weather data provider.
2.  **Modify the JavaScript**:
    * Replace `this.apiKey = 'demo_key';` with your actual API key.
    * Comment out or remove the `simulateAPICall()` and `displayDemoWeather()` methods.
    * Implement real `fetch()` calls inside `getWeatherByCity()` and `getWeatherByCoords()` to request data from the API endpoints.
    * Update the `updateWeatherDisplay()` function to parse the actual API response and display the data.

---

## 📝 Future Improvements

* Integrate a real weather API (e.g., OpenWeatherMap, WeatherAPI).
* Add search-as-you-type autocomplete for city names.
* Use `localStorage` to remember the user's last searched city and preferred temperature unit.
* Add more detailed hourly forecasts.
* Refactor CSS to use a preprocessor like SASS/SCSS for better organization.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
