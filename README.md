📰 Daily Digest Email (Python Automation)

📖 Overview

This project is a Python automation script that generates and sends a **daily email digest** containing useful information such as news headlines, weather updates, and personalized content. It fetches data using APIs and delivers it via SMTP to your inbox every morning.

⚙️ Features

* Fetches **top news headlines** from public APIs
* Provides **daily weather forecasts** for your city
* Includes **custom sections** (quotes, reminders, etc.)
* Automatically **sends the compiled digest via email**
* Supports **scheduling with `cron` or Windows Task Scheduler**

🧩 Tech Stack

* **Language:** Python 3
* **Libraries:** `requests`, `smtplib`, `email`, `datetime`, `schedule` (optional)
* **APIs Used:** (e.g., NewsAPI, OpenWeatherMap)
  
🚀 How It Works

1. The script collects data from selected APIs.
2. It composes an HTML/plain text email summarizing the day’s content.
3. It sends the email using your SMTP credentials (e.g., Gmail SMTP).
4. Optionally, it can be scheduled to run automatically every day.

 🧠 Example Email

```
Subject: Your Daily Digest - October 19, 2025

Good Morning!
Here’s your daily summary:

🌤 Weather: 29°C, partly cloudy
📰 Top News: "AI breakthrough in healthcare automation"
💡 Quote: "Success is nothing more than a few simple disciplines, practiced every day."
```

🪜 Setup Instructions

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/daily-digest-email.git
   cd daily-digest-email
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Add your credentials and API keys in `config.py`:

   ```python
   EMAIL_USER = "your_email@gmail.com"
   EMAIL_PASS = "your_app_password"
   NEWS_API_KEY = "your_news_api_key"
   WEATHER_API_KEY = "your_weather_api_key"
   ```
4. Run the script:

   ```bash
   python main.py
   ```

🕒 Automation (Optional)

To send the digest automatically every day:

* **Windows:** Use Task Scheduler
* **Linux/Mac:** Add a cron job like

  ```bash
  0 8 * * * /usr/bin/python3 /path/to/main.py
  ```
  
📧 Example Use Cases

* Morning digest emails for yourself
* Automated team updates
* Personalized daily newsletters

🧑‍💻 Author

Koushik Bhowmick
📧 koushikbhowmick04@gmail.com
🌐 https://dev-koushik.vercel.app/

