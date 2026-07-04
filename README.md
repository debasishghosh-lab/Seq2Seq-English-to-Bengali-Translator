# Seq2Seq English → Bengali Translator

A simple English to Bengali translator built using an Encoder-Decoder (Seq2Seq) architecture with LSTMs in TensorFlow.

The purpose of this project was to understand how Seq2Seq models work from scratch before moving on to Attention Mechanisms and Transformers.


## What I Learned

- Building an Encoder-Decoder architecture
- Understanding Embedding layers
- Implementing Teacher Forcing
- Preparing decoder inputs and targets
- Building separate training and inference models
- Word-by-word sequence generation during inference

## Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Google Colab

## Project Workflow
 English Sentence
        │
        ▼
Tokenization
        │
        ▼
Embedding
        │
        ▼
Encoder LSTM
        │
        ▼
Context (Hidden + Cell States)
        │
        ▼
Decoder LSTM
        │
        ▼
Dense + Softmax
        │
        ▼
Bengali Translation


## Limitations

- Uses a very small manually created dataset for learning purposes.
- Designed to understand Seq2Seq architecture rather than achieve production-level translation.
- Relies on a fixed-size context vector, making it less effective for longer or more complex sentences.

## Future Improvements

- Train on a larger English-Bengali parallel corpus.
- Add Bahdanau/Luong Attention.
- Experiment with GRU-based Seq2Seq.
- Replace the Seq2Seq architecture with a Transformer model.
