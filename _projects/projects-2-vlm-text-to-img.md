---
title: "Natural Language Image Search with Visual Language Models (VLMs)"
excerpt: "Built an end-to-end pipeline that integrates geospatial embeddings and text embeddings into a vector database with a custom UI for interactive natural language search. Demonstrates how VLMs enable powerful discovery and labeling in Earth observation data."
collection: projects
youtube_id: "nVYLakhQOGc"
header:
  teaser: /images/projects/projects-2-vlm-text-to-img.png
---

### Overview
This project demonstrates how **Visual Language Models (VLMs)** can be used to perform **text-to-image search** over geospatial data. Using NAIP imagery, I created embeddings for image tiles and stored them in **BigQuery**. Queries are processed via a **text encoder**, and similarity is computed between text and image embeddings to return the most relevant imagery.

Unlike the previous project (where embeddings were provided directly), this workflow involved **generating embeddings end-to-end**:
1. Exporting imagery from Google Earth Engine.
2. Passing tiles through an open-source VLM from Stanford, fine-tuned on satellite imagery + OpenStreetMap tags (a CLIP variant).
3. Building a vector index in BigQuery for scalable similarity search.
4. Developing a **Streamlit UI** to enable interactive natural language queries such as *“planes on a runway”* or *“isolated tree in a field.”*

### Key Components
- **Data Preparation** – NAIP imagery exported via Earth Engine.
- **Embedding Generation** – Applied Stanford’s CLIP-based geospatial VLM to produce image and text embeddings.
- **Vector Database** – Stored embeddings in **BigQuery** with partitioning and indexing for efficient similarity search.
- **Custom UI** – Built a **Streamlit app** for user queries and real-time result visualization, with imagery tiles served via Google Cloud Storage.

### Applications
- **Semantic image retrieval** using natural language (beyond keyword-based search).
- **Label bootstrapping** for machine learning workflows.
- **Exploration of topological features** (e.g., single trees, roads, urban structures) directly from text.
- **Improved accessibility** of large-scale Earth observation archives for non-technical users.

---

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto; margin-bottom: 1em;">
  <iframe
    src="https://www.youtube.com/embed/nVYLakhQOGc?autoplay=1&mute=1&loop=1&playlist=nVYLakhQOGc"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
  ></iframe>
  <img style="max-width: 100%; height: auto; border-radius: 8px; margin-top: 1em;" src="/images/projects/projects-2-vlm-text-to-img.png" alt="VLM Text-to-Image Search Workflow">
</div>
