# Preparation (Text Data Processing)

(Last updated: Feb 27, 2023)

This part will prepare you with the background knowledge that we will use for this module.
You will install some useful Python packages for Natural Language Processing (NLP) and Machine Learning (ML).
You will explore some small applications to get a grasp of word embeddings.


## Task 1: Check your installations

In this module, we will make use of some Python modules that require some extra downloads. We will use NLTK (Natural Language Toolkit) and spaCy for NLP and PyTorch for ML.

First, for NLTK and spaCy, install both through the package manager of your choice using one of the following commands: `conda install nltk spacy` or `pip install nltk spacy`. You might already have one of these installed.

Then, download the additional data for NLTK. Open a Python interpreter or notebook and run the following code:

```
import nltk
nltk.download('averaged_perceptron_tagger')
nltk.download('omw-1.4')
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

Download the spaCy model we'll use in further tasks using this command: `python -m spacy download en_core_web_sm`.

Finally, install PyTorch using the selector on [their website](https://pytorch.org/get-started/locally/). Use the stable version, choose your current operating system, package manager (`conda` or `pip`), and programming language (Python). If you have an NVIDIA GPU and are considering some more (heavy) ML work for other projects or your thesis, it might be worth taking some hours to look into using CUDA as a computing platform. However, for this module, just using the CPU suffices. 

## Task 2: Explore WebVectors

In the field of natural language processing (NLP), word embeddings are a way to represent a word as a vector of real numbers. This representation is useful for analyzing text. The vector is designed to encode the meaning of the word so that words that have similar meanings are closer together in the vector space.

The Nordic Language Processing Laboratory made the website [WebVectors](http://vectors.nlpl.eu/explore/embeddings/en/) to get familiar with the concept of word vectors by offering some nice interactive examples of how word vectors can be used. Browse around the website and answer the following questions:

- Using the Similar Words page: What are some semantic associates for the proper noun 'Amsterdam' in the English Wikipedia model? Do other models yield different results?
- Using the Calculator page: If "scientist" is related to "science", "artist" is related to what? Were you able to find some other nice combinations that did or did not work?
- Take a look at the Models page: Which types of preprocessing were used before training the models?