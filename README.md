# Sentiment-Analysis-on-Amazon-Reviews-using-Python
You are given a JavaScript Object Notation (JSON) file containing Amazon.com reviews for cell phones and accessories. 


 # 1. Preprocessing

- Dataset Structure:

{
  "reviewerID": "A30TL5EWN6DFXT",
  
  "asin": "120401325X",
  
  "reviewerName": "christina",
  
  "helpful": [0, 0],
  
  "reviewText": "They look good and stick good! I just don't like the rounded shape because I was always bumping it into things as I worked.",
  
  "overall": 4.0,
  
  "summary": "Looks Good",
  
  "unixReviewTime": 1400630400,
  
  "reviewTime": "05 21, 2014"
  
}

- Dataset Size: 194,439 entries
- Columns in the Dataset: ['reviewerID', 'reviewText', 'overall', 'asin', 'reviewerName', 'helpful', 'summary', 'unixReviewTime', 'reviewTime']

# Preprocessing Steps
Loaded the dataset from a JSON file.

Filtered unnecessary columns ('reviewerID', 'reviewText', 'overall').

Removed punctuation and converted text to lowercase.

Filtered out stopwords from the reviews.


 # 2. Thematic Analysis

Top Key Phrases or Words by Sentiment

# Positive Reviews:

great: 4.22%

good: 2.51%

love: 1.75%

excellent: 1.56%

recommend: 1.45%

nice: 1.23%

easy: 1.20%

works: 1.18%

like: 1.15%

well: 1.10%


# Negative Reviews:

bad: 2.08%

disappointed: 1.54%

dont like: 1.23%

poor: 1.14%

terrible: 1.12%

horrible: 1.10%

awful: 1.05%

waste of money: 0.93%

unsatisfied: 0.91%

wont buy: 0.78%



# 3. Sentiment Analysis
- Word Weights:

Positive Words: (e.g., 'great', 'awesome', 'amazing') with weights ranging from 0.5 to 0.95.

Negative Words: (e.g., 'bad', 'terrible', 'awful') with weights ranging from 0.01 to 0.5.

- Score Calculation: Calculates sentiment score based on occurrence and weighted value of sentiment words.
- Classification: Classifies sentiment as 'positive', 'negative', or 'neutral' based on the sentiment score.

# Results
Results are saved to 'sentiment_results.txt' file, containing each review text and its corresponding sentiment classification.

# Conclusion
The sentiment analysis project successfully preprocesses a large dataset of product reviews, performs thematic analysis to identify key positive and negative words, and classifies sentiments using predefined word weights. This approach provides insights into customer sentiments towards cell phones and accessories, aiding in understanding consumer preferences and product reception. 
