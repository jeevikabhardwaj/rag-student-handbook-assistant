# RAG Student Handbook Assistant

## 1. Project Overview
The RAG (Retrieval-Augmented Generation) Student Handbook Assistant is a question-answering system that helps students find information in the Amity University Student Handbook 2025–2026. It retrieves relevant text from the handbook and uses a generative AI model to produce answers with PDF page references.

## 2. Objectives
- Extract text from a university handbook PDF.
- Divide the text into smaller, overlapping chunks.
- Generate embeddings for semantic search.
- Store and retrieve document chunks using ChromaDB.
- Generate context-based answers using the Gemini API.
- Display source PDF page numbers for reference.

## 3. Technologies Used
- **Python** — implementation
- **Google Colab** — development environment
- **PyMuPDF** — PDF text extraction
- **Sentence Transformers** — text embeddings using `all-MiniLM-L6-v2`
- **ChromaDB** — vector storage and similarity search
- **Google Gemini API** — answer generation

## 4. System Workflow
1. Upload the student handbook PDF.
2. Extract text from the PDF pages.
3. Split the text into chunks with overlap.
4. Generate vector embeddings for the chunks.
5. Store the text, embeddings, and page metadata in ChromaDB.
6. Convert the user's question into an embedding.
7. Retrieve relevant chunks using similarity search.
8. Send the retrieved context and question to Gemini.
9. Display the generated answer and source PDF pages.

## 5. How to Run
1. Open the notebook in Google Colab.
2. Upload the student handbook PDF when prompted.
3. Run the notebook cells in order.
4. Enter a valid Gemini API key when requested. Keep the key private.
5. Ask questions about the handbook and review the answers and source pages.

## 6. Limitations
- Answer quality depends on the relevance of retrieved chunks.
- Some answers may be incomplete if relevant text is not retrieved.
- Gemini API availability and rate limits may affect response generation.
- Source page numbers refer to physical PDF pages.

## 7. Conclusion
This project demonstrates a basic Retrieval-Augmented Generation pipeline for answering questions from a university handbook. It combines semantic search and generative AI to provide context-based responses with source references.
