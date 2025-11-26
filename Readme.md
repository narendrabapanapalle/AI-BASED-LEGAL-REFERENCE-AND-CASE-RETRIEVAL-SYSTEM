# ⚖️ AI Legal Reference and Case Retrieval System

## 📌 Overview
**AI Legal Reference and Case Retrieval System** is an intelligent **AI-powered legal research assistant** designed to provide legal professionals with a **conversational interface for case research and document retrieval**. The platform enables users to **query legal documents, case laws, and constitutional articles using natural language**, delivering accurate and contextually relevant legal information instantly.

Developed during my **internship at Infosys (August 2025 - October 2025)** using **Python, Streamlit, LangChain, and OpenAI GPT-3.5-Turbo** for the **frontend and AI processing**, along with **Sentence-Transformers and Pinecone vector database** for **semantic search**, and **SQLite for secure backend management**, this system ensures **precision, efficiency, and reliable legal research support**.
<br>

---

<br>


### 📌 Login Page
![WhatsApp Image 2025-10-22 at 20 48 48_2805e3d5](https://github.com/user-attachments/assets/2de0d499-9517-49c8-a869-e0f486737257)


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

### 📌 Registration Page
![WhatsApp Image 2025-10-22 at 20 49 39_b2a86a85](https://github.com/user-attachments/assets/4b613297-d47a-41ea-af73-76d4f711836c)
*Create new account with profile picture upload*
<br><br>

---
### 📌 Main Dashboard
![WhatsApp Image 2025-10-22 at 20 54 50_0f68a5bb](https://github.com/user-attachments/assets/ddea2b53-96ba-43ee-aa0e-b470e0512038)

*LegalBot main interface - Your AI Legal Research Assistant*
<br><br>

---
### 📌 Chat Interface with Sidebar
![WhatsApp Image 2025-10-22 at 20 57 54_940ff7c1](https://github.com/user-attachments/assets/46c1f200-d3a7-4acf-b81d-ebd53c97d61f)

*User profile sidebar with chat management options*
<br><br>

---
### 📌 Legal Query Response
![WhatsApp Image 2025-10-22 at 22 05 22_c776e6ad](https://github.com/user-attachments/assets/1ae95294-cf3a-42fb-98a0-af3c351a5131)

*AI-powered answers with detailed legal explanations - Example: Article 15 of Indian Constitution*
<br><br>

---
### 📌 Multi-Turn Conversation
![WhatsApp Image 2025-10-22 at 22 44 57_dc11bc19](https://github.com/user-attachments/assets/15482099-e213-48d7-985e-922116d3a99e)

*Contextual follow-up questions and comprehensive legal research*
<br><br>

---
### 📌 User Profile Page
![WhatsApp Image 2025-10-22 at 22 01 33_94af8571](https://github.com/user-attachments/assets/cffa1d9e-acc1-4f82-a3f9-866e49367d87)

*View and manage profile information*
<br><br>

---
### 📌 Update Profile Page
![WhatsApp Image 2025-10-22 at 22 02 50_b53243e5](https://github.com/user-attachments/assets/75f3f8a4-d41f-4a11-bb51-f2b8f311d35e)

*Update personal information, profile picture, and password*
<br><br>

---
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

##📚 Legal Database Coverage
Indian Acts & Laws:
Constitution of India | Indian Penal Code | Criminal Procedure Code (1973) | Civil Procedure Code (1908)
Contract Act (1872) | Evidence Act (1872) | Companies Act (2013) | Consumer Protection Act (2019)
Information Technology Act (2000) | Hindu Marriage Act | Special Marriage Act (1954)
Negotiable Instruments Act (1881) | Right to Information Act (2005) | Juvenile Justice Act
Case Laws:
Maneka Gandhi vs. Union of India | Navtej Singh Johar vs. Union of India | Shreya Singhal vs. U.O.I
Kesavananda Bharati vs. State of Kerala | Other landmark judgments and precedents
----

---

**Built with ⚖️ for smarter legal research | Developed during Infosys Internship 2025**
