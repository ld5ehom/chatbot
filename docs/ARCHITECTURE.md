## Project Architecture Overview

```
project-architecture/
├── user_interface/         # Slack-based chatbot interface
├── api_service/            # FastAPI backend system
├── qa_engine/              # LangChain + AWS Bedrock
├── vector_search/          # Milvus-based document search
└── data_pipeline/          # Crawling, preprocessing, embedding generation
```

## Data Pipeline Structure

```
data-pipeline/
├── data_collection/        # Document crawling via Confluence & Notion API
├── preprocessing/          # Text extraction and document cleaning
├── embedding_generation/   # Vector embedding using AWS Bedrock
└── vector_storage/         # Store embeddings in Milvus for efficient search
```

## QA Pipeline Structure

```
qa-pipeline/
├── query_analysis/          # Analyze user question and convert to embedding vector
├── document_retrieval/      # Retrieve relevant documents using vector similarity (Milvus)
├── context_assembly/        # Combine question and documents to build prompt
└── answer_generation/       # Generate answer using AWS Bedrock LLM
```
