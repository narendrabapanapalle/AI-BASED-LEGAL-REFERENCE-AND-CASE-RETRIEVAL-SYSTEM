# ⚖️ AI Legal Reference and Case Retrieval System

## 📌 Overview
**AI Legal Reference and Case Retrieval System** is an intelligent **AI-powered legal research assistant** designed to provide legal professionals with a **conversational interface for case research and document retrieval**. The platform enables users to **query legal documents, case laws, and constitutional articles using natural language**, delivering accurate and contextually relevant legal information instantly.

Developed during my **internship at Infosys (August 2025 - October 2025)** using **Python, Streamlit, LangChain, and OpenAI GPT-3.5-Turbo** for the **frontend and AI processing**, along with **Sentence-Transformers and Pinecone vector database** for **semantic search**, and **SQLite for secure backend management**, this system ensures **precision, efficiency, and reliable legal research support**.
<br>

---

<br>

![Login Page](https://github.com/user-attachments/assets/645063ab-56af-4159-9689-da67af079ca3)

---

## 🎯 Features
✅ **Secure User Authentication**
- **User Login/Register:** Secure access for legal professionals and researchers.
- **Profile Management:** Update personal information and manage account settings.

✅ **Natural Language Legal Queries** – Ask complex legal questions in plain English and receive context-aware answers.

✅ **Retrieval-Augmented Generation (RAG)** – Integrated LangChain with OpenAI GPT-3.5-Turbo to deliver precise, citation-backed legal responses.

✅ **Efficient Semantic Search** – Implemented using Sentence-Transformers and Pinecone vector database for rapid and accurate information retrieval.

✅ **Case Law & Constitutional Research** – Access Indian Constitution articles, case precedents, and legal statutes.

✅ **Conversational Interface** – Interactive chat-based system with persistent chat history.

✅ **Secure Backend** – SQLite database manages user authentication, personalized sessions, and chat histories.

✅ **Professional UI/UX** – Clean, intuitive Streamlit-based interface designed for legal professionals.

---

## 🔧 Technologies Used
- **Frontend:** Streamlit, HTML, CSS  
- **AI/ML:** LangChain, OpenAI API (GPT-3.5-Turbo), Sentence-Transformers  
- **Vector Database:** Pinecone (for semantic search and embeddings)  
- **Database:** SQLite  
- **Backend:** Python  

---

## 🖼️ Screenshots of the Project

### 📌 Login Page
![Login Page](https://github.com/user-attachments/assets/645063ab-56af-4159-9689-da67af079ca3)
*Secure authentication portal for legal professionals*
<br><br>

---
### 📌 Registration Page
![Registration Page](https://github.com/user-attachments/assets/registration-placeholder)
*Create new account with profile picture upload*
<br><br>

---
### 📌 Main Dashboard
![Dashboard](https://github.com/user-attachments/assets/dashboard-placeholder)
*LegalBot main interface - Your AI Legal Research Assistant*
<br><br>

---
### 📌 Chat Interface with Sidebar
![Chat Interface](https://github.com/user-attachments/assets/chat-placeholder)
*User profile sidebar with chat management options*
<br><br>

---
### 📌 Legal Query Response
![Query Results](https://github.com/user-attachments/assets/query-placeholder)
*AI-powered answers with detailed legal explanations - Example: Article 15 of Indian Constitution*
<br><br>

---
### 📌 Multi-Turn Conversation
![Conversation Flow](https://github.com/user-attachments/assets/conversation-placeholder)
*Contextual follow-up questions and comprehensive legal research*
<br><br>

---
### 📌 User Profile Page
![User Profile](https://github.com/user-attachments/assets/profile-placeholder)
*View and manage profile information*
<br><br>

---
### 📌 Update Profile Page
![Update Profile](https://github.com/user-attachments/assets/update-profile-placeholder)
*Update personal information, profile picture, and password*
<br><br>

---
### 📌 About Section
![About Section](https://github.com/user-attachments/assets/about-placeholder)
*System information and capabilities overview*

<br>

## 🎓 Internship Highlights
**Company:** Infosys  
**Role:** Artificial Intelligence Intern  
**Duration:** August 2025 - October 2025  
**Mode:** Remote

### Key Achievements:
🔹 Developed a **full-stack AI Legal Reference and Case Retrieval System** from scratch  
🔹 Engineered a **Retrieval-Augmented Generation (RAG) pipeline** integrating LangChain with OpenAI GPT-3.5-Turbo  
🔹 Implemented **efficient semantic search functionality** using Sentence-Transformers and Pinecone vector database  
🔹 Designed a **secure SQLite-based backend** for user authentication and persistent chat histories  
🔹 Created an **intuitive conversational interface** for legal professionals to conduct research efficiently  
🔹 Successfully delivered **context-aware answers** to complex legal queries with proper citations

---

## 🚀 Future Plans
🔹 Integrate **Indian Penal Code (IPC) and other legal statutes** for comprehensive coverage.  
🔹 Add **case law citation** with hyperlinks to original documents.  
🔹 Implement **document upload feature** for analyzing custom legal documents.  
🔹 Develop **advanced search filters** by date, jurisdiction, and case type.  
🔹 Add **voice-based queries** using speech recognition technology.  
🔹 Create **comparison feature** for analyzing multiple case laws simultaneously.  
🔹 Integrate **real-time legal updates** and amendments tracking.  
🔹 Expand to include **international legal frameworks** and comparative law research.

💡 **Stay tuned for updates!** 🎉

---

## 📖 How It Works
1. **User Authentication:** Legal professionals register and log in securely
2. **Document Processing:** Legal documents are preprocessed and converted into vector embeddings
3. **Vector Storage:** Embeddings are stored in Pinecone vector database for efficient retrieval
4. **Query Input:** Users ask legal questions in natural language through the chat interface
5. **Semantic Search:** System searches for relevant legal information using Sentence-Transformers
6. **RAG Pipeline:** Retrieved documents are passed to GPT-3.5-Turbo for generating contextual answers
7. **Response Delivery:** Users receive accurate, citation-backed legal information instantly
8. **Chat History:** All conversations are saved for future reference

---

## 🛠️ Installation & Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/ai-legal-reference-system.git
cd ai-legal-reference-system

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
# Create a .env file with:
# OPENAI_API_KEY=your_openai_key
# PINECONE_API_KEY=your_pinecone_key


# Run the application
streamlit run app.py
```

---

## 📊 System Architecture
```
User Input → Streamlit UI → Query Processing
                ↓
         Sentence-Transformers
                ↓
         Pinecone Vector Search
                ↓
    Retrieved Legal Documents
                ↓
         LangChain + GPT-3.5
                ↓
    Context-Aware Response → Display to User
```

---

## 🔐 Security Features
- **Password Encryption:** Secure password hashing for user accounts
- **Session Management:** Protected user sessions with authentication tokens
- **Data Privacy:** User queries and chat histories stored securely in SQLite
- **Input Validation:** Sanitized inputs to prevent SQL injection and security vulnerabilities

---

## 📚 Legal Database Coverage
- ✅ **Indian Constitution** - Complete articles and amendments
- ✅ **Fundamental Rights** - Articles 12-35
- ✅ **Directive Principles** - Articles 36-51
- ✅ **Legal Procedures** - Criminal and Civil law procedures
- ✅ **Case Precedents** - Landmark judgments and citations

----

---

**Built with ⚖️ for smarter legal research | Developed during Infosys Internship 2025**
