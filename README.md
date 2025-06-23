# Amharic E-commerce Data Extractor

This project scrapes e-commerce messages from Ethiopian Telegram channels, preprocesses the Amharic text, and prepares data for Named Entity Recognition (NER) fine-tuning.

## 📦 Project Structure

- `scrape_telegram.py` - Scrapes messages from selected Telegram channels.
- `preprocess_data.py` - Cleans and tokenizes raw messages.
- `label_data_to_conll.py` - Interactive CLI tool for labeling tokens in CoNLL format.
- `raw_telegram_data.json` - Raw scraped data.
- `preprocessed_data.csv` - Cleaned and tokenized data.
- `labeled_data.conll` - Manually labeled dataset for NER.

## 🧪 Task Objectives

### ✅ Task 1: Data Ingestion & Preprocessing
- Collect messages from 20+ Ethiopian Telegram channels.
- Preprocess text by normalizing, tokenizing, and cleaning.
- Save structured message data with metadata.

### ✅ Task 2: Label Data in CoNLL Format
- Load preprocessed messages.
- Manually annotate 30–50 messages with `B-Product`, `B-PRICE`, `B-LOC`, etc.
- Save in standard CoNLL format for model fine-tuning.

## 📋 How to Run

### 1. Clone the repository and install requirements
```bash
git clone https://github.com/RuhamaY/Amharic-E-commerce-Data-Extractor.git
cd amharic-ner-telegram
pip install -r requirements.txt
````

### 2. Scrape Telegram Messages

```bash
python scrape_telegram.py
```

### 3. Preprocess Messages

```bash
python preprocess_data.py
```

### 4. Label Tokens in CoNLL Format

```bash
python label_data_to_conll.py
```

---