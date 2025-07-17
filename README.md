BharatStocks-GPT: Intelligent Stock Insights Dashboard 📈

 (Note: Replace this with your actual Streamlit Cloud app URL once deployed)

🌟 Overview
BharatStocks-GPT is a cutting-edge, AI-powered stock analysis dashboard designed to provide comprehensive, real-time insights into global and Indian stock markets. Built with Python and Streamlit, this interactive application aims to empower investors, analysts, and financial enthusiasts with intelligent tools for data-driven decision-making.

It consolidates diverse financial data streams, applies advanced analytical models, and leverages artificial intelligence to offer a holistic and intuitive view of stock performance and market sentiment.

✨ Features
This interactive application leverages various cutting-edge APIs to provide a holistic view of the market:

📈 Company Overview (AI-Enhanced): Get concise, AI-generated summaries and critical information about any stock, powered by Google Gemini.

💰 In-depth Financials: Dive into detailed balance sheets, income statements, and cash flow data sourced from Financial Modeling Prep.

🔮 Probabilistic Stock Models: Understand potential price movements and assess risk with advanced data-driven models.

📉 Advanced Price Forecasting: Utilize historical data to project future stock prices, aiding in strategic planning.

📰 Real-time News & Sentiment Analysis: Stay updated with the latest market news, automatically analyzed for sentiment to gauge public perception.

🔎 Intelligent Ticker Search: Easily find both global (e.g., AAPL, MSFT) and Indian stocks (e.g., RELIANCE.NS, TCS.BO) with smart autocomplete functionality, pulling data from Alpha Vantage and other sources.

🚀 Live Demo
Experience BharatStocks-GPT in action!


(Click the badge above to watch the demo video on Google Drive.)

🛠️ Technologies Used
Frontend/Backend Framework: Streamlit

Core Programming Language: Python 3.9+

Data Manipulation & Analysis: Pandas, NumPy

Historical Data Retrieval: yfinance, pandas-datareader, requests (for direct API calls)

Machine Learning/Statistical Models: Scikit-learn

Natural Language Processing (Sentiment): TextBlob

Data Visualization: Plotly, Matplotlib, Seaborn

External APIs:

Financial Modeling Prep (FMP)

Alpha Vantage

NewsAPI

Google Gemini

⚙️ Getting Started (Local Setup)
Follow these steps to get a local copy of BharatStocks-GPT up and running on your machine.

Prerequisites
Ensure you have Python 3.9 or higher installed.

Installation
Clone the repository:

git clone https://github.com/RajuKumar077/BharatStocks-GPT.git
cd BharatStocks-GPT

Create and activate a virtual environment (recommended):

python -m venv venv
# On Windows
.\venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate

Install dependencies:

pip install -r requirements.txt

(Note: The requirements.txt includes essential libraries for the core functionality. If you encounter issues, ensure your pip is up to date.)

API Keys Configuration
This application relies on several external APIs. You will need to obtain your own API keys and configure them within app.py.

Open app.py in your code editor.

Locate the API Key section (around lines 30-35) and replace the placeholder values with your actual keys:

# API Keys
NEWS_API_KEY = "YOUR_NEWSAPI_KEY" # Get from newsapi.org
FMP_API_KEY = "YOUR_FMP_KEY"     # Get from financialmodelingprep.com
GEMINI_API_KEY = "YOUR_GEMINI_API_KEY" # Get from Google AI Studio
ALPHA_VANTAGE_API_KEY = "YOUR_ALPHA_VANTAGE_API_KEY" # Get from alphavantage.co

Important: For production deployments (like Streamlit Cloud), it's highly recommended to use Streamlit Secrets instead of hardcoding keys directly in app.py.

Running the Application
Once dependencies are installed and API keys are configured, you can run the Streamlit application:

streamlit run app.py

This will open the application in your default web browser.

💡 Usage
Enter a Ticker: Use the search bar to type a stock ticker symbol (e.g., AAPL, MSFT) or a company name fragment (e.g., Reliance, Tata).

Select Suggestions: If suggestions appear, click on the desired stock to auto-fill the input.

Analyze: Click the "🚀 Analyze Stock" button to fetch data and display the various analysis tabs.

Explore Tabs: Navigate through "Company Overview," "Financials," "Probabilistic Models," "Forecasting," and "News Sentiment" to gain different insights.

📂 Project Structure
fingpt-one/
├── app.py                     # Main Streamlit application file
├── requirements.txt           # Python dependencies
├── assets/                    # Static assets like CSS
│   └── style.css              # Custom CSS for styling
├── pages/                     # Directory for modularizing Streamlit pages/functions
│   ├── __init__.py            # Makes 'pages' a Python package (CRITICAL for imports)
│   ├── fmp_autocomplete.py    # FMP-based autocomplete logic (if still used)
│   ├── yahoo_autocomplete.py  # Alpha Vantage-based autocomplete logic
│   ├── stock_summary.py       # Module for company overview
│   ├── financials.py          # Module for financial statements
│   ├── probabilistic_stock_model.py # Module for probabilistic models
│   ├── forecast_module.py     # Module for stock price forecasting
│   └── news_sentiment.py      # Module for news fetching and sentiment analysis
└── README.md                  # This README file

🚀 Future Enhancements
Advanced ML Models: Integrate more sophisticated deep learning models (e.g., LSTMs) for enhanced forecasting accuracy.

Technical Indicators: Add a wider range of technical analysis indicators and charting options.

Portfolio Management: Implement user authentication and features for tracking personal portfolios.

Alerts & Notifications: Set up custom alerts for price targets or significant news events.

Comparative Analysis: Allow users to compare multiple stocks side-by-side.

Interactive Charting: Enhance existing charts with more interactive features and custom overlays.

🤝 Contributing
Contributions are welcome! If you have suggestions for improvements, new features, or bug fixes, please feel free to:

Fork the repository.

Create a new branch (git checkout -b feature/YourFeatureName).

Make your changes.

Commit your changes (git commit -m 'Add new feature').

Push to the branch (git push origin feature/YourFeatureName).

Open a Pull Request.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgements
Streamlit community for the amazing framework.

Providers of the various financial and news APIs for their data.
