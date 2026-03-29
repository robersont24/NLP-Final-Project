# Computational Analysis of Natural Languages - Final Project (Spring 2026)

## 👥 Group Information

**Group No:** 04  

**Members:**
- Jayath Premasinghe  
- Shrutiben Patel  
- Taylor Roberson  

---

## 📄 Paper Details

**Title:** FinMTEB: Finance Massive Text Embedding Benchmark  
**Authors:** Yixuan Tang and Yi Yang  

This project is based on the above research paper. We selected this paper for our final project due to its focus on domain-specific embedding evaluation in the financial domain. The work presented in this repository is an attempt to reproduce the experimental results and analyze the benchmark.

---

## 📄 Paper Overview

Modern NLP systems rely on text embeddings for tasks such as retrieval, clustering, and classification. However, most embedding models are evaluated on general-purpose benchmarks, which may not reflect performance in specialized domains like finance.

Financial language is highly domain-specific, including:
- Earnings call transcripts  
- Corporate filings  
- ESG reports  
- Financial news  

The FinMTEB benchmark introduces a domain-specific evaluation framework designed for financial text. It evaluates embedding models across multiple NLP tasks such as classification, clustering, retrieval, reranking, summarization, and semantic similarity.

---

## 📌 Project Objective

The goal of this project is to reproduce and analyze experiments from the FinMTEB benchmark, a financial-domain evaluation framework for text embeddings.

This project aims to:
- Reproduce the main experimental results of the paper  
- Evaluate the reproducibility of the benchmark  
- Conduct an additional experiment beyond the original study  

---

## 🔬 Reproduced Experiments

We reproduced the benchmark evaluation for three embedding models:

- **BAAI/bge-base-en-v1.5**  
- **intfloat/e5-base-v2**  
- **sentence-transformers/all-MiniLM-L6-v2**  

The experiments were conducted on English tasks across all major task categories.

---

## 📊 Results Summary

| Model | Classification | Clustering | PairClassification | Reranking | Retrieval | STS | Summarization |
|------|--------------|-----------|-------------------|-----------|----------|-----|--------------|
| BAAI/bge-base-en-v1.5 | 0.640596 | 0.559759 | 0.678872 | 0.976689 | 0.618503 | 0.355123 | 0.453604 |
| intfloat/e5-base-v2 | 0.654155 | 0.561392 | 0.661632 | 0.975959 | 0.625210 | 0.387627 | 0.526124 |
| sentence-transformers/all-MiniLM-L6-v2 | 0.579296 | 0.537353 | 0.582532 | 0.973224 | 0.568446 | 0.308763 | 0.363982 |

### Key Findings:
- E5 achieves the best overall performance  
- BGE performs competitively across tasks  
- MiniLM shows lower performance due to smaller model capacity  

---

## 🔍 Comparison with Paper Findings

The reproduced results are consistent with the trends reported in the original study:

- Stronger embedding models (E5, BGE) outperform smaller models  
- Performance trends across task types are similar  
- Minor differences in scores are likely due to differences in hardware and evaluation settings  

---

## 🧪 Additional Experiment: Retrieval Consistency

We conducted an additional experiment analyzing retrieval performance across different datasets.

### Findings:
- All models show high variance across retrieval tasks  
- Performance varies significantly depending on the dataset  
- Benchmark averages alone do not fully capture model behavior  

---

## 📁 Repository Contents

- `FinMTEB_final.ipynb` — Main reproduction notebook  
- `README.md` — Project documentation