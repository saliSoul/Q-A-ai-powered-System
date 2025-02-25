🚀 **Overview** :


This project is a **hybrid Q&A system** that retrieves relevant documents and generates accurate responses using:

1. **Hybrid Retrieval**: Combines **BM25 (Sparse)** + **ChromaDB (Dense)** for better search

2. **Embeddings**: Uses **BAAI/bge-base-en** for high-quality vector representations

3. **LLM Answering**: Uses **FLAN-T5-Large** for response generation

4. **Dynamic Chunking**: Adjusts chunk size based on document length

5. **Multi-File Support**: Handles **PDF and TXT** documents



🛠️ Installation & Setup
### **1️⃣ Install Dependencies**
```bash
pip install langchain chromadb sentence-transformers transformers rank_bm25 pypdf langchain-community huggingface_hub
```



📂 How It Works
1. **Upload Documents**: Supports PDF & TXT files. (Find the sample file NEOV.txt above)
2. **Process & Index**: Chunks the documents, creates embeddings, and stores them in ChromaDB.
3. **Ask Questions**: Uses **hybrid retrieval** (BM25 + ChromaDB) to fetch relevant info.
4. **Generate Answers**: FLAN-T5 generates responses based on retrieved context.



📌 Example input/output
```bash
💬 Ask a question (or type 'exit' to quit): Who is NEOV?

💡 Response: NEOV is a rapidly growing consulting firm operating across the African continent, specializing in the insurance and fintech sectors.
```

**LIVE DEMO** : YOU CAN FIND THE LIVE DEMO HERE  = https://www.dropbox.com/scl/fi/91ezoblduidxyn2vfb6f1/LIVE-DEMO-QA-SYSTEM.mov?rlkey=9lfj162wgfr6d5r2edr16i814&st=903tau12&dl=0


📜 Future Improvements
- 🔄 **Support for more document types** (Word, HTML, md, ect..)
- 🤖 **Fine-tune the LLM for domain-specific answers**



