# AI_ML_Berkeley_Capstone_20.1

# Exploratory Data Analysis (EDA): Impact of Tweet Sentiments on Stock Prices

### Project Overview

This analysis investigates how tweet sentiment affects stock prices using a dataset containing stock return data and tweet sentiment scores. The dataset was preprocessed, cleaned, and visualized to understand relationships between sentiment polarity, stock returns, trading volume, and tweet counts.

### Data Cleaning and Preprocessing

- Dropped unnecessary columns.
- Converted date columns to appropriate datetime formats.
- Handled missing values.
- Ensured numeric columns were correctly formatted for analysis.

### Key Visualizations and Insights

#### 1. Distribution of Sentiment Scores
![download](https://github.com/user-attachments/assets/ae6d1f1f-b128-4a0a-91ac-622c4b687c9e)

##### The lstm_polarity column represents the sentiment polarity of tweets as determined by a Long Short-Term Memory (LSTM) neural network model. The LSTM model reads the text of each tweet and derive a sentiment score, typically denoting positive, negative, or neutral sentiment.
##### Textblob_polarity column represents sentiment polarity of tweets as analyzed using TextBlob library. TextBlob is a Python library for processing textual data with APIs for language processing like sentiment analysis. Polarity score returned by TextBlob ranges from -1 to 1, with: 
##### -1: Represents an extremely negative sentiment.
##### 0: Represents a neutral sentiment.
##### 1: Represents an extremely positive sentiment.

#### Findings:

- LSTM and TextBlob sentiment polarities show different distributions.
- The polarity scores generally center around neutral values.

#### 2. Stock Returns Comparison: 1-Day vs. 7-Day
![download](https://github.com/user-attachments/assets/f4328c95-cfd8-46ae-84d1-5b1d3a089b72)

#### Findings:

- 7-day returns are more spread out than 1-day returns.
- The data suggests that short-term fluctuations do not always translate into long-term movement.

#### 3. Sentiment Scores vs. 1-Day Stock Returns
![download](https://github.com/user-attachments/assets/e501a568-d6f4-4868-a4ef-6e7835470657)

#### Findings:

- Weak correlation observed between sentiment polarity and 1-day stock returns.
- Some extreme sentiment scores correspond to higher volatility in returns.

#### 4. Sentiment Scores vs. 7-Day Stock Returns
![download](https://github.com/user-attachments/assets/6dfbdc90-e9c2-4a92-afc3-a5e5669e8eb9)


#### Findings:

- Similar weak correlation as seen in 1-day returns.
- Longer-term returns may be influenced by additional market factors beyond sentiment.


#### Next Steps
For the second part of this project, I will begin with a linear regression model as our baseline machine learning model. Linear regression is an effective model to implement in this analysis because it will be capable of placing the correlation between stock price movement and tweet sentiment into simpler terms. With this model implemented as a baseline, it will be capable of comparing its accuracy to more intricate models like random forest regression or neural networks in the future.



### Repository Structure

- CapstoneReport.ipynb: Jupyter Notebook with full EDA analysis.
- screenshots/: Folder containing images of generated plots.
- data/: Folder containing the dataset.
- README.md: This document summarizing the analysis.
