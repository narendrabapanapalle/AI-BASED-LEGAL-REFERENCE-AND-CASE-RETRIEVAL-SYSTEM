# ⚖️ AI Legal Reference and Case Retrieval System

<div align="center">

![Legal AI Banner](https://img.shields.io/badge/AI-Legal%20Research-gold?style=for-the-badge&logo=scales&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-121212?style=for-the-badge&logo=chainlink&logoColor=white)

**Your AI-Powered Legal Research Assistant**

[Features](#-features) • [Tech Stack](#-tech-stack) • [Architecture](#-architecture) • [Installation](#-installation) • [Usage](#-usage) • [Screenshots](#-screenshots)

</div>

---

## 📋 Overview

An intelligent, full-stack AI-powered legal research platform designed to revolutionize how legal professionals conduct case research and document retrieval. Built during my internship at **Infosys** (August 2025 - October 2025), this system leverages cutting-edge RAG (Retrieval-Augmented Generation) technology to provide context-aware answers to complex legal queries.

### 🎯 Problem Statement

Legal professionals spend countless hours searching through case law, statutes, and legal documents. This system streamlines that process by providing:
- ⚡ **Instant Access** to relevant legal information
- 🎓 **Context-Aware Responses** using advanced AI
- 📚 **Comprehensive Citations** for legal accuracy
- 💬 **Conversational Interface** for natural queries

---

## ✨ Features

### 🔐 Authentication & User Management
- **Secure Registration System** with password encryption
- **User Authentication** with session management via SQLite
- **Profile Management** with customizable profile pictures
- **Persistent Chat History** for each user session

### 🤖 AI-Powered Legal Research
- **Retrieval-Augmented Generation (RAG)** pipeline using LangChain
- **Semantic Search** with Sentence-Transformers for accurate information retrieval
- **Pinecone Vector Database** for efficient similarity search
- **OpenAI GPT-3.5-Turbo** integration for intelligent response generation
- **Context-Aware Answers** specific to legal domains (Indian Constitution, case law, etc.)

### 💻 User Interface
- **Modern, Responsive Design** with Streamlit
- **Interactive Chat Interface** with real-time responses
- **Conversation History** with delete functionality
- **Profile Customization** with image upload support
- **Professional Legal Theme** with law-themed aesthetics

### 🔒 Security Features
- **Password Hashing** for secure credential storage
- **Session Management** for authenticated access
- **SQLite Database** for reliable data persistence
- **User Isolation** - each user's data remains private

---

## 🛠️ Tech Stack

### **Frontend**
- **Streamlit** - Interactive web interface
- **Custom CSS** - Professional styling and animations
- **HTML/CSS** - Enhanced UI components

### **Backend**
- **Python 3.8+** - Core programming language
- **SQLite** - Lightweight, serverless database
- **File Handling** - Profile picture management

### **AI/ML**
- **LangChain** - RAG pipeline orchestration
- **OpenAI GPT-3.5-Turbo** - Natural language generation
- **Sentence-Transformers** - Semantic embeddings
- **Pinecone** - Vector database for similarity search

### **Libraries & Tools**
```
streamlit
langchain
openai
sentence-transformers
pinecone-client
sqlite3
bcrypt/hashlib
Pillow
```

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INTERFACE (Streamlit)                │
│  ┌──────────┐  ┌──────────┐  ┌───────────┐  ┌───────────┐  │
│  │  Login   │  │ Register │  │ Dashboard │  │  Profile  │  │
│  └──────────┘  └──────────┘  └───────────┘  └───────────┘  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                   AUTHENTICATION LAYER                       │
│              (SQLite Database + Session Management)          │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                        RAG PIPELINE                          │
│  ┌──────────────────────────────────────────────────────┐   │
│  │  User Query → Sentence Transformers (Embeddings)     │   │
│  └──────────────────────────────────────────────────────┘   │
│                              │                               │
│                              ▼                               │
│  ┌──────────────────────────────────────────────────────┐   │
│  │  Pinecone Vector DB (Semantic Search)                │   │
│  └──────────────────────────────────────────────────────┘   │
│                              │                               │
│                              ▼                               │
│  ┌──────────────────────────────────────────────────────┐   │
│  │  Retrieved Context + Query → OpenAI GPT-3.5-Turbo    │   │
│  └──────────────────────────────────────────────────────┘   │
│                              │                               │
│                              ▼                               │
│  ┌──────────────────────────────────────────────────────┐   │
│  │  Context-Aware Legal Response with Citations         │   │
│  └──────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

---

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager
- OpenAI API key
- Pinecone API key

### Step-by-Step Setup

1. **Clone the repository**
```bash
git clone https://github.com/narendrabapanapalle/AI-BASED-LEGAL-REFERENCE-AND-CASE-RETRIEVAL-SYSTEM.git
cd AI-BASED-LEGAL-REFERENCE-AND-CASE-RETRIEVAL-SYSTEM
```

2. **Create a virtual environment**
```bash
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Set up environment variables**
Create a `.env` file in the root directory:
```env
OPENAI_API_KEY=your_openai_api_key_here
PINECONE_API_KEY=your_pinecone_api_key_here
PINECONE_ENVIRONMENT=your_pinecone_environment
PINECONE_INDEX_NAME=legal-cases
```

5. **Run the application**
```bash
streamlit run app.py
```

The application will open in your browser at `http://localhost:8501`

---

## 📖 Usage

### 1. **Registration**
- Navigate to the registration page
- Fill in your details (First Name, Last Name, Email, Password)
- Optionally upload a profile picture
- Click "Create Account"

### 2. **Login**
- Enter your registered email and password
- Click "Sign In" to access the dashboard

### 3. **Legal Research**
- Type your legal question in the chat interface
- Examples:
  - "What is Article 15 of the Indian Constitution?"
  - "What does Article 21 guarantee?"
  - "Explain the difference between Article 15 and Article 16"
- Receive AI-generated responses with proper legal context

### 4. **Profile Management**
- Click "View Profile" from the sidebar
- Update your information or profile picture
- View your account details and member since date

### 5. **Chat History**
- Access previous conversations
- Delete chat history when needed
- Each session is saved automatically

---

## 📸 Screenshots

> **Note**: Add your screenshots to the `/screenshots/` folder in your repository and they will display below.

### 🔐 Authentication Pages

#### Login Page
![Login Page](screenshots/01-login.png)
- Clean, professional interface with legal theme
- Secure authentication system
- Password visibility toggle
- Quick access to registration

#### Registration Page
![Registration Page](screenshots/02-register.png)
- User-friendly registration form
- Profile picture upload (optional)
- Password confirmation
- File size limits (200MB for PNG, JPG, JPEG)

### 💬 Dashboard

#### Main Chat Interface
![Dashboard](screenshots/03-dashboard.png)
- Conversational AI assistant (LegalBot)
- Real-time response generation
- Clean message display with user/bot differentiation
- Persistent chat history

#### Legal Q&A Examples
![Chat Interface](screenshots/04-chat-interface.png)

**Example Queries and Responses:**

- **Question**: "What is Article 15 of the Indian Constitution?"
  - **Response**: Detailed explanation of Article 15, covering prohibition of discrimination on grounds of religion, race, caste, sex, or place of birth
  
- **Question**: "What does Article 21 guarantee?"
  - **Response**: Comprehensive answer on the right to life and personal liberty, with reference to procedure established by law

### 👤 Profile Section

#### User Profile View
![User Profile](screenshots/05-profile.png)
- Display of user information (name, email, member since)
- Profile picture display
- Back navigation to dashboard

#### Profile Update
![Profile Update](screenshots/06-profile-update.png)
- Editable first name and last name
- Email display (non-editable)
- Password change option
- Profile picture update with drag-and-drop
- Real-time validation

---

## 🎯 Key Achievements

### Performance Metrics
- ⚡ **Sub-second Response Time** for most queries
- 🎯 **High Accuracy** in legal information retrieval
- 💾 **Efficient Storage** with SQLite database
- 🔒 **100% Secure** authentication system

### Technical Innovations
- **Semantic Search Implementation** using state-of-the-art transformers
- **RAG Pipeline** for context-aware generation
- **Scalable Architecture** ready for production deployment
- **User-Centric Design** focusing on legal professional needs

---

## 🔮 Future Enhancements

- [ ] **Multi-language Support** for regional languages
- [ ] **Document Upload** for case file analysis
- [ ] **Advanced Filters** for case law search (by date, jurisdiction, etc.)
- [ ] **Export Functionality** for research reports
- [ ] **Collaborative Features** for team research
- [ ] **Mobile Application** for on-the-go access
- [ ] **Integration with Legal Databases** (e.g., Indian Kanoon, SCC Online)
- [ ] **Citation Verification** system
- [ ] **Case Law Timeline** visualization

---

## 📊 Project Structure

```
AI-BASED-LEGAL-REFERENCE-AND-CASE-RETRIEVAL-SYSTEM/
│
├── app.py                      # Main Streamlit application
├── requirements.txt            # Python dependencies
├── .env.example               # Environment variables template
├── .gitignore                 # Git ignore file
├── README.md                  # Project documentation
│
├── screenshots/               # Application screenshots (for README)
│   ├── 01-login.png
│   ├── 02-register.png
│   ├── 03-dashboard.png
│   ├── 04-chat-interface.png
│   ├── 05-profile.png
│   └── 06-profile-update.png
│
├── data/                      # Legal documents and data
│   └── legal_database.db      # SQLite database
│
└── uploads/                   # User uploaded files
    └── profile_pictures/      # User profile images
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project was developed during my internship at Infosys (August 2025 - October 2025).

---

## 👤 Author

**Narendra Bapanapalle**
- LinkedIn: [Narendra Bapanapalle](https://linkedin.com/in/narendra-bapanapalle)
- GitHub: [@narendrabapanapalle](https://github.com/narendrabapanapalle)
- Email: Contact via GitHub

---

## 🙏 Acknowledgments

- **Infosys** for the internship opportunity
- **OpenAI** for GPT-3.5-Turbo API
- **Pinecone** for vector database services
- **Streamlit** for the amazing web framework
- **LangChain** community for RAG implementation guidance

---

<div align="center">

**⚖️ Built with passion for legal technology innovation ⚖️**

Made with ❤️ during Infosys Internship 2025

</div>
