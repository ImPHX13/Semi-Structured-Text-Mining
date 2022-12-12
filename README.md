The NLTK library has a number of stemmers, such as the Porter, Lancaster and Snowball Stemmers. Used at least two of those stemmers and compared the differences in some of the stemmed words. Used the word tokenizer to tokenize words before stemming. Selected one of the stemmer for the rest of the analysis. After stemming, constructed the term-document matrix. Eliminated stop words when constructing the term document matrix.
Then constructed the TF-IDF matrix from the term-document matrix. After this I combined the TF-IDF matrix with Customer data.
There are two types of feature selection methods used - the filter type and the wrapper type.
Filter type - Used Python's SelectKBest module to find the K best features.
Wrapper type - Used the SelectFromModel method to find a good set of features on the combined data.
Split the combined dataset into a training (80%) and a test set (20%). Using the best set of features from each method (filter and wrapper), built new classification model and evaluated them.
