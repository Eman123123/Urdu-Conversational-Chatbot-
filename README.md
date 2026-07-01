# Urdu-Conversational-Chatbot-
# 📋 Overview
A Transformer-based Conversational Chatbot for Urdu Language

This project implements an end-to-end Urdu Conversational Chatbot using a Transformer architecture with SentencePiece tokenization. The model is trained on a large Urdu corpus to generate contextually relevant responses in a conversational setting.

# 🎯 Key Features
Feature	Description
1. 🗣️ Urdu Language Support	Complete conversational understanding and generation in Urdu


1.🔄 Transformer Architecture	Encoder-decoder model with multi-head attention


1.📝 Subword Tokenization	SentencePiece tokenizer for efficient Urdu text processing


1.🎨 Interactive UI	Gradio-based web interface for easy interaction


1.📊 Comprehensive Evaluation	BLEU, ROUGE-L, and chrF metrics


1.🎯 Advanced Decoding	Top-k and top-p sampling with temperature control


1.💾 Model Persistence	Save and load trained models seamlessly


1.🚀 GPU Support	Optimized for CUDA-enabled training
# 🏗️ Architecture
Model Details
Component	Configuration
Model Type	Transformer Encoder-Decoder
Embedding Dimension	512
Number of Heads	8
Encoder Layers	4
Decoder Layers	4
Feed-forward Dimension	2048
Dropout Rate	0.1
Vocab Size	6,918 (configurable)
Max Sequence Length	64
Total Parameters	~15M
Training Configuration
Parameter	Value
Training Samples	19,994 conversational pairs
Batch Size	32
Epochs	20
Learning Rate	3e-4
Optimizer	Adam
Loss Function	Cross-Entropy Loss
Device	GPU (CUDA)
# 📊 Dataset
The project uses a large Urdu corpus containing over 19,995 sentences for training the conversational model.
Dataset Statistics
Metric	Value
Total Sentences	19,995
Conversational Pairs	19,994
Language	Urdu
Text Normalization	Diacritic removal, character normalization
Min Sentence Length	3 characters
Max Sentence Length	300 characters
Data Format	TSV (Tab-separated values)
# Preprocessing Pipeline
Text Normalization: Standardize Urdu script (remove diacritics, normalize characters)

Tokenization: SentencePiece subword tokenization (unigram model)

Sequence Formatting: Add CLS and SEP tokens

Padding: Uniform sequence length for batching

Pair Creation: Consecutive sentences form conversational pairs

