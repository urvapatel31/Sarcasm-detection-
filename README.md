Sarcasm Detection Portal
This project aims to detect sarcasm in text input using machine learning models. It provides a web interface for users to enter text, and the system predicts whether the input text is sarcastic or not.

Introduction
Past studies in sarcasm detection mostly make use of Twitter datasets collected using hashtag-based supervision. However, such datasets are noisy in terms of labels and language. Furthermore, many tweets are replies to other tweets, and detecting sarcasm in these requires the availability of contextual tweets.

To overcome the limitations related to noise in Twitter datasets, this project uses a News Headlines dataset for sarcasm detection collected from two news websites. The Onion aims at producing sarcastic versions of current events, and we collected all the headlines from News in Brief and News in Photos categories (which are sarcastic). Real (non-sarcastic) news headlines are collected from HuffPost.

Dataset Overview
The dataset consists of about 28,000 text data points, where each data category belongs to one of two categories: sarcastic or not sarcastic.

Models Used
Two models are used for making predictions:

Word2Vec Embeddings
GloVe Embeddings
Requirements
Python 3.x
Tensorflow
Keras
Streamlit
NLTK
Gensim
NumPy
Pandas
Matplotlib
Seaborn
BeautifulSoup
Installation
To run this project locally, follow these steps:

Clone the repository:
bash
Copy code
git clone <repository_url>
Install the required dependencies:
Copy code
pip install -r requirements.txt
Run the Streamlit app:
arduino
Copy code
streamlit run app.py
Usage
Once the Streamlit app is running, open your web browser and navigate to the provided URL. You will see the Sarcasm Detection Portal interface. Enter your text in the text input field and click the "Predict" button. The system will display whether the input text is sarcastic or not.

File Structure
app.py: Streamlit application code.
sarcasm_detection_model.h5: Pre-trained sarcasm detection model.
word2vec_model.h5: Pre-trained Word2Vec model.
glove_embeddings.h5: Pre-trained GloVe embeddings.
README.md: Documentation file.
Credits
TheOnion: Providing sarcastic news headlines.
HuffPost: Providing real news headlines.
Kaggle: Hosting the News Headlines dataset.
Google: Developing Word2Vec model.
Stanford NLP: Developing GloVe embeddings.# Sarcasm-detection-
