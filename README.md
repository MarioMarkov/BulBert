# Scripts to train BulBERT

### A LLM trained from scratch on bulgarian data.

#### The model and the model's tokenizer are trained _from scratch_ on bulgarian data from the **chitanka** dataset.

The notebook has the code to load the raw dataset and train the tokenizer from scratch from my huggingface-hub: *https://huggingface.co/datasets/mor40/chitanka_raw_document*

Or you can load the tokenized dataset from here and start training:
*https://huggingface.co/datasets/mor40/tokenized_chitanka*

The BERT config that it uses is this:
vocab_size=50265
max_position_embeddings=512
num_attention_heads=12
num_hidden_layers=6

It is trained for 3 epochs and gets -> Perplexity: 6.75 (on eval set)

The trained model you can find here: https://huggingface.co/mor40/BulBERT-chitanka-model
