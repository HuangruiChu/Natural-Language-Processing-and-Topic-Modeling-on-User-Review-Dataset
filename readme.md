# Natural Language Processing and Topic Modeling on User Review Dataset

## Objective

in this project, we will analyze the underlying structure of documents automatically and visualize the clustering result using natural language processing models/tools.


## Dataset

[watch reviews](https://drive.google.com/file/d/192JMR7SIqoa14vrs7Z9BXO3iK89pimJL/view)

## NLP Machine Learning Process

1. Load Data
2. Text/Document Preprocessing: 
    - Tokenizing 
    - Stemming
3. Feature Engineering: 
    - Term Frequency – Inverse Document Frequency (TFIDF)
4. Modle Traing: 
    - K-means clustering and Topic Modeling - Latent Dirichlet Allocation

For "Tokenizing and Stemming" we use "[NLTK](https://www.nltk.org/index.html)" toolkits.

## Key Take aways

### Tokenizing

"Tokenization is the process of replacing sensitive data with unique identification symbols that retain all the essential information about the data without compromising its security." (cited from https://www.techtarget.com/searchsecurity/definition/tokenization)

After doing document tokenization, we usually remove “stop words” from the result set. Stopwords are words that don't convey significant meaning, e.g. a, the, an, in. lt includes 153 stopwords in nltk.corpus.stopwords.words("english").

### Stemming
Stemming is a process of counting inflected forms of a word together. lt helps us to reduce thenumber of unique vocabulary items that we need to track.

Boys -> boy

Looked->look

Be,are,is,am,was,were -> be

### TF-IDF

TF-IDF is the product of two statistics, term frequency and inverse document frequency.

### Latent Dirichlet Allocation
1. Latent Dirichlet allocation (LDA) is a generative statistical model. 
2. LDA is an example of a topic model.
    - In LDA, each document is assumed to be characterized by a particular set of topics
3. lf observations are words collected into documents, LDA result means that:

    - Each document is a mixture of a small number of topics.
    
    - Each word's creation is attributable to one of the document's topics
