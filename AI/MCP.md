# MCP (Model Context Protocol) Overview

## What is MCP?

* **MCP (Model Context Protocol)** is an open-source protocol designed for standardizing how applications provide context to Large Language Models (LLMs).
* Think of MCP as a **USB-C port** analogy for AI, enabling standardized, efficient connections between LLMs and various data sources or tools.

---

## MCP as USB-C Analogy

* Without MCP: Each AI model or agent requires manual configuration (individual "ports") for each data source/tool, creating complexity.
* With MCP: Like USB-C, MCP provides a unified standard protocol, making it easy to connect numerous tools and data sources with minimal configuration.

---

## Background: Why MCP was Introduced?

### Traditional LLM Usage

* LLMs like GPT, LLaMA, or Mistral are pre-trained models.
* Each model has a **knowledge cutoff date**, meaning it's trained on data available up to a certain point (e.g., GPT-3.5 trained on data until 2021).
* Limitations:

  * Cannot handle real-time or updated information beyond its training date.

### RAG (Retrieval-Augmented Generation)

* Solves the issue partially by integrating custom or private data:

  * Custom documents are stored in **vector databases**.
  * Queries are processed by searching this database for relevant information.
  * However, it still cannot handle real-time queries or rapidly updating data.

### Agents and Tools

* To handle real-time information and broader data access, **agents** and **tools** were introduced:

  * Frameworks: CrewAI, LangGraph.
  * Tools: SERP APIs (Google Search), Wikipedia API, DuckDuckGo, etc.
* Agents dynamically choose the right tool based on the user's query.
* Challenges:

  * Requires extensive manual configuration ("glue code") for each tool.
  * Managing many tools (100+) becomes complicated, especially with tool updates or configuration changes.

---

## How MCP Solves the Problem

* MCP acts as an intermediary **standardized medium** between LLMs and multiple tools.
* Reduces complexity by eliminating individual manual configurations.
* Automatically manages integrations, configurations, and updates through the MCP standard.

### Key Components of MCP:

* **MCP Host**: Where MCP runs (examples: Cursor AI, Cloudy, Carori).
* **MCP Client**: Communicates requests from the host to the server.
* **MCP Server**: Connects to multiple tools and data sources, handling integrations and configurations.

### Workflow:

1. User sends input → MCP Host receives it.
2. MCP Client communicates with MCP Server to identify available tools.
3. LLM analyzes the query along with available tools to decide the best tool for retrieving the required context.
4. MCP Client uses selected tool (via MCP Server) to fetch real-time data/context.
5. Data fetched becomes context provided back to the LLM.
6. LLM processes the provided context and query, then returns the final output.

---

## Advantages of Using MCP:

* Simplifies managing multiple integrations and real-time contexts.
* Centralizes configuration, significantly reducing the overhead of maintaining and updating tool integrations.
* Enhances efficiency and scalability when building complex AI-driven applications.

---

## Practical Use Cases:

* Real-time news, weather updates, financial data.
* Multi-tool agent applications (search, translation, code execution).
* Efficient context management for complex AI tasks.

---

### Resources/Tools used:
**Youtube Video:** https://www.youtube.com/watch?v=vbqc7YddmBE&list=PLkz_y24mlSJYG_cg0oVYMRSEv2o-iGmhG&index=3
**Transcript Generator:** https://tactiq.io/tools/youtube-transcript


