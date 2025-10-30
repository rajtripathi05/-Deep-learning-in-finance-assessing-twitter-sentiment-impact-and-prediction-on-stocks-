1. Group Formation

Group Number 35
● Name: Raj Tripathi (16014223062)

●
https://docs.google.com/spreadsheets/d/1h7al9GiFlK73i9YDmEBMeXak-SpNH2N2AQ5p8P
lKxBQ/edit?gid=438850232#gid=438850232

2. Paper Selection link:
( If link not working also shared in Google sheets)

Github Link-
https://github.com/rajtripathi05/-Deep-learning-in-finance-assessing-twitter-sentiment-im

pact-and-prediction-on-stocks-
https://peerj.com/articles/cs-2018/

3. Summary of research paper selected :
The research paper, "Deep Learning in Finance: Assessing Twitter Sentiment
Impact and Prediction on Stocks" by Kaifeng Guo and Haoling Xie, investigates the
relationship between public sentiment on Twitter and stock market fluctuations
and proposes a deep learning framework to predict stock prices by integrating
sentiment information [cite: 15, 16, 20, 97].
The study highlights how social media sentiment reflects investor behavior and
demonstrates that incorporating sentiment into predictive models can improve the
accuracy of stock forecasts. The paper’s key contributions include:
● Fine-Tuned Sentiment Model: A pre-trained language model (ROBERTa) was
fine-tuned specifically on stock-related Twitter data to accurately classify tweets
as positive, neutral, or negative, capturing subtle financial sentiment nuances [cite:
21, 55, 69, 103, 104].

● Empirical Validation: Experiments on multiple datasets revealed a statistically
significant correlation between Twitter sentiment and stock price movements,
enhancing the predictive capability of the proposed deep learning models [cite: 23,
70].
● Transparency and Interpretability: The authors employed diverse evaluation
metrics to provide clear insights into model performance, improving interpretability
for broader audiences [cite: 61, 62, 71].

4. Theory/Implementation Explanation
This project reproduces the methodology of the paper, focusing on sentiment-informed
stock price prediction using deep learning.
Concept: Sentiment-Enhanced Stock Prediction
● Sentiment Extraction: A fine-tuned ROBERTa model predicts the sentiment polarity
of stock-related tweets (positive, neutral, negative).
● Stock Prediction: An LSTM-based RNN model takes historical stock prices and
sentiment features as input to forecast future stock prices.
● Integration: Combining sentiment and historical prices enables the model to capture
market dynamics beyond price trends alone.

Dataset Used:
● Original research used multiple stocks (Tesla, Apple).
● For reproduction, we used stock_data.csv (original dataset) and TWTR.csv
(new dataset for extension).
● Features included Closing Price and Sentiment Polarity (−1 to +1), generated via
TextBlob or simulated text.

5. Methodology Flow:
1.Data Collection – Stock price datasets (stock_data.csv and TWTR.csv) were

imported, along with synthetic or real tweets for sentiment.

2. Data Preprocessing – Cleaned missing values, converted dates to datetime, sorted
chronologically, and normalized features with MinMaxScaler.

3. Feature Extraction – Extracted sentiment polarity using TextBlob and combined with
normalized closing prices.

4. Model Training – A two-layer LSTM network (64 neurons per layer, Dropout 0.2) trained
on sequences of stock price + sentiment features.

5. Prediction Step – Forecasted stock closing prices and derived directional movement
(Up/Down) from regression outputs.

6. Evaluation – Measured performance using MSE loss, directional accuracy, and
classification metrics (precision, recall, F1-score).

7. Result Visualization – Plotted predicted vs actual stock prices and generated confusion
matrices for classification performance.

6. Advantages of Sentiment-Enhanced Prediction
● Improved Accuracy: Incorporating sentiment provides context beyond price trends.
● Applicability: The methodology can be extended to multiple stocks or new datasets
(e.g., TWTR.csv).
● Interpretability: Positive/negative sentiment trends correlate with upward/downward
price movements.

7. Extension

The approach was successfully extended to a new dataset (TWTR.csv), demonstrating:
● Generalizability of the model across different stocks and time periods.
● Adaptability to other domains where text-based sentiment influences numerical
trends.
● Validation of predictive power using MSE and directional accuracy (~72–73%).




Dataset 1 : Twitter Stock Market Analysis: Case Study
https://www.kaggle.com/datasets/bhanupratapbiswas/twitter-stock-market-analysis-case-study

Dataset2 : Stock-Market Sentiment Dataset

https://www.kaggle.com/datasets/yash612/stockmarket-sentiment-dataset
