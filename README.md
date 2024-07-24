**Title:** Chat with PDFs using Gemini

**Description:**

This Streamlit application empowers you to have a conversation with the content of your uploaded PDF files. Leverage the power of Google Generative AI to extract text, create contextual embeddings, and answer your questions in a comprehensive manner.

**Features:**

* **PDF Text Extraction:** Extracts text from uploaded PDF documents for further processing.
* **Contextual Embeddings:** Creates embeddings based on the extracted text to enable efficient searching and retrieval.
* **Conversational Question Answering:** Formulate questions about the PDF content, and the app will intelligently respond based on the extracted information.
* **Streamlit Interface:** Provides a user-friendly interface for uploading PDFs, asking questions, and viewing responses.

**Live Demo:**

The deployed Streamlit app is available at: [https://gemini-chat-with-pdfs.streamlit.app/](https://gemini-chat-with-pdfs.streamlit.app/)

**Requirements:**

* **Python 3.x**
* **Streamlit** (`pip install streamlit`)
* **PyPDF2** (`pip install PyPDF2`)
* **langchain** (`pip install langchain`)
* **langchain-google-genai** (`pip install langchain-google-genai`)
* **google-generativeai** (`pip install google-generativeai`)
* **dotenv** (`pip install python-dotenv`)

**Installation:**

1. Create a virtual environment (recommended) for managing dependencies:
   ```bash
   python -m venv env
   source env/bin/activate  # Windows: env\Scripts\activate.bat
   ```
2. Clone this repository or download the code.
3. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up your Google Cloud Project and obtain an API key (refer to Google Generative AI documentation for details):
   ```
   cp .env.example .env
   # Edit .env and add your Google API Key to GOOGLE_API_KEY
   ```

**Usage:**

1. Start the Streamlit app:
   ```bash
   streamlit run app.py
   ```
2. Access the app at http://localhost:8501/
3. Upload your PDF files using the file uploader in the sidebar.
4. Click the "Submit & Process" button to extract text and create embeddings.
5. Ask a question in the text input field related to the PDF content.
6. The app will display a response based on the extracted information and contextual analysis.

**Additional Notes:**

* Ensure your Google API key has appropriate permissions for using Google Generative AI services.
* This application is a work in progress. Expect further improvements and feature additions in the future.
* Feel free to contribute or raise issues on the repository.

**Further Contributions:**

* Consider adding error handling for potential issues during PDF processing, embedding creation, and question answering.
* Explore advanced question answering techniques and model fine-tuning for improved accuracy.
* Provide sample PDFs or a demo dataset to showcase the app's functionality.
* Include additional documentation or tutorials for advanced users.
