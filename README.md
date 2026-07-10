# 🚀 Transformer Architectures and Applications

This repository demonstrates the implementation of the three fundamental Transformer architectures using **TensorFlow/Keras**. Each implementation is built from scratch to help understand how Transformers work internally and how they are applied to different Natural Language Processing (NLP) tasks.

---

# 📖 What is a Transformer?

A **Transformer** is a deep learning architecture introduced in the paper **"Attention Is All You Need" (2017)**. Unlike RNNs and LSTMs, Transformers process all words in a sequence simultaneously using the **Attention Mechanism**, allowing them to capture long-range dependencies efficiently.

Today, Transformer architectures power state-of-the-art AI models such as **BERT, GPT, T5, LLaMA, and Gemini**.

---

# 🏗️ Transformer Architectures

Transformers are mainly divided into three architectures based on their application.

| Architecture        | Purpose                             | Popular Models                 |
| ------------------- | ----------------------------------- | ------------------------------ |
| **Encoder-Only**    | Understands and analyzes input text | BERT, RoBERTa                  |
| **Encoder-Decoder** | Converts one sequence into another  | Original Transformer, T5, BART |
| **Decoder-Only**    | Generates text one token at a time  | GPT, LLaMA                     |

---

# 📂 Repository Structure

```
Transformer-Architectures-and-Applications/

├── Encoder-Only/
├── Encoder-Decoder/
├── Decoder-Only/
└── README.md
```

---

# 1️⃣ Encoder-Only Transformer

### Application

**Sentiment Classification**

### Description

This implementation demonstrates how an **Encoder-Only Transformer** processes an input sentence and predicts whether its sentiment is **Positive** or **Negative**.

### Workflow

* Creates a sentiment dataset.
* Converts text into numerical tokens.
* Generates token embeddings and positional embeddings.
* Applies Multi-Head Self-Attention.
* Processes features using a Transformer Encoder block.
* Performs binary classification using a Dense output layer.
* Predicts sentiment for unseen sentences.

### Concepts Covered

* Text Vectorization
* Token Embedding
* Positional Encoding
* Multi-Head Self-Attention
* Feed Forward Network
* Layer Normalization
* Binary Classification

---

# 2️⃣ Encoder-Decoder Transformer

### Application

**English to Marathi Neural Machine Translation**

### Description

This implementation demonstrates the complete Transformer architecture where the **Encoder** understands the English sentence and the **Decoder** generates the translated Marathi sentence one word at a time.

### Workflow

* Creates a parallel English-Marathi dataset.
* Tokenizes both source and target languages.
* Adds Start and End tokens for decoding.
* Builds Encoder and Decoder embedding layers.
* Processes input using the Transformer Encoder.
* Generates output using Masked Self-Attention and Cross Attention.
* Produces translated sentences through autoregressive decoding.

### Concepts Covered

* Sequence-to-Sequence Learning
* Encoder
* Decoder
* Masked Self-Attention
* Cross Attention
* Teacher Forcing
* Greedy Decoding

---

# 3️⃣ Decoder-Only Transformer

### Application

**GPT-style Text Generation**

### Description

This implementation demonstrates how a **Decoder-Only Transformer** predicts the next word using previous context and generates text autoregressively.

### Workflow

* Creates a text dataset.
* Converts sentences into token sequences.
* Prepares input-target pairs for next-word prediction.
* Generates token and positional embeddings.
* Applies Masked Self-Attention using a causal mask.
* Trains the model to predict the next token.
* Generates complete text by repeatedly predicting the next word.

### Concepts Covered

* Next Word Prediction
* Causal Mask
* Masked Self-Attention
* Decoder Block
* Autoregressive Text Generation

---

# 🛠️ Technologies Used

* Python
* TensorFlow
* Keras
* NumPy

---

# ▶️ Run the Project

Install the required packages:

```bash
pip install -r requirements.txt
```

Run any implementation:

```bash
python transformer_encoder_only.py
```

```bash
python transformer_encoder_decoder.py
```

```bash
python transformer_decoder_only.py
```

---

# 🎯 Learning Outcomes

After exploring these implementations, you will understand:

* The working principles of Transformer architectures.
* The differences between Encoder-Only, Encoder-Decoder, and Decoder-Only models.
* How attention mechanisms enable efficient sequence processing.
* How Transformers are applied to classification, translation, and text generation tasks.
