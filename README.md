# 🧠 Natural Language to SQL Assistant

A powerful Streamlit app that allows you to chat with your **SQL database** using natural language via **LangChain**, **Groq’s LLaMA3 model**, and **MySQL** or **SQLite**.

## 📸 Demo

![Query_Interface](https://github.com/user-attachments/assets/e66c93d6-4c1d-4b3d-bd17-26d5de411e4b)

*Real-time SQL generation and query execution*

![Query_Results](https://github.com/user-attachments/assets/15d05504-5486-4c4e-a9b9-b16b7ce3e433)



## 🚀 Features

- 💬 **Natural Language Queries** – Ask questions like “Show all customers from Mumbai”
- 🧠 **AI-Powered** – Uses Groq's LLaMA3-8b model via LangChain for smart SQL generation
- 💾 **Multi-Database Support** – Works with both MySQL and SQLite
- 🧑‍💻 **Interactive UI** – Built with Streamlit for real-time chat
- 🔐 **Secure Input** – Password field for DB credentials
- 🧹 **Session Management** – History tracking with clear chat option

---

## 🛠️ Quick Start

### ✅ Prerequisites

- Python 3.8+
- Groq API key ([Get one here](https://console.groq.com/))
- MySQL (optional – defaults to SQLite)

### 📦 Installation

```bash
git clone https://github.com/Bhuvannaidu45/Natural-Language-to-SQL-Assistant.git
cd Natural-Language-to-SQL-Assistant

# Install requirements
pip install streamlit langchain langchain-groq sqlalchemy mysql-connector-python pathlib sqlite3

🗄️ Project Structure
  streamlit run app.py
   ├── app.py
   ├── README.md
   ├── requirements.txt
     └── database/
      └── your_db.db


👨‍💻 Author
Bhuvannaidu – GitHub | LinkedIn


