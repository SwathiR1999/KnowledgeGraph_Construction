# Knowledge Graph Construction from Web Data using LlamaIndex and Neo4j

This project demonstrates how to **automatically construct a semantic knowledge graph** from web pages related to a given topic. It uses **LlamaIndex**, **Neo4j**, and modern **open-source NLP models** to extract, embed, and structure information in a graph database for downstream querying and reasoning.

---

## What It Does

- Takes a **topic as input** (e.g., `"Shakespeare"`)
- Uses **DuckDuckGo Search** to find top web pages about the topic
- Parses and cleans the web content using `SimpleWebPageReader`
- Splits the content semantically using `SemanticSplitterNodeParser` with contextual embeddings
- Extracts **implicit entities and relationship paths** using `ImplicitPathExtractor`
- Stores the structured information in a **Neo4j property graph** for advanced querying and analysis

---

## Tech Stack

- LlamaIndex– document loading, parsing, node representation, graph indexing
- duckduckgo_search– fetch topic-specific web URLs
- HuggingFace Transformers – `intfloat/e5-base-v2` for semantic embeddings
- Neo4j – graph database for storing and exploring the knowledge graph

## Demo

Here's a preview of the extracted knowledge graph in Neo4j:

![Knowledge Graph Demo](https://github.com/user-attachments/assets/02579d83-eb03-43dd-bdef-5d2a9dfda215)
