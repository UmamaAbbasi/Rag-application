Simple Retrieval-Augmented Generation (RAG) Application
This project is a simple Retrieval-Augmented Generation (RAG) pipeline that uses OpenAI as the Large Language Model (LLM) and ChromaDB as the vector database.  
It retrieves relevant context from stored documents and augments the LLM’s response with this information.

Features
- Document ingestion and embedding into ChromaDB
- Semantic search over embedded documents
- Integration with OpenAI API for LLM-based responses
- Fully configurable and extendable

Technologies Used
- Python
- OpenAI API
- ChromaDB
- LangChain
- ONNX Runtime
- Visual Studio Code (development environment)

 Installation
 1. Clone the Repository
git clone https://github.com/UmamaAbbasi/rag-application.git
cd rag-application

2. Create and Activate Virtual Environment
   python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt

4. Set OpenAI API Key
Create a .env file in the project root and add:
OPENAI_API_KEY=your_api_key_here
Usage
5. Populate the Vector Database
python fill_db.py
This will embed and store documents in ChromaDB.

6. Ask a Question
python ask.py
The application will:
Search for relevant context in ChromaDB
Send the context + query to OpenAI
Return an augmented, context-aware answer
