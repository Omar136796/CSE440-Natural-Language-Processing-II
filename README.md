# CSE440 – Natural Language Processing II (BRAC University)

Lab assignments from CSE440 (Fall 2025), BRAC University's natural language processing
course, in Python. Covers corpus analysis with NLTK, text vectorization,
word embeddings, and neural networks for text classification. Each lab
folder contains my solution code and the assignment question (PDF).

## Labs

| Lab | Topic | Tasks | Code | Question |
|-----|-------|-------|------|----------|
| 01 | Corpus Analysis with NLTK | 1. Exploring the Gutenberg and Reuters corpora<br>2. Word clouds comparing two inaugural addresses (Roosevelt 1945 vs. Trump 2025)<br>3. Tokenization, stopword removal, lemmatization, and a top-30 word frequency plot for a negative movie review<br>4. Trigram co-occurrence matrix of the top 10 words in Truman's 1945 State of the Union<br>5. Vowel bigram frequency distribution in the French Universal Declaration of Human Rights | [lab01_nltk_corpus_analysis.py](Lab01/lab01_nltk_corpus_analysis.py) | [PDF](Lab01/Assignment01_NLTK_Corpus_Analysis.pdf) |
| 02 | Text Vectorization & Word Embeddings | 1. Bag-of-Words (CountVectorizer) on 50,000 Amazon reviews<br>2. TF-IDF and the top 25 highest-scoring words<br>3. Word analogies with GloVe embeddings (Paris − France + Italy ≈ Rome)<br>4. Training Word2Vec Skip-gram and CBOW models on the Brown corpus and testing analogies (King − Man + Woman) | [lab02_text_vectorization_and_word_embeddings.py](Lab02/lab02_text_vectorization_and_word_embeddings.py) | [PDF](Lab02/Assignment02_Text_Vectorization_and_Word_Embeddings.pdf) |
| 03 | Neural Networks for Classification | 1. Feed-forward neural network on the Wine dataset with loss and accuracy curves<br>2. Shallow embedding-based model for IMDb sentiment analysis, with ROC curve and AUC<br>3. Deep model with dropout, compared with the shallow model on training time, accuracy, overfitting, and confusion matrices | [lab03_neural_networks_for_classification.py](Lab03/lab03_neural_networks_for_classification.py) | [PDF](Lab03/Assignment03_Neural_Networks_for_Classification.pdf) |

## Datasets
Most datasets load automatically (NLTK corpora, scikit-learn's Wine
dataset, and Keras's IMDb dataset). Lab 02 also needs two large files
that are not included in this repo because of their size. Download them
and place them in the `Lab02` folder:

- **Amazon Reviews Polarity** (`train.csv`), available on Kaggle
- **GloVe 6B embeddings** (`glove.6B.100d.txt`), from https://nlp.stanford.edu/projects/glove/

## How to run
The code was written in Google Colab and exported as `.py` files. To run a
lab, paste it into a Colab notebook, or run it locally after installing the
libraries below. Lines starting with `!pip install` and `drive.mount()` only
work inside Colab.

## Tools
Python 3 · NLTK · scikit-learn · gensim · TensorFlow/Keras · pandas · NumPy · Matplotlib · WordCloud
