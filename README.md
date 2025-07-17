🇮🇳 BharatStocks-GPT: Intelligent Stock Insights Dashboard 📈
BharatStocks-GPT is an AI-powered stock analysis dashboard offering real-time insights for both global and Indian stock markets. Built with Python and Streamlit, this dynamic tool is designed for investors, analysts, and finance enthusiasts seeking advanced analytics, smart forecasting, and AI-powered insights.

🎥 Watch Demo Video

🌟 Features
Feature	Description
📊 AI-Enhanced Company Overview	Intelligent summaries powered by Google Gemini.
📉 Detailed Financials	Income statements, balance sheets, and cash flows from FMP.
🔮 Probabilistic Stock Models	Advanced risk and price movement analytics.
📈 Forecasting Engine	Stock trend predictions via historical data and ML models.
📰 Live News + Sentiment Analysis	Instant sentiment analysis using NewsAPI & TextBlob.
🔍 Smart Ticker Search	Autocomplete powered by Alpha Vantage and FMP.
🛠️ Tech Stack
Frontend/Backend: Streamlit

Language: Python 3.9+

Data Handling: Pandas, NumPy

ML Models: Scikit-learn

Sentiment: TextBlob

Visualization: Plotly, Seaborn, Matplotlib

📡 APIs Used
Financial Modeling Prep (FMP)

Alpha Vantage

NewsAPI

Google Gemini

⚙️ Getting Started
Prerequisites
Python 3.9+

Git

Installation
bash
# Clone the repository
git clone https://github.com/RajuKumar077/BharatStocks-GPT.git
cd BharatStocks-GPT

# Create a virtual environment
python -m venv venv

# Activate (Windows)
.\\venv\\Scripts\\activate

# Activate (macOS/Linux)
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
🔑 API Key Setup
Update app.py with your API credentials:

python
# API Keys
NEWS_API_KEY = "YOUR_NEWSAPI_KEY"
FMP_API_KEY = "YOUR_FMP_KEY"
GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"
ALPHA_VANTAGE_API_KEY = "YOUR_ALPHA_VANTAGE_API_KEY"
⚠️ Use secrets.toml for secure API key management on Streamlit Cloud.

🚀 Running the App
bash
streamlit run app.py
💡 How to Use
Search: Enter ticker symbols (e.g., AAPL, TCS.BO, RELIANCE.NS) or company names.

Select: Choose from the autocomplete dropdown.

Analyze: Click 🚀 Analyze Stock.

Explore Tabs:

📄 Company Overview

📊 Financials

📉 Probabilistic Models

🔮 Forecasting

📰 News Sentiment

📁 Project Structure
text
BharatStocks-GPT/
├── app.py                      # Main app launcher
├── requirements.txt            # Dependencies list
├── assets/
│   └── style.css               # Custom styles
├── pages/                      # Modular components
│   ├── __init__.py
│   ├── fmp_autocomplete.py
│   ├── yahoo_autocomplete.py
│   ├── stock_summary.py
│   ├── financials.py
│   ├── probabilistic_stock_model.py
│   ├── forecast_module.py
│   └── news_sentiment.py
└── README.md
🔮 Roadmap
🤖 Deep Learning (LSTM, Transformers) for forecasts

📈 More technical analysis indicators

👤 User authentication and portfolio tracking

🔔 Custom price/news alerts

📊 Multi-stock comparative analysis

📌 Interactive drag-and-drop dashboards

🤝 Contributions
Contributions welcome!

bash
# Fork > Branch > Code > Commit > PR
git checkout -b feature/YourFeature
git commit -m "Add: Your new feature"
git push origin feature/YourFeature
📜 License
Project released under the MIT License.

🙏 Acknowledgements
Streamlit for the intuitive UI framework

API Providers: FMP, Alpha Vantage, NewsAPI, Google Gemini

Python Open Source Community for libraries like Pandas, Scikit-learn, Plotly

📽️ Demo Video
Click below for a walkthrough:
🎥 Watch BharatStocks-GPT Demo

Made with 💼 by Raju Kumar
