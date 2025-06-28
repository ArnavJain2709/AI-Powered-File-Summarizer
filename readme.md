# AI File Summarizer & Chatbot

This is a web application built with Python and Streamlit that uses the Google Gemini API to analyze and interact with local files.

## Features

-   **Directory Scanning:** Scans a user-specified local directory for supported files.
-   **AI-Powered Summaries:** Generates a concise summary for each file found, using a truncated version of the content to stay within free-tier API limits.
-   **Multi-Format Support:** Can read and parse text from a wide range of file types:
    -   Documents: `.pdf`, `.docx`
    -   Spreadsheets: `.xlsx`, `.xls`
    -   Presentations: `.pptx`
    -   Code: `.py`, `.java`, `.js`, `.html`, `.css`, and more.
    -   Plain Text: `.txt`, `.md`, `.log`
-   **Interactive Q&A:** Features a chat interface that allows users to ask natural language questions about the files.
-   **Smart Context Handling:** If a question mentions a specific file, the application reads the *entire* file content to provide a detailed, context-aware answer.
-   **Cost-Aware Design:** Provides an explicit warning to the user before sending a full, large file for analysis, explaining that it may incur API costs.

## Setup & Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```

2.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the application:**
    ```bash
    streamlit run app.py
    ```

4.  **Add your API Key:**
    -   Get a free Google Gemini API key from [Google AI Studio](https://aistudio.google.com/).
    -   Paste the key into the input box in the application's sidebar.