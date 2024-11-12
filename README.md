# Research-chat-bot-Research Assistant AI
Overview

The Research Assistant AI is a tool built with Streamlit to support researchers in analyzing research papers. With this app, users can upload PDF files or paste text content from research articles, and perform tasks like citation extraction, semantic search, question answering, summarization, and finding related papers. Powered by Google Generative AI, the application provides robust natural language processing capabilities to enhance research workflows.

Features
Upload & Analyze Papers: Users can upload PDF research papers or paste content directly into the app for analysis.

Citation Extraction: Automatically extracts and formats citations from research papers.

Semantic Search: Perform advanced semantic searches across the uploaded research papers.

Ask Questions: Ask specific questions about the paper's content and receive AI-generated responses.

Paper Summarization: Generate concise summaries of research articles.

Find Related Papers: Get suggestions for related research papers based on content analysis.

Prerequisites
Python 3.10 or higher
Google API Key for Google Generative AI
Installation
Clone the Repository:


Set Up a Virtual Environment:


Copy code
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install Dependencies:


Copy code
pip install -r requirements.txt

Configuration

Configure Your Google API Key:

Obtain an API key from the Google Cloud Platform and add it to your environment.

Running the Application

Launch the Streamlit Application:



Copy code
streamlit run app.py

Access the App: Open your browser and go to http://localhost:8501 to begin using the application.

Code Structure

app.py: Main entry point for the Streamlit app, managing the core functionality and layout.

ui_layout.py: Functions that set up the sidebar and main page layout for a user-friendly interface.

analysis.py: Houses functions for research paper analysis, comparison, and summarization.

pdf_utils.py: Utility functions to extract text from uploaded PDF files.

citation.py: Functions for citation extraction and formatting.

semantic_search.py: Functions enabling semantic search and text highlighting.

reference_management.py: Reference management functions, with support for tools like Zotero.
