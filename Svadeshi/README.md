### LSTM with embedding layer:

The Embedding layer is used to create word vectors for incoming words. It sits between the input and the LSTM layer, i.e. the output of the Embedding layer is the input to the LSTM layer.

The weights for the Embedding layer can either be initialized with random values, or more commonly, they are initialized with third-party word embeddings such as word2vec, GloVe or fasttext (or others) and these weights can optionally be fine-tuned during training. Using third party embeddings to build word vectors is as a form of transfer learning, since you transfer the semantic information between words that was learned during the embedding process.
