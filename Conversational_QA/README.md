# Conversational RAG Chatbot with Memory
This is a RAG (Retrieval-Augmented Generation) chatbot built using LangChain.  
It uses a retriever to fetch relevant chunks from your documents and keeps track of the conversation using chat history — so follow-up questions actually make sense.

It runs in a Jupyter notebook for now, and it's meant to be a learning-friendly, working prototype.

---

## ✨ What It Does

- Retrieves relevant documents using `Chroma` and `HuggingFace` embeddings
- Uses `RunnableWithMessageHistory` to remember past messages per session
- Reformulates follow-up questions based on chat history
- Injects memory into the prompt automatically
- Uses a “create_stuff_documents_chain()” to pass all docs into a single prompt

