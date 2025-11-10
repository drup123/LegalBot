# LegalBot

**LegalBot** is an intelligent legal chatbot designed to provide information on Indian law, with a special focus on the Indian Penal Code (IPC) and Department of Justice (DoJ) services.

It leverages modern AI models and Retrieval-Augmented Generation (RAG) to provide context-aware, accurate, and multi-lingual legal information.

## 🚀 Features

* **Dual-Mode Operation:**
    * **Online Mode:** Utilizes the Google Gemini 1.5 (Flash/Pro) model for high-quality, real-time responses.
    * **Offline Mode:** Designed to work with local models via `ChatOllama` (e.g., `phi3`) for privacy and offline access (Note: This feature is not fully implemented in the provided code).
* **Retrieval-Augmented Generation (RAG):** Employs a `FAISS` vector store and specialized `law-ai/InLegalBERT` embeddings to retrieve relevant legal documents, ensuring answers are contextually grounded in legal texts.
* **Multi-language Support:** Built-in translation using `deep_translator` supports a wide variety of Indian languages, including Hindi, Bengali, Tamil, Telugu, Marathi, and more.
* **Interactive UI:** A user-friendly, real-time chat interface built with Streamlit, complete with chat history and a conversation reset button.
* **Standalone API Service:** Includes a separate Flask backend (`chatbot_api.py`) that serves the Gemini model via a simple REST API.

## 🛠️ Technology Stack

* **Frontend (Main App):** Streamlit
* **API Service:** Flask, Flask-CORS
* **AI Models:** Google Generative AI (Gemini 1.5 Flash/Pro), Ollama (phi3)
* **NLP & Embeddings:** LangChain, Hugging Face Transformers (`law-ai/InLegalBERT`)
* **Vector Store:** FAISS (`faiss-cpu`)
* **Translation:** `deep-translator`
* **Configuration:** `python-dotenv`

