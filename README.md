# DataHub Copilot - Metadata-Aware Code & Query Generator 🚀

An autonomous AI Agent built for **The Agent Hackathon by DataHub**. It integrates with DataHub's MCP Server and Agent Context Kit to read enterprise data schemas and generate accurate SQL queries, Airflow DAGs, and transformation scripts without hallucinations.

---

## 🌟 Key Features

* **Metadata-Aware Context Retrieval:** Fetches table schemas, column data types, and lineage directly from DataHub catalog.
* **Zero-Hallucination SQL Generation:** Uses real-time metadata context so LLMs never invent non-existent table or column names.
* **Pipeline Automation:** Generates production-grade Airflow DAGs for dataset processing.
* **DataHub MCP Server Integration:** Seamless connection using DataHub API and SDKs.

---

## 🏗️ Architecture & Workflow

1. **User Prompt:** Analyst inputs a natural language query (e.g., *"Show top revenue generating items"*).
2. **DataHub Context Lookup:** The agent queries DataHub's MCP Server to locate relevant datasets, schemas, and upstream dependencies.
3. **LLM Code Generation:** Schema-informed prompt is processed by the AI model to output optimized SQL / DAG code.
4. **Execution & Validation:** Agent validates the generated code structure against DataHub metadata rules.

---

## 💻 Quickstart Guide

### Prerequisites
* Python 3.9+
* DataHub Instance / API Token
* OpenAI / LLM API Key

### Installation

```bash
git clone [https://github.com/dreamplays-official/datahub-copilot-ai.git](https://github.com/dreamplays-official/datahub-copilot-ai.git)
cd datahub-copilot-ai
pip install -r requirements.txt

