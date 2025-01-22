# Graph RAG for Medicine: A Knowledge Graph Enhanced Retrieval-Augmented Generation Application

This project showcases the development of a **Graph RAG (Retrieval-Augmented Generation)** application combining **Large Language Models (LLMs)** with **knowledge graphs** to enhance the accuracy and explainability of Retrieval-Augmented Generation.

## Key Features
1. **Hybrid Search Approach**:
   - Initial retrieval of articles using a **vector database** based on semantic similarity.
   - Refinement of results via a **knowledge graph** and a controlled vocabulary (**MeSH**).

2. **Context Poisoning Mitigation**:
   - Ensures that LLMs process only the most relevant and structured data, improving reliability.

3. **Streamlined Workflow**:
   - Built using **Streamlit** for an intuitive user experience.
   - Demonstrates a three-step pipeline:
     - Search articles using vector similarity.
     - Refine terms with the MeSH vocabulary and knowledge graph.
     - Filter and summarize results with an LLM.

4. **Scalability and Governance**:
   - Highlights the importance of structured metadata for scalable and real-world deployments.

---

## Prerequisites
### Setup
To run this project locally, follow the steps below:

### Step 1: Clone the Repository
```bash
git clone https://github.com/Sa1f27/GraphRAG.git
cd <repository-folder>
```

### Step 2: Set Environment Variables
Create a `.env` file in the root directory and include the following:

```
WCD_URL=<paste your Weaviate instance>
WCD_API_KEY=<paste your Weaviate API key>
OPENAI_API_KEY=<paste your OPENAI API key>
```

### Step 3: Download the Dataset
Get the **PubMed MultiLabel Text Classification Dataset MeSH** from Kaggle:
[Download Here](https://www.kaggle.com/datasets/owaiskhan9654/pubmed-multilabel-text-classification).

### Step 4: Generate Knowledge Graph Data
Run the code in the notebook `VectorVsKG_updated.ipynb` to process the data. This notebook generates the file `PubMedGraph.ttl`. Place this file in the code folder containing the app.

### Step 5: Install Dependencies
Ensure all required Python dependencies are installed:
```bash
pip install -r requirements.txt
```

### Step 6: Run the Streamlit App
Start the application with the following command:
```bash
streamlit run app.py
```

---

## Screenshots

### Application Workflow

![Step 1](https://github.com/user-attachments/assets/03845fa9-6e73-4e23-bc6f-9bded223262b)


![Step 2](https://github.com/user-attachments/assets/c64009aa-be6e-4e21-8392-281da0e1b318)

![Step 3](https://github.com/user-attachments/assets/050ec5fb-be0f-4db2-89ac-84d44878b67f)

![Step 4](https://github.com/user-attachments/assets/8da6ff6f-c577-4eab-84c3-713d1e8e3528)

![Step 5](https://github.com/user-attachments/assets/8e348ab6-44ef-4f73-a202-3aa82ff7521a)

![Step 6](https://github.com/user-attachments/assets/b5f10765-844a-41e7-a257-211bde1d0c82)

![Step 7](https://github.com/user-attachments/assets/f8b1d636-8c04-436c-b411-0abc51c25bc1)

![Step 8](https://github.com/user-attachments/assets/6bf3f2f9-f7b2-45f5-97b8-d6e32c519503)

![Step 9](https://github.com/user-attachments/assets/fa41f5d1-67f9-4b1f-a97c-4be27e2d2360)

![Step 10](https://github.com/user-attachments/assets/5cd2690d-f1bb-44d8-ae22-03408152f1cc)

---

## Notes
- This application demonstrates the synergy of **LLMs**, **knowledge graphs**, and **vector databases** in solving real-world problems.
- Scalability and metadata governance ensure robust and reliable performance in production environments.


   
