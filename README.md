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
1. Financial PDF Ingestion

2. Financial Table Extraction

3. Excel Generation

4. Text Chunking

5. Sentence Transformer Embeddings

6. FAISS Vector Database

7. Retrieval-Augmented Generation (RAG)

8. Google Gemini API

9. Role-Based Access Control

10. Feedback Collection

11. Interactive Gradio Web Interface

---

# Project Architecture

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
AI-Financial-Assistant-Azentio/
│
├── AiFinancialAssistant.ipynb
├── LICENSE
├── README.md
├── annual_report.pdf
├── chunks.json
├── feedback.json
├── financial_data.xlsx
├── financial_index.faiss
├── requirements.txt
└── sample_questions.txt
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

### 1 Document Ingestion

- Upload Annual Report PDF
- Extract text using pdfplumber

↓

### 2 Data Processing

- Extract financial tables
- Convert tables into Excel

↓

### 3 Knowledge Base

- Split report into chunks
- Generate embeddings
- Store embeddings in FAISS

↓

### 4 User Query

- Convert question to embedding
- Retrieve relevant chunks

↓

### 5 AI Response

- Send retrieved context to Gemini API
- Generate context-aware answer

↓

### 6 RBAC

Different users have different permissions.

| Role | Access |
|------|---------|
| CEO | Full Access |
| CTO | Restricted Executive Information |
| Intern | Public Financial Information Only |

↓

### 7 Feedback

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
git clone https://github.com/Subhrajeet-21/AI-Financial-Assistant.git
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

#  Sample Questions

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

- Conversation Memory – Remember previous questions and answers for follow-up queries.
- Pinecone Vector Database – Use a scalable cloud-based vector database instead of local FAISS.
- User Authentication – Add login-based authentication and automatically assign user roles.
- Streaming Responses – Display Gemini responses progressively for a faster user experience.
- Metadata-Based RBAC – Use document metadata and permissions for more precise access control.
- Multi-Document Support – Support multiple financial reports, companies, and financial years.

---

# 🖼️ Demo

## Home Page

<img width="1395" height="819" alt="Screenshot 2026-08-07 223054" src="https://github.com/user-attachments/assets/5c36390a-3737-48e6-928d-ca48571490f4" />


## CEO Query

<img width="1374" height="600" alt="Screenshot 2026-08-07 223122" src="https://github.com/user-attachments/assets/7dbaf76a-bb4c-46ea-a8e7-567b3f47db6f" />


## RBAC

<img width="1367" height="577" alt="Screenshot 2026-08-07 223152" src="https://github.com/user-attachments/assets/0e1ea578-cdd3-4722-9121-d848ce982585" />


## Feedback

<img width="1330" height="597" alt="Screenshot 2026-08-07 223223" src="https://github.com/user-attachments/assets/8d9fc6e6-a6e0-49f8-b423-b43bc86d2817" />


# 👨‍💻 Author

**Subhrajeet Mohanty**

AI Agent Developer Assessment of *Azentio*

ITER, SOA University

---

# 📜 License

MIT License
