
# 🚀 ColdMail-GPT — Cold Emails That Land the Deal

ProspectPilot is a powerful AI-driven application that crafts **hyper-personalized cold emails** from job descriptions or career pages.

> 💡 Simply paste a job URL, and ProspectPilot scrapes it, identifies relevant roles, matches your portfolio, and writes a tailored cold email — all locally using LLaMA.

---

## 🎯 What It Does

- 🕸️ Scrapes job descriptions from company websites
- 🧠 Uses **RAG + LLaMA-4** via **LangChain** and **Groq**
- 🧾 Analyzes your portfolio from a CSV and matches relevant projects
- 📎 Attaches links matching the skills required in job
- ✉️ Crafts a **cold outreach email** tailored to the job, company, and your capabilities

---

## 🔧 How It Works

1. **Scrape Job Page**: Uses `WebBaseLoader` to get job descriptions  
2. **Extract Roles & Skills**: Parses job listings into structured JSON  
3. **Portfolio Vector DB**: Uses **ChromaDB** to match projects by tech stack  
4. **Cold Email Generation**: LLaMA-4 model generates a contextual pitch email  
5. **Final Output**: Cold email with portfolio links ready to send!

---

## 🖥️ Installation

### 1. # Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Pull necessary models
ollama pull llama3
ollama pull mxbai-embed-large
 ## Create virtual env and install requirements
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

pip install -r requirements.txt


