# Diagram Brief

**Title:** Governed Enterprise RAG Request And Feedback Flow

**Nodes:** Approved documents, ingestion, storage, Azure AI Search, Azure OpenAI, secured API, user application, Entra ID, Key Vault, telemetry, evaluation, feedback.

**Flow:** Documents are parsed and indexed. An authenticated request retrieves permitted chunks, produces a grounded answer with citations, and records diagnostics and feedback.

**Layout:** Ingestion lane above, runtime request lane in the center, governance and operations below.

Planned assets:

- azure-rag-runtime-flow-v1.excalidraw
- azure-rag-runtime-flow-v1.png
