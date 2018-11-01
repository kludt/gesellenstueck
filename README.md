# Digitales Gesellenstück
## Text Mining of abstracts on the subject of vitamin D

### Why this project was chosen
This project was chosen to learn how to extract features from text to get a DataFrame, how to process text to make it usable for ML algorithms and to study additional text specific techniques like Topic Modeling algorithms.

### Data
The data used in this project are nearly 70.000 abstracts on the subject of vitamin D. These abstracts were downloaded from PubMed (https://www.ncbi.nlm.nih.gov/pubmed/).

### Chosen approach
- extract features from text using regular expression
- isolate abstracts which classify their results as (non-)significant
    - label as many abstracts as possible if the results are significant or not significant
    - use an ML algorithm to classify the abstracts which could not be labeled by hand
        - use different text to vector algorithms (count vectorize & td-idf)
        - as MVP logistic regression is chosen, if not satisfactory Support Vector Machines are used as they do not overfit easily with wide data and according to literature have been used for text classification before
- try out different Topic Modeling algorithms (NFM & LDA) 

### Challenges
- getting features out of a text
    - no prior knowledge of regex (= regular expression)
- how to label the trainings data to predict, if an abstracts reports non-significant, significant results or both
- how to get descriptive topics

