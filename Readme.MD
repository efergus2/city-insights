# City Insights Web App **WIP**

A simple, clean web app to get insights about any city using free APIs. Shows **weather, climate, currency, average salary, cost of living, and number of grocery stores**.

## 🌐 Live Demo

[City Insights](https://efergus2.github.io/city-insights/)

## Features

* Weather and feels-like temperature (°C / °F toggle)
* Dark mode (toggle, dark by default)
* Currency information
* Estimated monthly salary (from World Bank GNI per capita)
* Estimated cost of living (based on salary)
* Count of grocery stores (from OpenStreetMap Overpass API)
* Responsive and polished UI with Tailwind CSS

## 📦 Technologies Used

* HTML / CSS / JavaScript
* Tailwind CSS for styling
* Free APIs:

  * [OpenWeatherMap](https://openweathermap.org/api) for weather
  * [RestCountries](https://restcountries.com/) for currency
  * [World Bank API](https://data.worldbank.org/) for salary / GNI
  * [OpenStreetMap Overpass API](https://overpass-api.de/) for grocery stores

## ⚙️ Setup

1. **Clone the repo:**

```bash
git clone https://github.com/efergus2/city-insights.git
cd city-insights
```

2. **Add your OpenWeatherMap API key as a GitHub secret:**

* Go to **Settings → Secrets and variables → Actions → New repository secret**
* Name it `OPENWEATHER_API_KEY`
* Paste your API key and save

3. **Update workflow** (already included) to inject the API key into `config.js` automatically.

4. **Deploy:**

* The GitHub Actions workflow automatically deploys to GitHub Pages on each push to `main`

## 🔄 Usage

* Open the site in a browser.
* Enter a city name in the search box.
* Toggle dark mode using the 🌙 button.
* Toggle temperature units (°C / °F) using the button.
* See live weather, currency, estimated salary, cost of living, and number of grocery stores.

## 📂 File Structure

```
city-insights/
├─ index.html
├─ app.js       # main JavaScript
├─ config.js    # injected via GitHub Actions with API key
├─ README.md
```

## 👨‍💻 Contributing

* Feel free to fork and submit pull requests.
* Ensure all API usage remains free.

## 📜 License

MIT License
