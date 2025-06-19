# Text Transformation Agent Prototype 🧠

This project showcases a lightweight, agent-style application built using LangChain and OpenAI's GPT-4o API. It performs creative and intelligent text rewriting tasks, such as summarization, translation, and tone modulation — with real-time response streaming. Although not a full LangChain Agent (with memory and tools), this prototype simulates agent behavior using prompt logic and conditional input.

---

## 🚀 Features

- 🔍 **Automatic Language Detection**  
  Detects the input text's language and conditionally decides whether translation is needed.

- 📝 **Summarization with Style**  
  Conditionally summarizes the text with user-specified tone: `formal`, `humorous`, `casual`, or `neutral`.

- 🌐 **Multilingual Translation**  
  Translates text into a user-selected target language — or explains if translation is redundant.

- ⚡ **Streaming Output**  
  Uses LangChain’s `ChatOpenAI(streaming=True)` to stream responses as they’re generated, simulating a real-time assistant.

---

## 🛠 Tech Stack

- [LangChain](https://www.langchain.com/)
- [OpenAI GPT-4o](https://platform.openai.com/)
- [Python](https://www.python.org/)
- [Jupyter Notebook](https://jupyter.org/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)
- [langdetect](https://pypi.org/project/langdetect/)

---

## 🧪 How to Run

1. **Clone the repo**

```bash
git clone https://github.com/your-username/text-transformation-agent.git
cd text-transformation-agent

Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate    # on macOS/Linux
venv\Scripts\activate       # on Windows

Install dependencies
pip install -r requirements.txt

Set your OpenAI API Key
Create a .env file in the root directory and add:
OPENAI_API_KEY=your-key-here

Launch the notebook:
jupyter notebook "Text Transformation Agent Prototype.ipynb"
