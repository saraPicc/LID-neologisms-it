# Italian neologisms language classification

**Aim of the project**

The aim of this project is to automatically identify the source language of some italian neologisms or other multilingual words by classifying character sequences with different supervised learning algorithms.


**Experiments**

Different kind of classifiers, matrices and n-grams: 


MATRIX | CLASSIFIER | N-GRAMS | 
-------|------------|---------|
count matrix | Naive Bayesian | 2-grams
count_matrix | Random Forest | 2-grams
count matrix | Logistic Regression | 2-grams
count_matrix | SMV Linear | 2-grams
count_matrix | SMV Sigmond | 2-grams
count_matrix | SMV RBF | 2-grams
Tf-idf | Naive Bayesian | 2-grams
Tf-idf  | Random Forest | 2-grams
Tf-idf | Logistic Regression | 2-grams
Tf-idf | SMV Linear | 2-grams
Tf-idf | SMV Sigmond | 2-grams
Tf-idf | SMV RBF | 2-grams

**Main challenges**

Word length: the shorter the segments, the most difficult is the classification task <br/>
Huge quanitity of features to classify: trigrams or bigrams

**Data**

The data used to train the models consists in an english-italian corpus of words from Wikipedia articles sampled through Plainstream. 
Words' starting and ending were also treated as bigrams through the tags '^' and '$', making more efficient the identification task for example in the case of words ending with consonants (that are very unusual in Italian).

**Training and test**

The data was shuffled and split for the training (80%) and test (20%). 
After the training, cross validation has been performed to check the consistency of the classification.


**Conclusions**

Best classification according to:

- Classifier performance
- Languages involved
- N-grams

**References**:


*   Plainstream https://github.com/jimmycallin/plainstream
*   scikit-learn https://scikit-learn.org/stable/index.html
*   Class material
