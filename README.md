<br>

🚀 Technology Stack
Programming Language: Python

Web Framework: Flask

AI Framework: LangChain

Vector Database: Pinecone

LLM Integration: Groq API (llama3-70b-8192 model)

Embeddings: Hugging Face (sentence-transformers/all-MiniLM-L6-v2)

Data Ingestion: pypdf, python-dotenv

Deployment: Render

Version Control: Git

<br>

✨ Key Features
Retrieval-Augmented Generation (RAG): Combines information retrieval with a powerful LLM to deliver fact-based, relevant answers.

PDF Data Processing: Extracts and processes text from PDF documents to create a custom, searchable knowledge base.

Semantic Search: Uses vector embeddings to understand the meaning and context of user queries, ensuring highly relevant document retrieval.

Concise Responses: The system is prompted to provide brief, three-sentence answers to keep information clear and to the point.

Scalable Architecture: Built to be easily deployed and scaled on cloud platforms like Render, AWS, or GCP.

<br>

⚙️ Installation & Setup
Clone the Repository:

Bash

git clone https://github.com/aniruddh47/End-to-end-medical-chatbot.git
cd End-to-end-medical-chatbot
Create a Virtual Environment:

Bash

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install Dependencies:

Bash

pip install -r requirements.txt
Set Up Environment Variables:
Create a .env file in the root directory and add your API keys.

PINECONE_API_KEY="YOUR_PINECONE_API_KEY"
groq_api_key="YOUR_GROQ_API_KEY"
<br>

🚀 Usage
The project is designed to be run in two phases:

Indexing the Data: Run the store_index.py script to load and process your PDF documents, create embeddings, and upload them to your Pinecone index.

Bash

python store_index.py
Running the Chatbot: Start the Flask application to launch the web-based chat interface.

Bash

python app.py
Your chatbot will be accessible at http://127.0.0.1:5000 (or http://0.0.0.0:8080 if configured).

<br>

📈 Future Enhancements
Chat History & Session Management: Implement a memory component to allow the chatbot to remember previous conversations.

Health Record Storage: Add functionality to securely store and retrieve user health records.

External Tool Integration: Create tools for the chatbot to perform actions like providing meal plans or finding nearby hospitals.

<br>

📧 Contact
Author: Aniruddh Kumbhar

Email: aniruddh4722@gmail.com