# Sentiment-Analytics
Real-time Retail &amp; Review Intelligence with Sentiment + Market Basket Analysis

# Notebook	Description
01_reddit_streaming.ipynb	Uses Reddit API (PRAW) to collect live comments from targeted subreddits.
02_cleaning_and_sentiment.ipynb	Cleans Reddit data and performs sentiment analysis with TextBlob.
03_amazon_reviews_analysis.ipynb	Analyzes review texts for sentiment and links them with star ratings.
04_market_basket_model.ipynb	Uses FP-Growth in PySpark for item association rule mining.

# Tech Stack
Language: Python 3.10+

NLP: TextBlob, NLTK

Big Data: PySpark

API & Web: PRAW (Reddit API)

Analysis: Pandas, NumPy, Matplotlib, Seaborn

Modeling: scikit-learn, FP-Growth

# Setup Instructions
# Install Requirements
bash
Copy
Edit
pip install -r requirements.txt
# Reddit API Setup
Go to https://www.reddit.com/prefs/apps

Create a new app and note your:

client_id

client_secret

user_agent

Add them to a .env file:

env
Copy
Edit
REDDIT_CLIENT_ID=your_id
REDDIT_CLIENT_SECRET=your_secret
REDDIT_USER_AGENT=shoplytics_pipeline
# Sample Insights
Positive Reddit sentiment increases on weekends across eCommerce subreddits.

Amazon product reviews with higher sentiment often correlate with 4- and 5-star ratings.

Common itemsets like ['phone_case', 'screen_protector'] have high lift and support, ideal for product bundling.

# Future Enhancements
Integrate Streamlit dashboard for live Reddit sentiment visualization.

Use BERT or DistilBERT for advanced sentiment classification.

Alert system for detecting sentiment dips across product discussions.
