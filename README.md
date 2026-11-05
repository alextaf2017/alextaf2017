<div align="center">

<a href="https://github.com/alextaf2017">
  <img src="https://capsule-render.vercel.app/api?type=rect&height=210&color=0:0D1117,45:14243A,100:1F6FEB&text=ALESSIO%20TAFUNI&fontColor=F0F6FC&fontSize=48&fontAlignY=40&desc=DATA%20SCIENCE%20%20%E2%80%A2%20%20ARTIFICIAL%20INTELLIGENCE%20%20%E2%80%A2%20%20ACTUARIAL%20SCIENCE&descAlignY=62&descSize=13" width="100%" alt="Alessio Tafuni — Data Science, Artificial Intelligence and Actuarial Science" />
</a>

<br/>

<a href="https://github.com/alextaf2017"><img src="https://img.shields.io/badge/GitHub-alextaf2017-161B22?style=for-the-badge&logo=github&logoColor=F0F6FC" alt="GitHub profile" /></a>
<a href="https://www.linkedin.com/in/alessio-tafuni-9544a4264/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn profile" /></a>

<br/><br/>

**Building intelligent systems. Measuring risk. Turning data into decisions.**

</div>

---

## About

Hi, I'm Alessio Tafuni, I have a Master's degree in Statistics (LM-83) with honours and I work at the intersection of statistics, machine learning, and generative AI.

Today, my focus is on LLM and RAG-based solutions. I am keen on applying analysis, modeling, and forecasting to actuarial, financial, and scientific problems using an evidence-based approach: measuring, comparing, and honestly addressing where a model falls short. 

## Selected projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>01 · RAG Assistant for Motor Insurance</h3>
      <a href="https://github.com/alextaf2017/rag-assicurazioni">
        <img src="https://img.shields.io/badge/VIEW_PROJECT-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="View RAG Assistant project" />
      </a>
      <p>A Retrieval-Augmented Generation assistant for Italian motor insurance documentation.</p>
      <ul>
        <li>Hybrid retrieval: dense embeddings, BM25 and Reciprocal Rank Fusion</li>
        <li>Local LLM inference with Llama 3.1 8B and Ollama</li>
        <li>Answers grounded in source documents and page references</li>
        <li>FastAPI service and Docker</li>
      </ul>
      <p><strong>Evaluation snapshot:</strong> 0.82 hit@5 across 38 manually annotated questions. This is a preliminary result on a small evaluation set, not a general performance guarantee.</p>
      <p>
        <img src="https://img.shields.io/badge/RAG-161B22?style=flat-square" alt="RAG" />
        <img src="https://img.shields.io/badge/Hybrid_Search-161B22?style=flat-square" alt="Hybrid search" />
        <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h3>02 · Insurance Claims Risk Platform</h3>
      <a href="https://github.com/alextaf2017/insurance-risk-platform">
        <img src="https://img.shields.io/badge/VIEW_PROJECT-1F6FEB?style=for-the-badge&logo=github&logoColor=white" alt="View Insurance Risk Platform project" />
      </a>
      <p>An insurance data engineering and risk analytics project built around the freMTPL2 dataset.</p>
      <ul>
        <li>Apache Spark and Apache Iceberg</li>
        <li>Bronze / Silver / Gold data lake architecture</li>
        <li>Data quality checks and data contracts</li>
        <li>Deterministic train/test split</li>
      </ul>
      <p><strong>Current status:</strong> Milestone 1 completed. Statistical analysis, actuarial models, machine learning and deployment are planned future milestones.</p>
      <p>
        <img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="Apache Spark" />
        <img src="https://img.shields.io/badge/Apache_Iceberg-161B22?style=flat-square&logo=apache&logoColor=white" alt="Apache Iceberg" />
        <img src="https://img.shields.io/badge/Data_Quality-161B22?style=flat-square" alt="Data quality" />
        <img src="https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="SQL" />
      </p>
    </td>
  </tr>
</table>

## Architecture at a glance

<details open>
  <summary><strong>RAG · Insurance document intelligence</strong></summary>

  ```mermaid
  flowchart LR
      A[Insurance PDFs] --> B[Text extraction & cleaning]
      B --> C[Chunking]
      C --> D[Embeddings]
      C --> E[BM25 index]
      D --> F[Hybrid retrieval]
      E --> F
      F --> G[Reciprocal Rank Fusion]
      G --> H[Local LLM · Llama 3.1 8B]
      H --> I[Answer with source references]
  ```
  <p><sub>Conceptual view of the implemented retrieval and answer-generation workflow.</sub></p>
</details>

<details open>
  <summary><strong>Insurance risk platform · Data lake foundation</strong></summary>

  ```mermaid
  flowchart LR
      A[freMTPL2 dataset] --> B[Raw data]
      B --> C[Bronze]
      C --> D[Silver]
      D --> E[Gold]
      E --> F[Deterministic train/test split]

      subgraph Platform
        G[Apache Spark]
        H[Apache Iceberg]
        I[S3-compatible storage]
        J[PostgreSQL JDBC catalog]
      end

      C -.-> G
      D -.-> H
      E -.-> I
      H -.-> J
  ```
  <p><sub>Milestone 1 data foundation. Modeling and downstream analytics remain on the roadmap.</sub></p>
</details>

## Technologies

<div align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/SQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL" />
<img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="Apache Spark" />
<img src="https://img.shields.io/badge/Apache_Iceberg-161B22?style=for-the-badge&logo=apache&logoColor=white" alt="Apache Iceberg" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Ollama-161B22?style=for-the-badge&logoColor=white" alt="Ollama" />
<img src="https://img.shields.io/badge/ChromaDB-161B22?style=for-the-badge&logoColor=white" alt="ChromaDB" />

</div>

## 📊 GitHub Overview

### GitHub Profile Statistics

![GitHub Statistics](./github-stats.svg)

### 🧰 Technologies & Tools

**Programming & Data Analysis**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

**Machine Learning & Artificial Intelligence**

![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-102A43?style=for-the-badge)
![NLP](https://img.shields.io/badge/NLP-00897B?style=for-the-badge)
![Generative AI](https://img.shields.io/badge/Generative_AI-7B61FF?style=for-the-badge)
![LLM](https://img.shields.io/badge/LLM-412991?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-6C47FF?style=for-the-badge)

**Data Engineering & Development**

![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F61?style=for-the-badge)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Cloud & Business Intelligence**

![Microsoft Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

### Contribution Activity

![Contribution Activity](./github-contributions.svg)
## Current focus

- Strengthening the data foundation of the insurance risk platform.
- Exploring statistical and actuarial approaches to insurance claims.
- Building reliable retrieval and evaluation workflows for insurance-document AI.

## Connect

<div align="center">

<a href="https://www.linkedin.com/in/alessio-tafuni-9544a4264/"><img src="https://img.shields.io/badge/LinkedIn-Let's%20connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" /></a>
<a href="https://github.com/alextaf2017"><img src="https://img.shields.io/badge/GitHub-Follow-161B22?style=for-the-badge&logo=github&logoColor=white" alt="Follow on GitHub" /></a>

<br/><br/>

<sub>Data · Engineering · Intelligence</sub>

</div>
