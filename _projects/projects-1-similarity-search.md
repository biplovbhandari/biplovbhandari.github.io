---
title: "Similarity Search with Foundational Models and Vector Databases"
excerpt: "Built an end-to-end system that integrates geospatial embeddings, scalable vector storage, and a custom UI for interactive similarity search. Demonstrates how foundational models can accelerate labeling and discovery in Earth observation data."
collection: projects
youtube_id: "04U0uyARMgw"
header:
  teaser: /images/projects/projects-1-similarity-search.png
---

### Overview
This project showcases how **Earth Observation Foundational Models (EOFM)** can power geospatial similarity search at scale. Using **Clay embeddings** derived from NAIP imagery, I developed a workflow to store and query embeddings with **BigQuery’s vector search capabilities**, and built a **custom UI in Google Earth Engine** to explore results interactively.

### Key Components
- **Embedding Generation** – Extracted feature embeddings from Clay (EOFM) for NAIP imagery stored in parquet format.
- **Vector Database** – Stored embeddings in **BigQuery**, using partitioning and vector indexing for fast similarity search.
- **Custom UI** – Developed an Earth Engine interface for visualizing search results and exploring geospatial similarity interactively.

### Applications
- **Bootstrap labeling efforts** by finding visually similar samples.
- **Data discovery** across large remote sensing archives.
- **Interactive exploration** for analysts and decision-makers.

---

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto; margin-bottom: 1em;">
  <iframe
    src="https://www.youtube.com/embed/04U0uyARMgw?autoplay=1&mute=1&loop=1&playlist=04U0uyARMgw"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
  ></iframe>
  <img style="max-width: 100%; height: auto; border-radius: 8px; margin-top: 1em;" src="/images/projects/projects-1-similarity-search.png" alt="Similarity Search UI Screenshot">
</div>
