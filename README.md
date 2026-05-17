I built an Enterprise Finance GenAI Copilot for finance operations support at Wells Fargo. In this project, I created a document intelligence workflow where finance users could upload operational finance PDFs and ask questions in natural language.

I independently handled the complete workflow from document ingestion to final response generation. First, I extracted text from finance documents using Python and PDF processing libraries. Then I cleaned the data, removed unwanted characters, and split the document into section-based chunks to preserve business context.

After chunking, I added metadata enrichment like finance topic classification, source file tracking, and access-level tagging. I created categories such as invoice operations, reconciliation, customer support, risk compliance, security access, and AI governance so the retrieval system could search only the correct business area.

For retrieval, I implemented a hybrid retrieval approach using TF-IDF vectorization, cosine similarity scoring, keyword matching, metadata filtering, and reranking-style final scoring. This improved retrieval quality and helped return more accurate finance-related answers.

I also added RBAC-based filtering logic so users could retrieve only authorized finance content. Then I built grounded response generation where the system generated answers only from retrieved document context and avoided unsupported responses or hallucinations.

To improve trust and compliance, I added validation checks, audit logging, source tracking, confidence scoring, and safe fallback handling whenever the answer was not available in the approved finance document.

Finally, I built a Gradio-based UI where users could upload finance documents, ask questions, review retrieved source chunks, and see validation status. This project helped simulate a real enterprise finance GenAI workflow similar to production-level RAG applications used in banking environments.
