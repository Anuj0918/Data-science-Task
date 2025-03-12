# RAG and Text-to-SQL Query in Single Interface

This project builds a RAG and Text-to-SQL query app in a single interface. We use:

- **OpenAI** to power the LLM capabilities  
- **LlamaIndex** for orchestrating the RAG app  
- **SQL Database** for storing and processing data from CSV files.  
- **Streamlit** Provides an interactive and user-friendly UI. 



## 🧵 Twitter Thread  
**[X Thread](https://typefully.com/t/EJEGoEp)** 

---

## 🚀 Installation and Setup  

## 1️. Setup OpenAI and LlamaCloud

Get an API key from [OpenAI](https://openai.com) and set it in the `.env` file:

Get an API key from [Llama Cloud](https://www.llama.cloud) and set it in the `.env` file:


```ini
OPENAI_API_KEY="your-openai-api-key"

name="your-llama-cloud-index-name"
project_name="your-llama-cloud-project-name"
organization_id="your-llama-cloud-organization-id"
api_key="your-llama-cloud-api-key"
```
## 2. Install Dependencies and Run the App
   
```ini  
  pip install streamlit llama-index openai sqlalchemy python-dotenv nest-asyncio
 ```
## How to Use

1. **Upload a CSV file** using the file uploader in the main interface.
2. **Ask questions** in natural language in the text input field, such as:
   - "Tell me about the history of Los Angeles City."
   - "Which states have cities with populations over 1 million?"
3. The application will **automatically determine** whether to use SQL or RAG to answer your question and display the results.

### How It Works:
The system **routes queries** between:
- **Text-to-SQL Tool** → Translates natural language into SQL queries for structured data analysis.
- **Llama Cloud RAG Tool** → Retrieves information from a knowledge base for contextual answers.


```ini  
  streamlit run app.py
 ```


