# 📚 Chat with your PDF App

A simple yet powerful web-based chatbot that **enables users to interact with their own PDF documents using natural language**. Powered by OpenAI's GPT models and enhanced with Retrieval-Augmented Generation (RAG) capabilities, the chatbot understands context from user-uploaded PDFs and answers questions accurately and concisely.

It features vector storage with FAISS, and history-aware memory, making the experience more conversational and contextually intelligent. The app is built with Streamlit, providing an intuitive and responsive user interface for seamless interactions.

---

## 🚀 Features

- PDF Upload & Parsing: Upload single or multiple PDFs and automatically extract structured content using `PyPDFLoader`.
- Text Chunking: Split documents using `RecursiveCharacterTextSplitter` for improved retrieval accuracy.
- FAISS Vector Store: Store and retrieve document embeddings for fast similarity search.
- OpenAI-powered QA: Answer user questions by combining document knowledge and GPT responses via LangChain’s QA chain.
- Chat History Memory: Maintain per-session conversation history using `RunnableWithMessageHistory` and `InMemoryChatMessageHistory`.
- Streamlit UI: Clean sidebar for uploading PDFs, and chat-like interface for asking questions and viewing responses.

---

## 🧑‍💻 How to Use

1. 👉 Go to the app: **[Click here to open the app](https://chat-with-your-pdf.streamlit.app/)**
2. 📄 Upload your PDF file
3. ✅ Wait for the document to be processed, util the text box to ask questions is displayed
4. ❓ Ask question about your PDF, and wait the answer
5. ↪️ You can even ask follow up question, See the message log in the side bar, and restart the session

---

## 💻 Run Locally

1. Clone the repository
```bash
git clone https://github.com/roissyahf/chat-with-your-pdf.git
cd chat-with-your-pdf
```
2. Create virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Create API Key

Visit https://platform.openai.com/api-keys to get OPENAI API KEY, then placed inside `.env` for security reason

5. Run the Streamlit app
```bash
streamlit run app.py
```


