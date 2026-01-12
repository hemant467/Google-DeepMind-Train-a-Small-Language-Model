# Google DeepMind Train a Small Language Model 💠
Character-level Arabic language model 🤖 for generating simple, coherent stories using n-gram and transformer-based approaches.

# Overview 📜 :

Cymbal Chat is a startup-focused project designed to develop a character-level language model for generating simple, coherent stories in Arabic. This repository contains the foundational tools and data preparation framework for training custom, small-scale transformer models for Arabic NLP tasks.

Character-based models can offer better performance than word-based models for languages like Arabic, where morphology and word composition are complex. This project provides a starting point for creating robust, specialized language models tailored to Arabic text generation.

# Features ✨ :

- Character-level Tokenizer: Efficiently encodes Arabic text at the character level for model training.
- N-gram Text Generator: Provides a baseline generative model for Arabic story generation.
- Data Preparation Pipeline: Prepares raw Arabic text for training character-based transformer models.
- Extensible Codebase: Easy to extend for custom datasets and advanced model architectures.

# Project Structure 🏗️ :
```text
cymbal-chat-arabic/
│
├── data/
│   ├── raw/            # Original Arabic story datasets
│   └── processed/      # Tokenized and cleaned datasets ready for training
│
├── notebooks/          # Jupyter notebooks for experimentation
│
├── src/
│   ├── tokenizer.py     # Character-level tokenizer implementation
│   ├── ngram_model.py  # N-gram text generator
│   └── prepare_data.py # Data preparation pipeline
│
├── scripts/            # Training and evaluation scripts
│
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

Usage
1. Prepare the Dataset

Place your Arabic story dataset in data/raw/ and run the preprocessing script:

```bash
python src/prepare_data.py --input_dir data/raw --output_dir data/processed
```

2. Train the N-gram Baseline Model 🤖

```bash
python src/ngram_model.py --data_path data/processed/stories.txt --n 3
```

3. Tokenize Text for Transformer Model 🤖

```bash
python src/tokenizer.py --input data/processed/stories.txt --output data/processed/tokenized.npy
```

<img src="https://readme-typing-svg.herokuapp.com/?lines=Google+DeepMind+Train+a+Small+Language+Model+💠&font=Fira%20Code&color=%23FFD700&center=true&width=600&height=60">
