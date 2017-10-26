# beyond_word2vec
Slides for my doc2vec workshop/talk



# Setup Instructions

### 1) Clone repo

```bash
git clone git@github.com:andrewdblevins/beyond_word2vec.git
```

once you clone this repo, you can follow along these instructions in this notebook

### 2) Python Installs:

Please note, that we'll need several packages installed on your laptop.

If you have python, gensim and keras installed on your laptop you are probably good to go.

If you haven't performed installs yet, here are some steps to follow:

I generally recommend using the [anaconda package](https://anaconda.org/anaconda/python)

Create a conda environment:  

```bash
conda create -n beyondw2v python=3    
source activate beyondw2v
conda install anaconda     
```
Then install additional packages:    
```bash

conda install gensim
conda install -c conda-forge keras     
conda install -c conda-forge theano
```

### 3) Pretrained Word Vectors
Download the pretrained google news word vectors

**warning: This file is 3.6GB**


```python
!wget https://s3.amazonaws.com/mordecai-geo/GoogleNews-vectors-negative300.bin.gz
```

**Optional** you may want to test other pretrained vectors. If so, download those

* glove http://nlp.stanford.edu/projects/glove/
* sense2vec https://github.com/explosion/sense2vec
* fastText https://github.com/facebookresearch/fastText/blob/master/pretrained-vectors.md
* metaembeddings http://cistern.cis.lmu.de/meta-emb/

### 4) Evaluation Dataset

https://nlp.stanford.edu/projects/snli/

Download the following ~100MB:


```python
!wget https://nlp.stanford.edu/projects/snli/snli_1.0.zip
```
