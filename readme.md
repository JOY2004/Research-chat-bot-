# Research Assistant AI

## Overview

This application is a Research Assistant AI built using Streamlit. It allows users to upload research papers in PDF format or paste their content, and then perform various analyses such as extracting citations, performing semantic searches, asking questions, and summarizing the papers. The application leverages Google Generative AI for natural language processing tasks.

## Features

- **Upload and Analyze Research Papers**: Upload PDF files or paste text content for analysis.
- **Extract Citations**: Extract and format citations from the research papers.
- **Semantic Search**: Perform semantic searches across the uploaded papers.
- **Ask Questions**: Ask specific questions about the content of the papers and get AI-generated answers.
- **Summarize Papers**: Generate concise summaries of the research papers.
- **Find Related Papers**: Suggest related research papers based on the analysis.

## Prerequisites

- Python 3.10 or higher
- Google API Key for accessing Google Generative AI

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/anubhab-m02/Research-Assistant-AI.git
    cd research-paper-analysis-assistant
    ```

2. **Create a virtual environment**:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

## Configuration

1. **Set up your Google API Key**:
    - Obtain an API key from Google Cloud Platform.

## Running the Application

1. **Start the Streamlit application**:
    ```sh
    streamlit run app.py
    ```

2. **Open your web browser** and navigate to `http://localhost:8501` to access the application.

## Code Structure

- **app.py**: Main entry point of the application. Configures the Streamlit page and handles the main logic.

- **ui_layout.py**: Contains functions to render the sidebar and main content layout.

- **analysis.py**: Functions for analyzing research papers, comparing papers, and summarizing content.

- **pdf_utils.py**: Utility functions for extracting text from PDF files.

- **citation.py**: Functions for extracting and formatting citations.

- **semantic_search.py**: Functions for performing semantic searches and highlighting text.

- **reference_management.py**: Functions for managing references using Zotero.


1. **API Key Exposure**: Ensure that the Google API key is kept secure and not exposed in the code or version control.

2. **Input Validation**: The application does not perform extensive validation on user inputs, which could lead to issues such as injection attacks or processing of malformed data.

3. **Error Handling**: While the application includes basic error handling, it could be improved to handle more specific cases and provide more informative error messages.

4. **PDF Extraction**: The text extraction from PDFs relies on PyPDF2, which may not
