# 📚 Streamlit RAG with Groq

A lightweight **Retrieval-Augmented Generation (RAG)** application built with **Streamlit**, **Groq**, and **NumPy**. This project allows users to ingest custom text, generate lightweight vector embeddings, retrieve the most relevant context using cosine similarity, and obtain AI-powered answers from Groq's Llama 3.3 model.

---

## 🚀 Features

- 📄 Paste and process custom knowledge base
- ✂️ Automatic text chunking
- 🧠 Lightweight semantic embeddings (Pure Python + NumPy)
- 🔍 Cosine similarity-based document retrieval
- 🤖 AI-powered question answering using Groq Llama 3.3
- ⚡ Fast and interactive Streamlit interface
- 📚 Displays retrieved source chunks for transparency
- 🔒 Secure API key management with `.env`

---

## 🛠️ Tech Stack

- Python
- Streamlit
- Groq API
- NumPy
- Python Dotenv
- Regular Expressions (re)

---

## 📂 Project Structure

```
Streamlit-RAG-Groq/
│
├── app.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/streamlit-rag-groq.git

cd streamlit-rag-groq
```

---

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv .venv
```

Activate

```bash
.venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

or

```bash
pip install streamlit groq python-dotenv numpy
```

---

### 4. Configure Environment Variables

Create a `.env` file in the project root.

```env
GROQ_API_KEY=your_groq_api_key_here
```

---

### 5. Run the Application

```bash
streamlit run app.py
```

---

## 📦 Requirements

```text
streamlit
groq
python-dotenv
numpy
```

---

## 🧠 How It Works

### Step 1 — Knowledge Ingestion

Paste your text, meeting notes, documentation, or articles into the input area.

↓

### Step 2 — Text Chunking

The application automatically splits long text into manageable chunks.

↓

### Step 3 — Vector Embedding

Each chunk is converted into a lightweight semantic vector using a deterministic hash-based embedding approach.

↓

### Step 4 — Query Processing

When the user asks a question, the query is embedded into the same vector space.

↓

### Step 5 — Retrieval

Cosine similarity identifies the most relevant text chunks from the stored knowledge base.

↓

### Step 6 — AI Response Generation

The retrieved context is sent to Groq's **Llama 3.3-70B Versatile** model, which generates an answer based only on the retrieved information.

---

## 💡 Example Workflow

### Input Knowledge

```
Artificial Intelligence is transforming healthcare by improving diagnostics,
predictive analytics, and personalized medicine.
```

### User Question

```
How is AI used in healthcare?
```

### Retrieved Context

```
Artificial Intelligence is transforming healthcare by improving diagnostics,
predictive analytics, and personalized medicine.
```

### AI Response

```
According to the provided context, AI is used in healthcare to improve
diagnostics, predictive analytics, and personalized medicine.
```

---

## 🔐 Environment Variables

| Variable | Description |
|----------|-------------|
| GROQ_API_KEY | Your Groq API Key |

---

## 🎯 Future Improvements

- 📄 PDF document upload
- 📑 Multiple document support
- 🧠 SentenceTransformer embeddings
- 🗄️ ChromaDB / FAISS vector database integration
- 💬 Chat history and conversational memory
- 📁 File management
- 🌐 Web document ingestion
- 📊 Embedding visualization
- 🔍 Hybrid semantic + keyword search
- 🎨 Improved responsive UI

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```


---

## 👨‍💻 Author

**Nekkanti Jahnavi**

Computer Science Engineering Student

GitHub: https://github.com/your-username

---

## ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

Happy Coding! 🚀