---
title: "Agentic Workflows with Foundational Models and Geospatial Toolbelts"
excerpt: "Developed an end-to-end system that leverages agentic workflows, custom geospatial tools, and Google Cloud services to enable natural language-driven geospatial analysis with multimodal outputs."
collection: projects
youtube_id: "hxXAKDts77s"
header:
  teaser: /images/projects/projects-3-agentic-workflow.png
---

### Overview
This project demonstrates how **agentic workflows** can orchestrate complex geospatial analysis by combining **Foundational Models**, **custom geospatial toolsets**, and **Google Cloud services**.

Using the **Google Agent Development Kit (ADK)** as the LLM orchestrator, the system interprets natural language queries, selects the right geospatial tools, and delivers outputs as maps, tables, or captions. In this example, an **open-source multimodal change detection model** is integrated into the workflow, producing both **change masks** and **textual captions**.

The pipeline leverages:
- **Vertex AI** for online model inference,
- **Google Cloud Storage (GCS)** for imagery and tile storage,
- **BigQuery** for structured/tabular data, and
- A **Streamlit-based chat UI** for user interaction.

### Key Components
- **LLM Orchestrator** – Google ADK (Gemini) manages tool selection, memory, and response generation.
- **Custom Geospatial Toolbelt** – Tools for change detection, counting, map export, raster/vector operations, and custom Python execution.
- **Cloud Services Integration** – Vertex AI (inference), GCS (image storage), BigQuery (tabular/vector storage).
- **User Interface** – Streamlit-based chat app enabling conversational interaction and multimodal results.

### Applications
- **Change Detection at Scale** – Captioned + masked results for monitoring land-use, urban expansion, and environmental changes.
- **Conversational GeoAI** – End-users can run geospatial analysis tasks with natural language queries.
- **Customizable Workflows** – Extendable toolbelt supports flexible geospatial pipelines (e.g., counting features, saving maps, running raster operations).
- **Decision Support** – Bridges foundational models and operational geospatial workflows for policy, planning, and sustainability.

---

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto; margin-bottom: 1em;">
  <iframe
    src="https://www.youtube.com/embed/hxXAKDts77s?autoplay=1&mute=1&loop=1&playlist=hxXAKDts77s"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
  ></iframe>
  <img style="max-width: 100%; height: auto; border-radius: 8px; margin-top: 1em;" src="/images/projects/projects-3-agentic-workflow.png" alt="Agentic Workflow Architecture Diagram">
</div>
