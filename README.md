My background spans a wide range of end-to-end projects across **Machine Learning, Deep Learning, and Generative AI**. I specialize in building complex, production-ready AI workflows using:
* **Agentic AI & Orchestration** (LangGraph, Multi-Agent systems)
* **Retrieval-Augmented Generation (RAG)**
* **MLOps & Continuous Training Pipelines**
* **Enterprise Cloud AI** (Snowflake Cortex, Snowpark, Azure and IBM cloud)

Below, you will find documentation for two featured architectures that provide a quick glance at my engineering approach.

---

## 📂 Featured Architectures

### 1. Autonomous Data Migration System (Multi-Agent Architecture)
* **Files:** `Data Migration Agent End-to-End Blog.pdf`, `Data-Migration-Agent-High-Level.pdf`
* **Overview:** A source-agnostic, multi-agent framework built with Snowflake Cortex and Snowpark. It replaces manual ETL scripts with an intelligent, self-healing migration workforce.
* **Key Highlights:**
  * **Parallel Execution:** Master agent orchestrates sub-agents to process multiple tables concurrently.
  * **Automated Schema Translation:** Uses LLMs to translate legacy SQL Server/Oracle DDLs to Snowflake syntax.
  * **Intelligent Security:** Automatically scans metadata to detect PII and applies dynamic masking policies.
  * **Automated Reconciliation:** Dual-source profiling ensures 100% data integrity without manual intervention.

### 2. Self-Healing MLOps Pipeline & Agentic AI
* **File:** `MLOps Churn Modeling and Agentic AI.pdf`
* **Overview:** An end-to-end, closed-loop machine learning pipeline natively built on Snowflake to predict student churn, featuring a GenAI interface for business users.
* **Key Highlights:**
  * **Automated Drift Detection:** A "Watchdog" agent monitors data using Jensen-Shannon Distance and triggers retraining when necessary.
  * **Champion vs. Challenger System:** New models are automatically trained, shadow-tested, and promoted only if they outperform the current production model.
  * **Agentic Simulation Engine:** A Cortex-powered Text-to-SQL and simulation bot allows non-technical advisors to run live "what-if" scenarios (e.g., *"If we increase attendance by 10 hours, how does the churn risk change?"*) and retrieves prescriptive intervention strategies.
 
### 3. AI Co-Pilot: Territory & Quota (T&Q) System Architecture
* **File:** `AI Co-Pilot Territory and Quota System Architecture.pdf` *AI Co-Pilot.pdf*
* **Overview:** An enterprise-grade Snowflake AI Agent designed to orchestrate Territory and Quota planning using a dual-engine approach
* **Dual-Engine Logic:** Combines Cortex Analyst for semantic read-only reporting with Custom Python Workflow Tools for secure database mutations
* **Context-Aware Routing:** Dynamically adapts data writes based on the planning cycle, writing Annual Planning directly to production while routing In-Year changes to staging tables for Sales Ops approval
* **Strict Governance & Security:** Enforces Row-Level Security (RLS/RBAC) and mandates a PREVIEW -> CONFIRM -> EXECUTE pattern to prevent LLM hallucinations during financial updates
