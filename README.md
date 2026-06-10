# AI-Powered Banking Document Intelligence System
Overview

This project implements an enterprise-style Retrieval-Augmented Generation (RAG) system capable of understanding and answering questions from:

RBI Master Directions
RBI Circulars
Banking Guidelines
Bank Statements
UPI Transaction Screenshots
Payment Receipts
Financial PDFs

The system combines OCR, semantic search, vector databases, and locally hosted Large Language Models to provide privacy-preserving document intelligence without relying on external APIs.

## Features
OCR-based extraction from scanned PDFs
OCR support for payment screenshots
Native text extraction from digital PDFs
Local embeddings using nomic-embed-text
ChromaDB persistent vector storage
LangChain-based retrieval pipeline
Local LLM inference using llama3.2
Interactive conversational interface
Multi-document semantic search
Source-grounded responses
Offline execution without cloud APIs


### Technologies Used
Python
LangChain
LangChain Chroma
LangChain Ollama
ChromaDB
Ollama
Llama 3.2
Nomic Embed Text
PyMuPDF
Tesseract OCR
PDF2Image
Pillow


#### Installation

Clone repository
git clone https://github.com/yourusername/AI-Banking-RAG-System.git
cd AI-Banking-RAG-System

Install dependencies
pip install -r requirements.txt

Install Ollama
ollama pull llama3.2
ollama pull nomic-embed-text

Start Ollama
ollama serve

##### Usage
Place RBI documents inside:
 data/sample_rbi_pdfs/
Place bank statements inside:
data/sample_bank_statements/
Place payment screenshots inside:
 data/sample_transaction_images/
Run notebook.
Build vector database.
Start interactive session.


###### Example Queries
Summarize the RBI KYC Master Direction.

List all salary credits during May.

Identify repeated round-figure debit transactions.

Show all UPI payments above ₹5,000.

Does this statement indicate suspicious activity?

Which RBI guideline discusses customer due diligence?

Summarize the uploaded payment screenshots.

What is the average monthly balance?

