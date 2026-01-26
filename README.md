md (copy-paste)
# 🔎 AI Search Engine with LangChain Tools + Agents (Groq + Streamlit)

A Streamlit-based **AI search engine** powered by **LangChain Agents** and **Groq LLMs**, capable of answering questions by using real tools like:

✅ Wikipedia  
✅ arXiv  
✅ DuckDuckGo Search  

The agent decides which tool to use, fetches relevant info, and produces a final answer.

---

## 🚀 Features

- ✅ LangChain Agent-based reasoning
- ✅ Uses external tools for live search:
  - WikipediaAPIWrapper
  - ArxivAPIWrapper
  - DuckDuckGo Search
- ✅ Streamlit UI for interactive chat
- ✅ Groq LLM integration for fast responses
- ✅ Real-time tool calling with agent execution traces

---

## 🧠 Tech Stack

- **Frontend**: Streamlit  
- **LLM**: Groq (via `langchain_groq`)  
- **Agents + Tools**: LangChain  
- **Search Tools**:
  - Wikipedia Query Tool
  - arXiv Query Tool
  - DuckDuckGo Search Tool  
- **Environment**: Python + dotenv

---

## 📂 Project Structure
```bash
.
├── app.py
├── requirements.txt
├── .env.example
└── tools_agent.ipynb
```

---

## ⚙️ Setup Instructions

### 1️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate:

Windows
```bash
.\venv\Scripts\activate
```

Mac/Linux
```bash
source venv/bin/activate
```
### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Add Groq API Key

Create .env file:
```bash
GROQ_API_KEY=your_api_key_here
```
### 4️⃣ Run the App
```bash
streamlit run app.py
```
## ✅ How It Works

- User types a question

- Agent decides which tool(s) to call:

- Wikipedia for general knowledge

- arXiv for research papers

- DuckDuckGo for live web info

- Agent collects tool outputs

- Groq LLM produces the final answer

## 🧪 Example Queries

- "What is Retrieval-Augmented Generation?"

- "Find recent arXiv papers on vision transformers"

- "Latest updates about LangChain?"

## 🔥 Future Improvements

- Add citations and source highlighting

- Add caching to reduce tool calls

- Add multi-step reasoning logs in UI

- Add PDF upload + RAG mode

## 👤 Author

Sahib Taj Singh


---