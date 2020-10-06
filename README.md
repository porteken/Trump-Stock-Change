# Trump-Stock-Change
Rpubs Notebook: https://rpubs.com/porteken/Trump-Stock-Change

This project attempts to predict how trump's tweets changes SPY (SPDR S&P 500 Trust ETF). I used Python to process trump tweet's into a cosine similarity score using Spacy and Bert transformer, and random forest in R for the classification task. Below are some assumptions and parameters I had for this project. 

1. A positive change is when the close price was greater than the open price (Change=1) and vice versa for a negative change (Change=0).
2. If trump tweeted in the morning (AM) then the tweet score was tested against the same date stock change.  If it was in the evening (PM) then the tweet score was tested against the next date stock change.   If the tweet was on a weekend or holiday,  the score would be compared against the next trading day.
3. The SPY data and tweets are from October 2018 to September 2019

