# Assignment 1
Implement the Byte-Pair Encoding algorithm and apply it to a large dataset.

In this assignment you will implement the BPE algorithm, described in [Chapter 2 of J&M](https://web.stanford.edu/~jurafsky/slp3/2.pdf). We will then compare it to some other tokenization methods. You will write your code on Google Colab.

## Dependencies[^1]

For this assignment, we will have to load a corpus. [HuggingFace](https://huggingface.co) hosts a large number of corpora and provides a package called `datasets` that allows us to download and access a corpus easily in our code. After we run our implementation of BPE on the corpus we download, we will also run other existing tokenizers to compare. The other tokenizers are implemented in a package called [`nltk`](https://nltk.org) which contains a number of useful NLP tools.

`nltk` is already pre-installed on Google Colab so we can use it immediately. However, `datasets` is not installed by default. In order to install it, we will use a special syntax available in Colab (and Jupyter) notebooks.

```
!pip install datasets
```

The exclamation mark preceding `pip` informs Colab that you wish to run the line in the terminal instead of interpretting it as Python.

## Byte-Pair Encoding
![Original Work](https://img.shields.io/badge/OriginalWork-%23ff0077.svg?style=for-the-badge)

[^1]: A dependency is a package containing code written by someone else that you need in order to write or run your own code. Python has a package manager that allows you to install and update packages from a central repository. This makes it easy for people to share code and to make sure everyone has the right version. Several of the dependencies we will use are preinstalled on google colab so we don't have to add them specifically.
