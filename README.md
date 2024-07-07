# Multi PDF RAG Chatbot

This project is a Retrieval-Augmented Generation (RAG) based conversational AI application built using Streamlit. The application allows users to upload multiple PDF files, process them, and interact with the content through a chatbot interface. The chatbot uses advanced natural language processing techniques to understand and respond to user queries based on the content of the uploaded PDFs.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Project Structure](#project-structure)

## Features
- Upload multiple PDF files for processing
- Extract text from PDF files
- Split extracted text into manageable chunks
- Convert text chunks into vector representations for fast and efficient search
- Use OpenAI's GPT model to answer questions based on the PDF content
- Simple and user-friendly web interface built with Streamlit

## Technologies Used
- [Streamlit](https://streamlit.io/): Web application framework for creating interactive web apps
- [PyPDF2](https://pypi.org/project/PyPDF2/): Library for reading PDF files
- [Langchain](https://www.langchain.com/): Suite of tools for natural language processing and creating conversational AI
- [FAISS](https://faiss.ai/): Library for efficient similarity search of vectors
- [OpenAI](https://www.openai.com/): Provider of powerful AI models for natural language understanding and generation

## Setup and Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/multi-pdf-rag-chatbot.git
    cd multi-pdf-rag-chatbot
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up your OpenAI API key:
    - Create a `.env` file in the root directory and add your OpenAI API key:
    ```sh
    OPENAI_API_KEY=your_openai_api_key
    ```

5. Run the application:
    ```sh
    streamlit run app.py
    ```

## Usage
1. Open your web browser and go to `http://localhost:8501`.
2. Use the sidebar to upload one or more PDF files.
3. Click on the "Submit & Process" button to process the uploaded PDFs.
4. Once processing is complete, you can ask questions related to the PDF content using the text input field.

## Project Structure
multi-pdf-rag-chatbot<br>
├── app.py # Main application file<br>
├── requirements.txt # Required dependencies<br>
├── .env.example # Example environment file for API keys<br>
└── README.md # Project README file<br>

