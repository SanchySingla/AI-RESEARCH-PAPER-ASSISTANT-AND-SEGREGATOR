# **AI Research Paper Assistant and Segregator**

## **Project Overview**

This project aims to build an **AI-powered assistant** for researching and categorizing academic papers. It leverages **semantic search**, **summarization**, **keyword extraction**, and **Named Entity Recognition (NER)**.

## **Dataset**

**ML-ArXiv Papers from Hugging Face**
- ~15,000 ML research papers with Title and Abstract
- Link: [CShorten/ML-ArXiv-Papers](https://huggingface.co/datasets/CShorten/ML-ArXiv-Papers)

## **Technologies and Packages Used**

### **Core Libraries:**
- **datasets**: For loading and managing the academic paper dataset.
- **pandas**: For data manipulation and analysis, primarily for handling DataFrames.
- **numpy**: For numerical operations, especially with embeddings.

### **Semantic Search:**
- **sentence-transformers**: For generating high-quality sentence embeddings to enable semantic search.
- **faiss-cpu**: For efficient similarity search and indexing of embeddings.
- **scikit-learn**: Specifically for cosine_similarity to demonstrate similarity calculations.

### **Summarization:**
- **transformers**: For utilizing pre-trained models from Hugging Face, specifically a **BART-based summarization** pipeline.

### **Keyword Extraction:**
- **keybert**: For extracting important keywords and keyphrases from paper abstracts.

### **Named Entity Recognition (NER):**
- **gliner**: For advanced, **zero-shot named entity recognition** using a pre-trained model.
- **spacy**: For rule-based and statistical named entity recognition, providing structured categorical data.

### **LangChain Integration:**
- **langchain-community**: For integrating various language model components.
- **langchain-core**: Foundational components for Langchain.
- **langchain-huggingface**: Integration with Hugging Face models for Langchain pipelines.

### **Utility:**
- **flashdeberta**: Used as an environment variable to potentially optimize operations.

## **Future Development Plan**

To evolve this project into an **industry-scale solution**, the following enhancements are planned:

### **1. Restructuring for Industry Scale**
- **Modular Architecture**: Refactor the codebase into a more modular and scalable architecture, separating concerns like data loading, embedding generation, search, and NLP tasks into distinct modules.
- **API Design**: Design and implement a clear and well-documented API for interacting with the core functionalities (**search**, **summarization**, **NER**).

### **2. Advanced NER Tuning and Implementation**
- **Custom NER Models**: Train custom Named Entity Recognition models specifically tailored to the nuances and entities present in academic research papers.
- **Domain-Specific Labels**: Expand the set of NER labels to capture more domain-specific information crucial for academic analysis.
- **Contextual NER**: Implement contextual NER techniques that can better disambiguate entities based on the surrounding text in scientific abstracts.
- **Integration with Knowledge Graphs**: Explore integrating extracted entities into a knowledge graph to build richer relationships between papers and concepts.

### **3. Deployment and User Interface**
- **Deployment**: Use **Streamlit** or **FastAPI** to provide a UI layer.
- **Real-time Processing**: Optimize the search and NLP pipelines for near real-time performance to provide immediate results to users.

### **VIEW MY WORK IF RENDERING PROBLEM**
-**cleaned_notebook.ipynb**-For viewing static outputs and code.

-**semantic_research.ipynb**-For downloading and testing my work.

   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO_NAME/blob/main/your_notebook.ipynb)
