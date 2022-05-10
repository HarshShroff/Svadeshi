# How to run?

1. Clone this repo
2. Go to `Svadeshi/Svadeshi`
3. Open `Neural translation.ipynb`
4. Run all cells sequencially
5. If everything goes as expected, you will hear English translation and original Sanskrit shloka


# Files and directories

## Data
`Sanskrit.txt` and `English.txt` are data files containing 700 Shlokas and thier translations, respectively.


## Model dir
This model contains the saved LSTM with embedding layer to avoid frequent trainings.

### LSTM with embedding layer:

The Embedding layer is used to create word vectors for incoming words. It sits between the input and the LSTM layer, i.e. the output of the Embedding layer is the input to the LSTM layer.

The weights for the Embedding layer can either be initialized with random values, or more commonly, they are initialized with third-party word embeddings such as word2vec, GloVe or fasttext (or others) and these weights can optionally be fine-tuned during training. Using third party embeddings to build word vectors is as a form of transfer learning, since you transfer the semantic information between words that was learned during the embedding process.


## `.mp3` files
These files are named as `en_x[n].mp3` and `sa_x[n].mp3`; where __en__ and __sa__ represent English and Sanskrit, __n__ is the line number (or index) of the selected line.
