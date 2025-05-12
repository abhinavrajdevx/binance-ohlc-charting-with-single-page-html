# 📊 Binance OHLC Candlestick Charting Tool

[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit-brightgreen?style=for-the-badge)](https://abhinavrajdevx.github.io/binance-ohlc-charting-with-single-page-html/)
<!-- ^^^ IMPORTANT: Make sure GitHub Pages is enabled for your 'main' or 'master' branch
     and this link points to it. Usually it's https://<your-username>.github.io/<repository-name>/ -->

A sleek, single-page HTML, CSS, and JavaScript application that fetches and displays OHLC (Open, High, Low, Close) candlestick charts using Binance's free public APIs. Visualize cryptocurrency price action over the last 7 days with various timeframes and trading pairs.

![Screenshot Placeholder - Replace with an actual screenshot or GIF of your application in action!]
*(Suggestion: Take a screenshot of the app, perhaps in dark mode, showing a chart, and upload it to your repo, then update the link above)*
*Example: `![App Screenshot](./images/app_screenshot.png)` if you create an `images` folder.*

## ✨ Features

*   **Real-time Data:** Fetches the latest candlestick data directly from the Binance API.
*   **Dynamic Pair Selection:** Choose from a curated list of popular trading pairs (e.g., BTC/USDT, ETH/USDT).
*   **Selectable Timeframes:** View charts for various intervals (1m, 5m, 15m, 30m, 1h, 4h, 1d).
*   **7-Day Data History:** Displays OHLC data for the past 7 days.
*   **Interactive Candlestick Charts:** Powered by [ApexCharts](https://apexcharts.com/) for a rich, interactive experience (zoom, pan, tooltips).
*   **Light & Dark Mode:** Switch between light and dark themes for comfortable viewing.
*   **Responsive Design:** Adapts to different screen sizes for a good user experience on desktop and mobile.
*   **Single-Page Application:** All HTML, CSS, and JavaScript are contained within a single `index.html` file for simplicity and easy deployment.
*   **Professional UI:** Clean and modern user interface.
*   **No API Keys Required:** Uses Binance's public, unauthenticated endpoints.

## 🚀 Live Demo

Experience the charting tool live:
**[https://abhinavrajdevx.github.io/binance-ohlc-charting-with-single-page-html/](https://abhinavrajdevx.github.io/binance-ohlc-charting-with-single-page-html/)**

*(Ensure this link is correct and your GitHub Pages site is active.)*

## 🛠️ Technologies Used

*   **HTML5:** For the basic structure of the page.
*   **CSS3:** For styling, including dark/light themes and responsive design.
*   **JavaScript (ES6+):** For fetching data, DOM manipulation, and chart logic.
*   **[ApexCharts.js](https://apexcharts.com/):** A modern JavaScript charting library for rendering interactive candlestick charts.
*   **[Binance Public API (`/api/v3/klines`)](https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#klinecandlestick-data):** For fetching OHLCV data.

## ⚙️ How to Use

There are two main ways to use this application:

1.  **Via the Live Demo (Recommended):**
    Simply click on the [Live Demo link](https://abhinavrajdevx.github.io/binance-ohlc-charting-with-single-page-html/) above to open it directly in your browser.

2.  **Running Locally:**
    *   Clone the repository:
        ```bash
        git clone https://github.com/abhinavrajdevx/binance-ohlc-charting-with-single-page-html.git
        ```
    *   Navigate to the project directory:
        ```bash
        cd binance-ohlc-charting-with-single-page-html
        ```
    *   Open the `index.html` file in your favorite web browser. No web server is strictly necessary for this single-file application.

Once loaded:
1.  Select your desired **Trading Pair** from the dropdown.
2.  Choose your preferred **Timeframe**.
3.  Click the **"Fetch & Draw Chart"** button.
4.  Toggle the **Light/Dark mode** switch in the header to change themes.
5.  Interact with the chart (zoom, pan, hover for details).

## 🔧 Code Highlights

*   **`fetchCandlestickData(symbol, interval)`:** Asynchronously fetches kline data from the Binance API. It handles pagination (Binance API limit per request) by making multiple requests if needed to gather the full 7 days of data for the selected timeframe.
*   **`transformDataForChart(klines)`:** Processes the raw API response into the format required by ApexCharts.
*   **`renderChart(seriesData, symbol, interval)`:** Initializes and renders the ApexCharts candlestick chart with appropriate configurations, including theme settings.
*   **Theme Management:** JavaScript functions `applyTheme` and `toggleTheme` handle switching between light and dark modes, updating CSS variables and ApexCharts options accordingly. Theme preference is saved in `localStorage`.

## 💡 Potential Future Enhancements

*   Allow users to specify a custom date range.
*   Add more technical indicators (e.g., Moving Averages, RSI, MACD).
*   Implement drawing tools on the chart.
*   Allow users to save their favorite pairs/timeframes.
*   Auto-refresh chart data.
*   More comprehensive error handling and user feedback.
*   Option to download chart data or image.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/abhinavrajdevx/binance-ohlc-charting-with-single-page-html/issues).

1.  Fork the Project.
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 📜 License

Distributed under the MIT License. See `LICENSE` file for more information (though you haven't added one yet, MIT is a good default for open-source projects like this. If you wish to add one, create a `LICENSE` file with the MIT license text).

---

Made with ❤️ by [Abhinav Raj](https://github.com/abhinavrajdevx)

Give a ⭐️ if you find this project useful!
