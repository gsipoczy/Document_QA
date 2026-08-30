# DocChat: a Multi-Agent RAG System

This application combines multiple AI agents, each with a specific role:
- A Hybrid Retriever that intelligently combines BM25 keyword search and vector embeddings to retrieve the most relevant passages
- A Research Agent that analyzes the retrieved content and generates an initial response
- A Verification Agent that cross-checks the response against the original document to detect hallucinations and flag unsupported claims
- A Self-Correction Mechanism that re-runs the research step if any contradictions or unsupported statements are found

## Multi-step, verification-driven approach

This multi-step, verification-driven approach ensures that DocChat provides precise, document-grounded answers, even for complex and long-form documents that general-purpose chatbots struggle with. Whether you need to extract specific data points, summarize sections, compare multiple reports, or analyze tables, DocChat is built to help you navigate your documents with confidence.

## Document types

DocChat only accepts documents in these formats: '.pdf', '.docx', '.txt', '.md'.

## Prerequisites

The following environment variables must have set:

For OpenAI:
- OPENAI_API_KEY

For IBM WatsonX AI:
- WATSONX_API_KEY
- WATSONX_URL
- WATSONX_PROJECT_ID

