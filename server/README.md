# 📚 CISI Search API with Flask & Elasticsearch

This project provides a RESTful API for searching and retrieving documents from the **CISI dataset**, using **Elasticsearch** for indexing and **Flask** as the web framework. It includes search, autocomplete, and document retrieval functionalities, with a modular and production-ready architecture.

---

## 🚀 Features

- 🔍 **Search**: Multi-field text search across `title`, `text`, and `author` with fuzzy matching and highlight support.
- ✨ **Autocomplete**: Phrase prefix matching to simulate autocomplete behavior.
- 📄 **Document Retrieval**: Fetch document details by document ID.
- 🧠 **NLP Preprocessing**: Tokenization, lowercasing, stopword removal, punctuation filtering using NLTK.

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Ghassan-Dib/Search-Engine-System.git
cd es-cisi
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Environment Variables
```bash
ES_HOST=<your-elasticsearch-host>
ES_API_KEY=<your-elasticsearch-api-key>
```


###  ⚙️ Running the App
```bash
python run.py
```

---

## 📡 API Endpoints

### 🔍 Search
```bash
GET /api/search/?q=<query>&size=<optional: number of results>
```

### 🔤 Autocomplete
```bash
GET /api/search/autocomplete?q=<query>&size=<optional: number of suggestions>
```

### 📄 Document by ID
```bash
GET /api/document/<id>
```
