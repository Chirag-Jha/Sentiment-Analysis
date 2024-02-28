## Sentiment Analysis using BERT

This Python script demonstrates how to perform sentiment analysis on reviews using the BERT (Bidirectional Encoder Representations from Transformers) model. The script utilizes the Hugging Face `transformers` library to load a pre-trained BERT model for sequence classification and tokenize the input text.

### Steps:

1. **Install Required Libraries:**
   - `transformers`
   - `torch`
   - `requests`
   - `beautifulsoup4`
   - `pandas`
   - `numpy`

2. **Load BERT Model and Tokenizer:**
   - The script uses `AutoTokenizer` and `AutoModelForSequenceClassification` from the `transformers` library to load a pre-trained BERT model and tokenizer for sequence classification.

3. **Scrape Reviews:**
   - The script uses the `requests` library to fetch reviews from a specified URL. It then uses `BeautifulSoup` to parse the HTML content and extract review text.

4. **Tokenize Reviews:**
   - The review text is tokenized using the BERT tokenizer, and the tokens are encoded into a tensor for input to the BERT model.

5. **Perform Sentiment Analysis:**
   - The encoded tokens are passed through the BERT model, which predicts the sentiment of each review. The sentiment is determined based on the highest probability class predicted by the model.

6. **Display Results:**
   - The script creates a pandas DataFrame containing the reviews and their corresponding sentiment scores, which are then displayed.
