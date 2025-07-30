# law-chatbot-ai

LawChatbot AI is a powerful legal assistant built for Google Colab that leverages advanced Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG) to provide intelligent, document-grounded answers to questions based on Indian law.

This chatbot is designed to bridge the gap between complex legal documentation and everyday understanding. It processes real legal PDFs — including the Constitution of India, BNS, BNSS, BSA, Civil Procedure Code, and various Women & Child Protection Laws — and converts them into searchable, contextual knowledge through vector embeddings.

When a user asks a legal question, the system retrieves the most relevant sections from these laws using ChromaDB (a vector database), and then prompts a generative AI model (like Gemini, OpenAI, or Groq) to generate a precise, simplified, and law-aware response.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🧠 Why This Matters

Most people struggle to interpret legal documents due to their complexity, formality, and length. LawChatbot AI democratizes access to legal information by:

- 🧾 Simplifying legal jargon into everyday language
- 📖 Explaining laws contextually, referencing actual legal PDFs
- 🧑‍⚖️ Recommending the correct court based on the type and value of the case
- 🧠 Classifying the nature of a legal case from user input
- 🌐 Supporting multilingual input and voice accessibility (optional)

The goal is to empower students, activists, and the general public with easy access to legal insights, without needing prior legal training.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🔧 How It Works (Under the Hood)

1. PDF Loading & Parsing  
   Law PDFs are uploaded and processed using libraries like PyMuPDF or pdf2image.

2. Text Embedding & Storage  
   Parsed content is converted into dense vector embeddings using language model embeddings and stored in ChromaDB for fast semantic search.

3. User Question Handling  
   User enters a query in natural language. The system:
   - Searches the vector DB for the most relevant text snippets
   - Sends both the query and retrieved context to a selected LLM

4. LLM-Generated Answer  
   The LLM (Gemini, OpenAI, or Groq) generates a detailed, context-aware response grounded in law.

5. Optional Add-ons  
   - Case Classification: Determines if the case is civil, criminal, family, etc.
   - Court Suggestion: Recommends appropriate court type (e.g., Sessions, Family Court) based on dispute value and case type
   - Multilingual & Voice Input (future-ready)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🎯 Who Can Use This?
- 👩‍🎓 Students: for learning law practically
- 📢 NGOs/Legal Aid Groups: for spreading awareness
- 🧑‍💻 Developers & Researchers: as a prototype for AI + Law integration
- 🧑‍🤝‍🧑 General Public: to get easy answers without legal background


