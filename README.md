# Medical Chatbot

A web-based AI chatbot that answers medical queries using **LangChain**, **OpenAI**, **Pinecone**, and **Flask**. It retrieves context from medical documents and generates accurate, conversational responses.

## ⚙️ Tech Stack

* **Backend:** Python, Flask
* **AI/LLM:** OpenAI GPT models
* **Vector DB:** Pinecone
* **Framework:** LangChain
* **Deployment:** Docker, AWS

## 🚀 Setup

```bash
git clone https://github.com/Kushagra001/Medical-Chatbot.git
cd Medical-Chatbot
pip install -r requirements.txt
```

Create a `.env` file:

```
OPENAI_API_KEY=your_openai_api_key
PINECONE_API_KEY=your_pinecone_api_key
```

Build and store embeddings:

```bash
python store_index.py
```

Run the app:

```bash
python app.py
```

Visit `http://localhost:8080` to use the chatbot.

## 🧠 How It Works

1. Medical documents are converted into vector embeddings using LangChain.
2. Embeddings are stored in Pinecone for semantic search.
3. On user query, the system retrieves relevant context and generates an LLM-based answer via OpenAI API.

## 📄 License

Licensed under the **Apache License 2.0**.
