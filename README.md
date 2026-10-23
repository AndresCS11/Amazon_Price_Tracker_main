# 🛒 Amazon Price Tracker

A Python web scraper that monitors the price of selected Amazon products and alerts you when the price drops below your target. Built with **Requests** and **BeautifulSoup4** as a hands-on web scraping exercise.

## ✨ Features

- Scrapes the current price and product title from any Amazon product URL
- Compares the live price against a target price you define
- Sends an email alert when the price falls below your target
- Easy to configure for multiple products
- Lightweight: no browser automation required

## 🛠️ Tech Stack

- **Python 3.x**
- **Requests**: fetches the product page HTML
- **BeautifulSoup4**: parses the HTML and extracts price data
- **smtplib**: sends email notifications

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/amazon-price-tracker.git
   cd amazon-price-tracker
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## ⚙️ Configuration

Set your product URL, target price, and email credentials (preferably as environment variables):

```python
PRODUCT_URL = "https://www.amazon.com/dp/XXXXXXXXXX"
TARGET_PRICE = 99.99
```

## ▶️ Usage

```bash
python main.py
```

To track prices automatically, schedule the script with **cron** (macOS/Linux), **Task Scheduler** (Windows), or a cloud service like PythonAnywhere.

## ⚠️ Disclaimer

This project is for educational purposes only. Amazon's page structure changes frequently and the site may block automated requests, so selectors and headers may need updating. Please respect Amazon's Terms of Service.

## 📚 What I Learned

- Sending HTTP requests with custom headers
- Parsing and navigating HTML with BeautifulSoup
- Cleaning and converting scraped text into numeric data
- Automating notifications with Python

## 📄 License

MIT License
