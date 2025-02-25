#AI-Powered Q&A System

## 🚀 Overview
This project is a **hybrid Q&A system** that retrieves relevant documents and generates accurate responses using:

✅ **Hybrid Retrieval**: Combines **BM25 (Sparse)** + **ChromaDB (Dense)** for better search
✅ **Embeddings**: Uses **BAAI/bge-base-en** for high-quality vector representations
✅ **LLM Answering**: Uses **FLAN-T5-Large** for response generation
✅ **Dynamic Chunking**: Adjusts chunk size based on document length
✅ **Multi-File Support**: Handles **PDF and TXT** documents



## 🛠️ Installation & Setup
### **1️⃣ Install Dependencies**
```bash
pip install langchain chromadb sentence-transformers transformers rank_bm25 pypdf
```

### **2️⃣ Run the Script**
```bash
python main.py
```



##📂 How It Works
1. **Upload Documents**: Supports PDF & TXT files.
2. **Process & Index**: Chunks the documents, creates embeddings, and stores them in ChromaDB.
3. **Ask Questions**: Uses **hybrid retrieval** (BM25 + ChromaDB) to fetch relevant info.
4. **Generate Answers**: FLAN-T5 generates responses based on retrieved context.



##📌 Example input/output
```bash
💬 Ask a question (or type 'exit' to quit): Who is NEOV?

💡 Response: NEOV is a rapidly growing consulting firm operating across the African continent, specializing in the insurance and fintech sectors.
```


##📜 Future Improvements
- 🔄 **Support for more document types** (Word, HTML, md, ect..)
- 🤖 **Fine-tune the LLM for domain-specific answers**



