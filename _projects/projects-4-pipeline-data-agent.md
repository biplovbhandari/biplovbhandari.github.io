---
title: "Pipeline Data Agent - Pipeline Analytics with Google ADK"
excerpt: "Built an intelligent data analysis agent using Google's Agent Development Kit (ADK) and Claude 3.5 Haiku for advanced pipeline data analytics. Features modular tool architecture for retrieval, pattern recognition, and anomaly detection across 23.8M+ pipeline transaction records."
collection: projects
youtube_id: "mh05q4R6FuM"
header:
  teaser: /images/projects/projects-4-pipeline-data-agent.png
---

### Overview
This project demonstrates the power of **Google's Agent Development Kit (ADK)** combined with **Claude 3.5 Haiku** to create an intelligent data analysis agent. The agent processes a massive pipeline dataset (23.8M+ records) and can handle queries ranging from simple data retrieval to complex pattern recognition and anomaly detection.

### Key Components
- **Google ADK Architecture** – Implements ADK's modular design patterns with high-level, flexible tools that the LLM orchestrates dynamically.
- **Pipeline Data Processing** – Analyzes 13-column dataset with pipeline names, scheduled quantities, gas days, receipt/delivery indicators, categories, and state information.
- **Three-Tier Tool System** – Organized into Retrieval Tools (basic queries), Pattern Tools (clustering & correlations), and Anomaly Tools (outlier detection).
- **LLM Orchestration** – Claude 3.5 Haiku combines multiple tool calls to solve complex analytical queries without requiring specific functions for each use case.

### Technical Architecture
- **Retrieval Layer** – Volume aggregation, pipeline ranking, net flow calculations, time series analysis
- **Pattern Recognition** – Seasonal analysis, monthly trends, correlation detection, K-means clustering
- **Anomaly Detection** – Multi-method outlier detection using z-score, rolling windows, change detection, and percentile-based methods
- **Modular Design** – Tools are composable and reusable across different query types, following ADK best practices

### Applications
- **Pipeline Operations** – Monitor gas flow patterns across utilities, industrial, production, and storage categories
- **Seasonal Analysis** – Identify seasonal trends and compare winter vs. summer delivery patterns
- **Anomaly Detection** – Automatically detect unusual pipeline activities and transaction outliers
- **Multi-dimensional Analytics** – Aggregate data across time, geography, and transaction types for comprehensive insights

### Dataset Scope
The agent processes pipeline transaction data with:
- **23.8M+ Records** across utilities (LDC), industrial, production, and storage categories
- **Transaction Types** – Receipts (+1 inflow) vs deliveries (-1 outflow)
- **Geographic Coverage** – State-level pipeline activity analysis
- **Temporal Analysis** – Multi-granularity time series from daily to yearly patterns

---

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto; margin-bottom: 1em;">
  <iframe
    src="https://www.youtube.com/embed/mh05q4R6FuM?autoplay=1&mute=1&loop=1&playlist=mh05q4R6FuM"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
  ></iframe>
  <img style="max-width: 100%; height: auto; border-radius: 8px; margin-top: 1em;" src="/images/projects/projects-4-pipeline-data-agent.png" alt="Pipeline Data Agent Architecture Diagram">
</div>
