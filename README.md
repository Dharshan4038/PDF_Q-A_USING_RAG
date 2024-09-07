## PDF Question Answering Application
This application provides a robust solution for answering questions from PDF documents, including content from tables and images. It utilizes a combination of advanced techniques to extract and process information from various elements within a PDF, ensuring comprehensive and accurate responses.

### Features
1. Text Extraction from PDF: Utilizes PyMuPDF to extract images and text from PDF pages.
2. OCR for Images: Uses EasyOCR to recognize and extract text from images within the PDF, enabling answers from scanned content or embedded graphics.
3. Table Extraction: Processes tables from the PDF to ensure structured data is included in the question-answering process.
4. LangChain Integration: Leverages LangChain for document splitting and retrieval, using embeddings to build a vector store for efficient information retrieval.
5. Conversational AI: Employs OpenAI's Azure-based models for generating answers based on the extracted content.

### Techniques Used
1. Image Extraction: Images are extracted from the PDF using PyMuPDF and saved as PNG files for OCR processing.
2. Optical Character Recognition (OCR): EasyOCR is applied to extracted images to convert text from scanned or embedded images into machine-readable format.
3. Text Splitting and Vectorization: Documents are split into manageable chunks using RecursiveCharacterTextSplitter, and vector embeddings are created using OpenAI's Azure embedding model.
4. Question Answering Chain: A retrieval-augmented generation (RAG) approach is used, combining context retrieval with generative AI models to provide accurate and concise answers.
4. Handling Tables: Extracted table data is processed to ensure structured information is considered in the Q&A process.

### Usage
1. Load PDF: Input your PDF file for processing.
2. Extract Data: The application extracts text from PDF pages, including text from tables and images.
3. Ask Questions: Use the integrated Q&A system to ask questions about the content in the PDF, including data from tables and images.

This application provides a comprehensive solution for analyzing and retrieving information from complex PDF documents, making it an invaluable tool for data extraction and question answering.

