🦜 LangChain: Chat with SQL Database
A powerful Streamlit application that enables natural language conversations with SQL databases using LangChain and Groq's Llama3 model. Ask questions in plain English and get intelligent responses from your database!
✨ Features

🗣️ Natural Language Queries: Chat with your database using everyday language
🗄️ Multi-Database Support: Works with both SQLite and MySQL databases
🤖 AI-Powered: Leverages Groq's Llama3-8b-8192 model for intelligent responses
💬 Interactive Chat Interface: Real-time conversation with streaming responses
🔄 Session Management: Maintains conversation history with clear option
🛡️ Secure: Password fields for sensitive database credentials

🚀 Quick Start
Prerequisites

Python 3.8 or higher
Groq API key (Get one here)
MySQL database (optional, if not using SQLite)

Installation

Clone or download the application
bash# Save the code as app.py or your preferred filename

Install required packages
bashpip install streamlit langchain langchain-groq sqlalchemy mysql-connector-python pathlib sqlite3

Prepare your database

For SQLite: Place your student.db file in the same directory as the app
For MySQL: Ensure your MySQL server is running and accessible


Run the application
bashstreamlit run app.py


🗄️ Database Configuration
Option 1: SQLite Database

Select "Use SQLLite 3 Database- Student.db" from the sidebar
Ensure student.db exists in your project directory
The app will automatically connect in read-only mode

Option 2: MySQL Database

Select "Connect to you MySQL Database" from the sidebar
Fill in the required connection details:

MySQL Host: Your database host (e.g., localhost, 127.0.0.1)
MySQL User: Your database username
MySQL Password: Your database password
MySQL Database: The name of your database



🔑 API Configuration

Get your Groq API key from Groq Console
Enter the API key in the sidebar field labeled "GRoq API Key"
The app uses Llama3-8b-8192 model for processing queries

💡 Usage Examples
Once connected, you can ask questions like:

General Queries:

"How many students are in the database?"
"Show me all tables in this database"
"What columns are available in the students table?"


Data Analysis:

"What's the average age of students?"
"Show me students from a specific city"
"Find the top 10 students by grades"


Complex Queries:

"Compare enrollment numbers by department"
"Show monthly registration trends"
"Which courses have the highest completion rates?"



🏗️ Project Structure
your-project/
│
├── app.py              # Main Streamlit application
├── student.db          # SQLite database (if using SQLite option)
├── requirements.txt    # Python dependencies (optional)
└── README.md          # This file
📦 Dependencies
txtstreamlit
langchain
langchain-groq
sqlalchemy
mysql-connector-python
pathlib
sqlite3
⚙️ Configuration Details
Database Connection Strings

SQLite: sqlite:/// with file path
MySQL: mysql+mysqlconnector://user:password@host/database

Model Configuration

Model: Llama3-8b-8192
Streaming: Enabled for real-time responses
Agent Type: ZERO_SHOT_REACT_DESCRIPTION

🔒 Security Notes

Database credentials are entered through secure password fields
SQLite database opens in read-only mode for safety
API keys are handled securely through Streamlit's input fields
Session data is stored locally and not persisted

🛠️ Troubleshooting
Common Issues

"Please enter the database information and uri"

Ensure you've selected a database option and filled in required fields


"Please add the groq api key"

Enter your valid Groq API key in the sidebar


"Please provide all MySQL connection details"

Fill in all MySQL connection fields (host, user, password, database)


Database Connection Errors

Verify your database is running and accessible
Check connection credentials
Ensure firewall settings allow the connection


SQLite File Not Found

Ensure student.db exists in the same directory as your app
Check file permissions



Performance Tips

The database connection is cached for 2 hours to improve performance
Use "Clear message history" to reset the conversation
For large databases, be specific in your queries to get faster responses

🤝 Contributing
Feel free to enhance this application by:

Adding support for more database types
Implementing query result visualization
Adding export functionality for chat history
Improving error handling and user feedback

📄 License
This project is provided as-is for educational and development purposes.

Happy Chatting with your Database! 🎉
For issues or questions, please check the troubleshooting section above or refer to the official documentation of LangChain and Streamlit.
