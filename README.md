# Fake-News-Detection-with-Machine-Learning
### Getting Started
```
##### 1- Understand the Problem Statement and business case 
##### 2- Import libraries and datasets
##### 3- Perform Exploratory Data Analysis
##### 4- Perform Data Cleaning
##### 5- Visualize the cleaned data
##### 6- Prepare the data by tokenizing and padding
##### 7- Understand the theory and intuition behind Recurrent Neural Networks
##### 8- Understand the theory and intuition behind LSTM
##### 9- Build and train the model
##### 10- Assess trained model performance
```


### IMPORT LIBRARIES AND DATASETS
```!pip install --upgrade tensorflow-gpu==2.0
!pip install plotly
!pip install --upgrade nbformat
!pip install nltk
!pip install spacy # spaCy is an open-source software library for advanced natural language processing
!pip install WordCloud
!pip install gensim # Gensim is an open-source library for unsupervised topic modeling and natural language processing
import nltk
nltk.download('punkt')

import tensorflow as tf
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from wordcloud import WordCloud, STOPWORDS
import nltk
import re
from nltk.stem import PorterStemmer, WordNetLemmatizer
from nltk.corpus import stopwords
from nltk.tokenize import word_tokenize, sent_tokenize
import gensim
from gensim.utils import simple_preprocess
from gensim.parsing.preprocessing import STOPWORDS
# import keras
from tensorflow.keras.preprocessing.text import one_hot, Tokenizer
from tensorflow.keras.preprocessing.sequence import pad_sequences
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense, Flatten, Embedding, Input, LSTM, Conv1D, MaxPool1D, Bidirectional
from tensorflow.keras.models import Model
from jupyterthemes import jtplot
jtplot.style(theme='monokai', context='notebook', ticks=True, grid=False) 
# setting the style of the notebook to be monokai theme  
# this line of code is important to ensure that we are able to see the x and y axes clearly
# If you don't run this code line, you will notice that the xlabel and ylabel on any plot is black on black and it will be hard to see them.
```
