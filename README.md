# 🌦️ Weather Forecast Application

A simple Spring Boot application that fetches real-time weather data using a REST API and displays it based on city input.

---

## 🚀 Features

* 🌡️ Get current temperature
* 💧 Get humidity data
* 📍 Search weather by city name
* 🔗 REST API integration with OpenWeatherMap
* 📦 JSON response handling

---

## 🛠️ Technologies Used

* Java
* Spring Boot
* REST API (OpenWeatherMap)
* JSON
* Maven

---

## 📁 Project Structure

```
com.example.demo
│
├── Controller
│   └── WeatherController.java
│
├── Service
│   └── WeatherService.java
│
└── WeatherForecastApplication.java
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/your-username/weather-forecast-app.git
cd weather-forecast-app
```

### 2. Configure API Key

Create or update `application.properties`:

```
weather.api.key=YOUR_API_KEY
weather.api.url=https://api.openweathermap.org/data/2.5/forecast
```

👉 Get your API key from: https://openweathermap.org/

---

### 3. Run the Application

Using Maven:

```
mvn spring-boot:run
```

Or run the main class:

```
WeatherForecastApplication.java
```

---

## 🌐 API Endpoint

### Get Weather by City

```
GET /api/weather/{city}
```

### Example:

```
http://localhost:8080/api/weather/Pune
```

---

## 📄 Sample Response

```
{
  "list": [
    {
      "main": {
        "temp": 30,
        "humidity": 60
      }
    }
  ]
}
```

---

## ⚠️ Common Issues

### ❌ 401 Unauthorized (Invalid API Key)

* Ensure API key is correct
* Wait a few minutes after generating the key
* Remove extra spaces or quotes in properties file

---

## 🔮 Future Improvements

* ✅ Convert JSON to structured Java objects
* 📅 Add 5-day forecast filtering
* 🎨 Build frontend UI (React / Thymeleaf)
* ☁️ Deploy to cloud (AWS / Render)
* ⚡ Add caching for API responses

---

## 👨‍💻 Author

Dhananjay Kadale

---

## 📜 License

This project is open-source and available under the MIT License.
