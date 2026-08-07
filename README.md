# AI-Financial-Assistant-Azentio
AI Financial Assistant using RAG, Google Gemini API, FAISS, Role-Based Access Control, and Gradio.

# 📊 AI Financial Assistant

<p align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Google Gemini](https://img.shields.io/badge/Google-Gemini_API-orange?logo=google)
![FAISS](https://img.shields.io/badge/FAISS-Vector_DB-green)
![Gradio](https://img.shields.io/badge/Gradio-Web_UI-red)
![License](https://img.shields.io/badge/License-MIT-yellow)

An AI-powered Financial Assistant that answers questions from financial reports using **Retrieval-Augmented Generation (RAG)**, **Google Gemini API**, **FAISS**, and **Role-Based Access Control (RBAC)**.

</p>

---

# 🚀 Features

✅ Financial PDF Ingestion

✅ Financial Table Extraction

✅ Excel Generation

✅ Text Chunking

✅ Sentence Transformer Embeddings

✅ FAISS Vector Database

✅ Retrieval-Augmented Generation (RAG)

✅ Google Gemini API

✅ Role-Based Access Control

✅ Feedback Collection

✅ Interactive Gradio Web Interface

---

# 🏗️ Project Architecture

```
                      Financial Report (PDF)
                               │
                               ▼
                     PDF Text Extraction
                               │
                               ▼
                      Financial Tables
                               │
                               ▼
                       Text Chunking
                               │
                               ▼
                 Sentence Transformer Embeddings
                               │
                               ▼
                      FAISS Vector Database
                               │
                User Question ─┤
                               ▼
                  Semantic Similarity Search
                               │
                               ▼
                     Retrieved Context
                               │
                               ▼
                   Google Gemini API (LLM)
                               │
                               ▼
                Role-Based Access Control
                               │
                               ▼
                       Final AI Response
                               │
                               ▼
                     User Feedback Storage
```

---

# 📂 Repository Structure

```
AI-Financial-Assistant
│
├── AI_Financial_Assistant.ipynb
├── README.md
├── requirements.txt
├── annual_report.pdf
├── financial_data.xlsx
├── financial_index.faiss
├── chunks.json
├── feedback.json
├── sample_questions.txt
└── LICENSE
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| Google Gemini API | LLM Response Generation |
| Sentence Transformers | Text Embeddings |
| FAISS | Semantic Vector Search |
| pdfplumber | PDF Text Extraction |
| Pandas | Data Processing |
| NumPy | Numerical Operations |
| OpenPyXL | Excel File Generation |
| Gradio | Interactive Web UI |

---

# 🔄 Workflow

### 1️⃣ Document Ingestion

- Upload Annual Report PDF
- Extract text using pdfplumber

↓

### 2️⃣ Data Processing

- Extract financial tables
- Convert tables into Excel

↓

### 3️⃣ Knowledge Base

- Split report into chunks
- Generate embeddings
- Store embeddings in FAISS

↓

### 4️⃣ User Query

- Convert question to embedding
- Retrieve relevant chunks

↓

### 5️⃣ AI Response

- Send retrieved context to Gemini API
- Generate context-aware answer

↓

### 6️⃣ RBAC

Different users have different permissions.

| Role | Access |
|------|---------|
| CEO | Full Access |
| CTO | Restricted Executive Information |
| Intern | Public Financial Information Only |

↓

### 7️⃣ Feedback

Store Helpful / Not Helpful responses in JSON.

---

# 🔒 Role-Based Access Control

## 👔 CEO

✔ Full access to financial information

Examples

- Total Revenue
- Executive Compensation
- Cash Holdings
- Acquisitions

---

## 💻 CTO

Restricted

- Executive Compensation
- Salary
- Headcount

Allowed

- Revenue
- Net Income
- Operating Expenses

---

## 🎓 Intern

Allowed

- Revenue
- Gross Margin
- Product Sales

Restricted

- Executive Information
- Salary
- Cash Holdings
- Investments
- Acquisitions

---

# 💻 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Financial-Assistant.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Gemini API Setup

Replace

```python
api_key="YOUR_API_KEY"
```

with your own Gemini API key.

---

# ▶️ Running

Open

```
AI_Financial_Assistant.ipynb
```

Run all cells.

Launch the Gradio interface.

---

# 📈 Sample Questions

### CEO

- What was Apple's total revenue?
- What was Apple's executive compensation?
- How much cash did Apple have?

### CTO

- What was Apple's net income?
- What were Apple's operating expenses?

### Intern

- What was Apple's gross margin?
- What were Apple's product sales?

---

# 📊 Generated Files

| File | Purpose |
|------|----------|
| chunks.json | Document Chunks |
| financial_index.faiss | Vector Index |
| feedback.json | User Feedback |
| financial_data.xlsx | Financial Tables |

---

# 🎯 Future Improvements

- Conversation Memory
- Pinecone Vector Database
- User Authentication
- Streaming Responses
- Metadata-Based RBAC
- Multi-document Support

---

# 👨‍💻 Author

**Subhrajeet Kumar**

AI Agent Developer Assessment

SOA University

---

# 📜 License

MIT License
