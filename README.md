# Chatbot powered by LangChain, OpenAI and Streamlit.

## Overview
This code sets up a chatbot powered by OpenAI model to assist with queries related to specific documents.
It starts by setting the OpenAI API key and initializing the ChatOpenAI component. Then, it loads the data from a JSON file, processes this data by splitting it into manageable text chunks, and embeds these chunks using OpenAI embeddings. 
The embeddings are stored in a FAISS vector database, which enables efficient similarity search and retrieval of relevant documents. 
A retriever is created to query this vector database, allowing the chatbot to get pertinent information based on user input, conversation history and relevant documents. 


## Features

- **User-friendly Interface**: Built with Streamlit, making it easy to interact with the chatbot.
- **Conversational Memory**: Maintains chat history to provide contextually relevant responses.
- **Document Retrieval**: Utilizes FAISS for efficient document retrieval based on embeddings from OpenAI.
- **Prompt Templates**: Uses `ChatPromptTemplate` to structure chatbot responses and queries.

## Installation

1. **Clone the repository**:
    
      git clone https://github.com/franconti/context_aware_chatbot.git
      cd recipes-chatbot


2. **Install dependencies**:

      pip install -r requirements.txt


## Usage

1. **Run the Streamlit application**:
   
       streamlit run context_aware_chatbot.py

2. **Input your OpenAI API Key** in the sidebar.

3. **Interact with the chatbot**: Type your questions in the chat input, and the bot will respond based on the conversation history and retrieved documents.

