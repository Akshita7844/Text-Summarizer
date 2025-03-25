# 🚀 Streamlining Text Summarization with Transformer Models

This repository showcases a powerful Python-based tool for **abstractive text summarization** using state-of-the-art **transformer models**. It allows you to scrape and summarize large blocks of web content with just a URL, using pre-trained models from the Hugging Face ecosystem.

---

## 📌 Overview

Text summarization condenses lengthy content into concise, meaningful summaries — and with **transformer-based models** like T5, BART, and PEGASUS, it's more coherent and context-aware than ever.

This project:
- Uses **Hugging Face Transformers** for summarization
- Extracts web text with **BeautifulSoup**
- Provides customizable summary parameters
- Preprocesses large texts into manageable chunks
- Outputs clear, controlled-length summaries

---

## 🧰 Libraries Used

- `transformers` – for pre-trained summarization pipelines  
- `bs4` – BeautifulSoup for web scraping  
- `requests` – for fetching web content  
- `pandas` – for structured text handling (optional)

---

## ✨ Key Features

🔎 **Web Scraping**  
Easily extract readable text from any article or blog using BeautifulSoup and Requests.

🧹 **Preprocessing & Chunking**  
Splits long texts intelligently into chunks suitable for transformer models.

🧠 **Transformer-based Summarization**  
Uses Hugging Face's summarization pipeline with models like T5/BART to generate concise, high-quality summaries.

⚙️ **Customizable Output**  
Control the minimum and maximum length of summaries via parameters.

📈 **Scalable**  
Efficiently handles large content—perfect for summarizing long-form research papers, news articles, or documentation.

---

## 🚀 Getting Started

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/transformer-summarizer.git
cd transformer-summarizer
```

2. **Install Dependencies**
```bash
pip install transformers beautifulsoup4 requests pandas
```

3. **Run the Script**

# launch the notebook
jupyter notebook Text summarisation.ipynb
```

---

## 💻 Example Usage

```python
from summarizer import summarize_url

url = "https://en.wikipedia.org/wiki/Natural_language_processing"
summary = summarize_url(url, max_length=200, min_length=60)
print(summary)
```

---

## 📎 Sample Output

> Natural language processing (NLP) is a subfield of linguistics, computer science, and artificial intelligence concerned with the interactions between computers and human language. It involves the development of algorithms and models that allow machines to understand, interpret, and generate human language.

---

## 🧠 Models Supported

- `t5-small`, `t5-base`, `t5-large`
- `facebook/bart-large-cnn`
- `google/pegasus-cnn_dailymail`  
*(Easily switch models via config)*

---

## 💬 Contribute

Found a bug or want to suggest a new feature? Open an issue or submit a pull request! Contributions are welcome.

---

## 🧪 Future Enhancements

- Streamlit UI for instant summarization via browser  
- Model selector dropdown  
- Multi-URL summarization pipeline  
- PDF/Text file summarization support

---

> Built with ❤️ using Transformers & Python
