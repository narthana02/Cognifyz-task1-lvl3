# Cognifyz-task1-lvl3
Analyze the text reviews to identify the most common positive and negative keywords.  Calculate the average length of reviews and explore if there is a relationship between review length and rating.
Certainly, let's summarize the theoretical concepts covered in the code:

1. **Importing Libraries:**
   - Libraries such as `pandas` and `matplotlib` are imported for data manipulation and plotting.
   - `stopwords` module from NLTK is imported for handling common English stopwords.

2. **Loading the Data:**
   - The dataset is loaded using `pd.read_csv('your_file.csv')`. Replace 'your_file.csv' with the actual file path containing the dataset.

3. **Identifying Negative Keywords:**
   - A list called `negative_keywords` is initialized to store negative keywords.
   - The `stopwords` set is defined to exclude common English stopwords during analysis.
   - For each review in the 'Cuisines' column:
     - The review text is split into words.
     - Words are converted to lowercase, and stopwords are removed.
     - If a word contains 'bad' or 'poor', it is considered a negative keyword and added to the list.

4. **Getting the Most Common Negative Keywords:**
   - A frequency distribution of negative keywords is calculated using `pd.Series(negative_keywords).value_counts()`.
   - The top 5 most common negative keywords are printed.

The primary focus here is on extracting and analyzing negative keywords from the 'Cuisines' column of the dataset. The process involves basic tokenization, lowercasing, and filtering out stopwords to identify negative sentiment indicators. The resulting frequency distribution provides insights into the most common negative keywords in the dataset.
