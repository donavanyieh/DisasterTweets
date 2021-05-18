# Detecting disaster related text from twitter<br>
#### From Kaggle competition: Natural Language Processing with Disaster Tweets. View the full notebook with outputs here: https://www.kaggle.com/yiehyuheng/disaster-tweets-glove-stacking-ann-lstm

<b>Tech Stack</b><br>
NumPy, Pandas, Matplotlib, Seaborn, NLTK, TextBlob, Sklearn, GloVe word embeddings, Tensorflow (ANN, LSTM)
<br><br>
<b>Dataset</b><br>
https://www.kaggle.com/c/nlp-getting-started/data
<br><br>
<b>Problem Description</b><br>
Twitter has become an important communication channel in times of emergency. Agencies are increasingly interested in monitoring Twitter for emergencies (i.e. disaster relief organizations and news agencies).<br>
However, it is not always clear whether a person’s words are actually announcing a disaster. <br>For example, the text <b>"The sky looked ablaze"</b> may not be referring to a disaster. This may be clear to a human but no so much to a machine.
<br><br>
<b>Objective</b><br>
Create a machine learning model to predict which tweets are about real disasters and which are not.
<br><br>
<b>Summary of Approach</b><br>
<ol>
  <li>We clean each tweet in the dataset through a series of functions, including removing emojis, expanding abbreviations and lemmatizing each word</li>
  <li>We use GloVe word embeddings to get the vector representation of the word to capture semantic of each word. For each tweet, the overall semantic of the tweet is the average of all word vectors in the tweets</li>
  <li>We utilize a series of models, including stacking ensembles, ANN, and LSTM to evaluate F1-score.</li>
</ol>
