## Welcome
Find below short descriptions and links to the reports for the two projects I completed as part of a one term nanodegree in Natural Language Processing with Udacity (April 2020 - June 2020). In this program, I learned and put in practice the concepts behind natural
language processing and speech recognition, including machine translation, part of speech tagging, and
sentiment analysis. 

## Part of Speech Tagging

Part of speech tagging is the process of determining the syntactic category of a word from the words in its surrounding context. It is often used to help disambiguate natural language phrases because it can be done quickly with high accuracy. Tagging can be used for many NLP tasks such as for information retrieval or for word sense disambiguation.

The project is built on a template provided by Udacity. The approach uses the _Pomegranate library_ to build a _Hidden Markov Model (HMM)_ for part of speech tagging using an 'universal' tag set. Hidden Markov models have been able to achieve more than 96% tag accuracy with larger tag sets on realistic text corpora. These models have also been used for speech recognition and speech generation, machine translation, and human gesture recognition for computer vision, and more.

There are two taggers constructed in this project. First a Most Frequent Class tagger to use as a baseline is built. A good baseline for tagger performance is to simply choose the tag most frequently assigned to each word. This 'most frequent class' tagger inspects each observed word in the sequence and assigns it the label that was most often assigned to that word in the corpus.

The HMM tagger has one hidden state for each possible tag, and is parameterized by two distributions: the emission probabilities giving the conditional probability of observing a given word from each hidden state, and the transition probabilities giving the conditional probability of moving between tags during the sequence.

_This presentation is using Jupyter Notebook with a Python 3 kernel, using Pomegranate library._

[Link: POS Tagging](http://htmlpreview.github.io/?https://github.com/SolanaO/Natural-Language-Processing/blob/master/dand.T1P1.Explore_Weather_Trends.html)


## Machine Translation Project

In this notebook (part of it provided by Udacity) I build a deep neural network that functions as part of an end-to-end machine translation pipeline. The completed pipeline accepts English text as input and returns the French translation. The project has three parts:

  - _Preprocess_ - convert text to sequence of integers.<br>
  - _Models_ - create several deep neural networks which accept a sequence of integers as input and return a probability distribution over possible translations.<br>
  - _Prediction_ - run the model on English text sample.

There are four models built in this project: 
    - a simple RNN,
    - a RNN with Embedding (from Keras),
    - a Bidirectional RNN,
    - an Encoder - Decoder RNN.

_This project requires GPU acceleration to run efficiently. The project is written in: Python 3, NumPy, TensorFlow 1.x, Keras 2.x._

