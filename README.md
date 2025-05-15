# nmt-english-hindi-seq2seq-tf2
A TensorFlow 2.x implementation of a neural machine translation system using a sequence-to-sequence (seq2seq) model with GRUs, translating from English to Hindi.

# Neural Machine Translation (English → Hindi) using TensorFlow 2.x

This project implements a **Neural Machine Translation (NMT)** model for translating English sentences into Hindi using a **Sequence-to-Sequence (Seq2Seq)** architecture with GRU-based encoder and decoder layers. The model is trained and evaluated on the [WAT Indic Languages Corpus](http://lotus.kuee.kyoto-u.ac.jp/WAT/indic-multilingual/).

---

## 📌 Features

- Custom implementation of Encoder-Decoder using TensorFlow 2.x
- Support for Indic languages using `indic-nlp-library`
- Preprocessing pipeline with tokenization, cleaning, padding
- Teacher Forcing during training
- Greedy decoding at inference time
- Evaluation using BLEU score

---

## 🧠 Model Architecture

### Encoder
- Embedding layer
- GRU (1024 units)
- Outputs sequence and final hidden state

### Decoder
- Embedding layer
- GRU (1024 units)
- Dense layer for output vocabulary prediction

---

## 📦 Dataset

Download the dataset:

```bash
wget "http://lotus.kuee.kyoto-u.ac.jp/WAT/indic-multilingual/indic_languages_corpus.tar.gz"
