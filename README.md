# Document RAG Assistant

This project is a simple document question answering system.

It takes a document, splits it into chunks, converts the chunks into searchable vectors, and retrieves the most relevant chunks for a user question. Then it gives a grounded answer using only the retrieved document content.

## What this project does

- uploads a document
- reads PDF, DOCX, or TXT files
- cleans the text
- splits the document into chunks
- creates TF-IDF vectors
- retrieves the most relevant chunks for a question
- generates a grounded answer from retrieved text
- saves output files

## Main files

- `document_chunks.csv`
- `sample_query_answers.csv`
- `app.py`
- `requirements.txt`
- `README.md`

## Tools used

- Python
- pandas
- scikit-learn
- pypdf
- python-docx
- gradio

## Example questions

- What does the document say about AI governance?
- What systems are mentioned in the enterprise architecture?
- What are the future roadmap priorities?
- How does the organization handle security?
- What does the document say about digital transformation?

## Why this project is useful

This project is useful for understanding how document retrieval and grounded question answering work in a simple way.

It shows how a document can be turned into searchable chunks and used to answer questions without relying on a paid API.

## How to run

1. Open the notebook in Google Colab
2. Upload your document
3. Run all cells
4. Ask questions
5. Review the saved output files
6. Upload the project files to GitHub
