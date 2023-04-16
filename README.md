# Italian neologisms language classification

**Aim of the project**

The aim of this project is to automatically identify the source language of some italian neologisms or other multilingual words by classifying character sequences with different supervised learning algorithms (Naive Bayesian, Random Forest, Logistic Regression,  SMV Linear, SMV Sigmond, SMV RBF).

Count, TF-IDF and language-dependent weigth matrices were built and used for the classification.

**Main challenges**

Word length: the shorter the segments, the most difficult is the classification task.
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
