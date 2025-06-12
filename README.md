## 💬 RAG-based Personal Story Chatbot

A Retrieval-Augmented Generation (RAG) chatbot that interacts with my personal story! It uses OpenAI embeddings and FAISS for intelligent search and GPT for generating responses — all wrapped in a simple Streamlit app.

---

## 🔍 Features
- **RAG Architecture**: Retrieval + Generation using vector similarity
- **Custom Dataset**: Trained on my personal story, chunked semantically
- **FAISS Vector DB**: Fast, efficient retrieval of relevant text
- **OpenAI Embeddings**: `text-embedding-ada-002` for high-quality vectorization
- **Streamlit UI**: Clean and interactive chat interface

---

## 🧠 How It Works
1. **Preprocessing**: The story is split into meaningful chunks (e.g., scenes or paragraphs)
2. **Embedding**: Each chunk is converted into a vector using OpenAI’s embedding model
3. **Storage**: Vectors are stored in a FAISS index for fast similarity search
4. **Query**: User input is embedded and the most similar chunks are retrieved
5. **Generation**: GPT generates a response using the retrieved chunks as context

---

## 🛠️ Tech Stack
- Python
- OpenAI API (Embeddings + GPT)
- FAISS (Vector Search)
- NLP (Text preprocessing, chunking)
- Streamlit (Web UI)

---

## 🚀 Run Locally

```bash
git clone https://github.com/yourusername/rag_based_app.git
cd rag-story-chatbot
pip install -r requirements.txt
streamlit run app.py
