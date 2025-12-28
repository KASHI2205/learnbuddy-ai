
# 🤝 LearnBuddy AI

**LearnBuddy AI** is an AI-powered study assistant that lets you upload PDF notes and interact with them using chat, summaries, and quizzes. It helps students learn smarter by turning static notes into an interactive learning experience.

---

## 🚀 Features

- 📄 Upload PDF notes
- 💬 Chat with your documents (RAG-based Q&A)
- 📝 Generate concise summaries
- ❓ Create quizzes from notes
- 📊 Word cloud & basic analytics
- 📄 Export chat to PDF
- 🎨 Clean, minimal UI (neutral + coral theme)
- ⚡ Real-time AI responses

---

## 🧠 How It Works

LearnBuddy uses **Retrieval-Augmented Generation (RAG)**:
1. Extracts text from uploaded PDFs  
2. Splits text into chunks  
3. Uses TF-IDF + cosine similarity to find relevant content  
4. Sends only relevant context to the LLM for accurate answers  

This ensures responses stay grounded in your notes.

---

## 🛠 Tech Stack

- **Python**
- **Streamlit** – UI framework
- **OpenAI API** – LLM responses
- **PyPDF** – PDF text extraction
- **Scikit-learn** – TF-IDF & similarity search
- **Matplotlib & WordCloud** – analytics
- **ReportLab** – export chat to PDF

---
## 📂 Project Structure

learnbuddy/
│
├── app.py # Main Streamlit app
├── requirements.txt # Dependencies
├── .env # API key (not committed)
└── README.md

yaml
Copy code

> *(Optional: Can be modularized further into RAG, AI utils, and styles.)*

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/learnbuddy-ai.git
cd learnbuddy-ai
2️⃣ Create virtual environment (optional but recommended)
bash
Copy code
python -m venv venv
venv\Scripts\activate   # On Windows
# source venv/bin/activate  # On Mac/Linux
3️⃣ Install dependencies
bash
Copy code
pip install -r requirements.txt
4️⃣ Set up environment variables
Create a .env file in the root:

env
Copy code
OPENAI_API_KEY=your_api_key_here
⚠️ Never commit your API key.

▶️ Run the App
bash
Copy code
streamlit run app.py
Then open the URL shown in the terminal (usually http://localhost:8501).



Learning by doing

📫 Feel free to connect on LinkedIn or GitHub!
## 📂 Project Structure

