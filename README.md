# NLP-Final-Project
FinMTEB
Modern NLP systems rely on text embeddings to represent meaning for tasks like search, clustering, and classification. Most embedding models are evaluated on general benchmarks like Massive Text Embedding Benchmark (MTEB), which contain broad, non-specialized text. However, financial language is highly domain-specific (earnings calls, filings, ESG reports, financial news). The authors question whether models that perform well on general benchmarks actually work well in finance.

The paper introduces FinMTEB, a benchmark specifically designed to evaluate embeddings on financial text.

Key characteristics:

<br>64 finance-specific datasets
<br>7 embedding task types
<br>Text sources include:
<br>Financial news
<br>Corporate annual reports
<br>ESG reports
<br>Regulatory filings
<br>Earnings call transcripts

Supports English and Chinese

<br>The benchmark evaluates embeddings across common NLP tasks:

<brClassification – categorize financial documents
<br>Clustering – group similar financial texts
<br>Retrieval – find relevant financial documents
<br>Pair classification – determine relationships between texts
<br>Reranking – reorder search results
<br>Summarization-related evaluation
<br>Semantic Textual Similarity (STS) – measure similarity between financial sentences.
