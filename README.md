# Trump-Stock-Change Mod
Rpubs Notebook: https://rpubs.com/porteken/Trump-Stock-Change-Mod
This project attempts to predict how trump's tweets changes SPY (SPDR S&P 500 Trust ETF). Unlike Trump-Stock-Change (master branch), I used RBERT instead of Python to process trump tweet's into a cosine similarity score using Spacy and Bert, and random forest in R for the classification task. Below are some assumptions and parameters I had for this project. 
1. A positive change is when the close price was greater than the open price and vice versa for a negative change. 
2. If trump tweeted in the morning (AM) then the tweet score was tested against the same date stock change. 
3. If it was in the evening (PM) then the tweet score was tested against the next date stock change. 
4. If the tweet was on a weekend or holiday, the score would be compared against the next trading day. 
