# 📈 Stock‑News SMS Alert

A lightweight Python script that monitors selected stock tickers, checks for significant daily price moves, collects the latest news headlines, and sends a concise SMS digest via **Twilio**.  
Ideal for getting a quick market pulse straight to your phone.

---

## Features
* **Price‑Move Detection** – fetches previous‑close vs. current price and flags notable percentage moves  
* **Headline Summaries** – pulls the top 3 news headlines for each triggered ticker  
* **SMS Delivery** – sends a single text containing price move and headline snippets  
* **Secure Credentials** – all API keys and tokens are stored in environment variables (no hard‑coding)

---

## Tech Stack
| Purpose | Library / API |
|---------|---------------|
| Stock & News data | *Alpha Vantage* or *Finnhub* (you can swap in any JSON API) |
| SMS delivery | [Twilio Python SDK](https://www.twilio.com/) |
| HTTP requests | `requests` |
| Environment variables | `os`, `.env` file (via `python‑dotenv`) |

---

