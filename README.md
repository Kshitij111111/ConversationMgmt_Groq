💬 Conversation Management & 🗂️ Classification using Groq API

This project demonstrates:
✨ Task 1: Conversation Management with Summarization
✨ Task 2: JSON Schema Classification & Information Extraction

Built in Google Colab using the Groq API (OpenAI SDK compatible) — with no frameworks (pure Python only).

🔥 Features
📝 Task 1: Conversation Management with Summarization

✔️ Maintain a running history of chats
✔️ Summarize conversation history to keep it concise
✔️ Flexible truncation options:
  ➡️ Limit by number of turns (last n messages)
  ➡️ Limit by character/word length
✔️ Periodic summarization after every k-th run
✔️ Demo with multiple conversations and truncation settings

📊 Task 2: JSON Schema Classification & Information Extraction

✔️ Define a JSON schema for 5 details:

name

email

phone

location

age

✔️ Use Groq API function calling for structured outputs
✔️ Extract and validate information from chats
✔️ Demonstrated on 3 sample user conversations

🛠️ Tech Stack

🐍 Python (standard library only)

☁️ Google Colab (testing & demos)

⚡ Groq API (OpenAI-compatible client)

✅ jsonschema (schema validation)

📂 Project Structure
📦 conversation-groq-assignment
 ┣ 📜 Assignment.ipynb   → Main Colab notebook
 ┣ 📜 README.md          → Documentation (this file)
 ┗ 📜 requirements.txt   → Dependencies (openai, jsonschema)

⚙️ Setup & Usage

1️⃣ Clone Repository

git clone https://github.com/<your-username>/conversation-groq-assignment.git
cd conversation-groq-assignment


2️⃣ Install Dependencies

pip install -r requirements.txt


3️⃣ Run in Google Colab

Upload Assignment.ipynb

Add your Groq API key in Cell 2:

os.environ["GROQ_API_KEY"] = "your_api_key_here"


4️⃣ Execute Cells in Order

🎯 Example Outputs
📝 Task 1 – Summarization Demo
=== Run 1 ===
Assistant: Sure, I can help review your resume...

=== Run 3 ===
Assistant: (Summary) User is seeking help with SDE resume, projects, and ML video processing.

📊 Task 2 – Extraction Demo

💬 Input Chat:

Hi, I’m Kshitij Sharma, 23 years old from Delhi.
My email is ksh@example.com and my phone is 9876543210.


📦 Extracted JSON:

{
  "name": "Kshitij Sharma",
  "email": "ksh@example.com",
  "phone": "9876543210",
  "location": "Delhi",
  "age": 23
}

✅ Evaluation Criteria (Covered)

✔️ Correctness of implementation
✔️ Summarization logic (k-th run)
✔️ Schema-based extraction
✔️ Clean documentation & code clarity
✔️ GitHub version control

📌 Notes

Uses Groq-hosted models (OpenAI-compatible).

Tested on llama3-8b-8192.

No frameworks (LangChain, etc.) were used.

👨‍💻 Author: Kshitij Sharma

