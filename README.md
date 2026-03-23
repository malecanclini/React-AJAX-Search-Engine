# 🌤️ ATMOS — Weather Search Engine

A clean, responsive weather search engine that fetches real-time data from the OpenWeatherMap API using **Axios** and displays the current temperature and atmospheric conditions for any city in the world.

---

## 🚀 Demo

> Search any city → get live temperature, humidity, wind speed, pressure, and more.

![preview](https://via.placeholder.com/800x400?text=Weather+Search+Engine+Preview)

---

## ✨ Features

- 🔍 Search weather by city name
- 🌡️ Displays current temperature in °C
- 💧 Humidity, wind speed & direction
- 🌅 Sunrise and sunset times
- 📉 Daily min / max temperature range
- ☁️ Cloud cover, visibility, and atmospheric pressure
- ⚡ Fast HTTP requests with **Axios**
- ❌ Graceful error handling (city not found, invalid API key)

---

## 🛠️ Technologies

| Technology | Purpose |
|---|---|
| HTML5 / CSS3 | Structure and styling |
| JavaScript (ES6+) | Logic and DOM manipulation |
| [Axios](https://axios-http.com/) | HTTP requests |
| [OpenWeatherMap API](https://openweathermap.org/api) | Weather data source |

---

## 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/your-username/weather-search-engine.git
cd weather-search-engine
```

2. **Get a free API Key**

   Go to [openweathermap.org](https://openweathermap.org/api), create a free account, and copy your API key.

3. **Add your API Key**

   Open `index.html` and replace the placeholder:

```javascript
const API_KEY = 'YOUR_API_KEY_HERE'; // 👈 paste your key here
```

4. **Open in browser**

```bash
# No build step needed — just open the file
open index.html
```

---

## 🔌 API Usage

This project uses the **OpenWeatherMap Current Weather API**:

```
GET https://api.openweathermap.org/data/2.5/weather?q={city}&appid={API_KEY}&units=metric
```

The Axios request looks like this:

```javascript
const response = await axios.get(url);
const temperature = response.data.main.temp; // temperature in °C
```

---

## 📁 Project Structure

```
weather-search-engine/
├── index.html       # Main app (HTML + CSS + JS in one file)
└── README.md        # You are here
```

---

## ⚠️ Notes

- The free tier of OpenWeatherMap allows **60 calls/minute**.
- API keys can take up to **10 minutes** to activate after registration.
- Make sure your key is from the **Current Weather Data** plan.

---

## 📄 License

MIT © [Your Name](https://github.com/your-username)
