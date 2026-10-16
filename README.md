<div align="center">
  
# Pleatwright

<p align="center">
  <img src="https://github.com/user-attachments/assets/90f89d9c-a327-493d-b038-a01933c2522e" alt="2026-10-12-0037-scorpion_overview" width="100%">
</p>
 
▶️ [pleatwright demo](https://www.youtube.com/watch?v=8e9vlsNsiY0)
 
</div>
---
 
Pleatwright is an AI-native CAD software for origami design. It uses a neuro-symbolic approach that leverages LLM for reasoning and decision-making and computational-origami algorithms for deterministic solving.
 
## ⚙️ Overview

Users send a query (a description of the desired subject), a HF model generates a 3D mesh of the subject, and an LLM (Sonnet 5) uses MCP tools to take measurements of the appendages and draw a tree graph of the structure. A computational origami algorithm is then used to map the tree graph onto a square grid and then fill in creases to produce a flat-foldable base. The base is then shaped with a BFS algorithm to produce a stick-figure-like model that can be further shaped by Origami artists.

 
The computational algorithm used to build crease patterns from trees has two steps:
 
> **1. Packing** — an initial packing step maps out regions of the paper (flaps) for each branch of the tree, and then
>
> **2. Solving** — a solving step determines the placement and direction of creases and creates a crease pattern for a base.
 
## 📚 Acknowledgements
 
This project was inspired heavily by a paper from Google Deepmind researchers and leading Origami artists (including, notably, the founding father of modern Origami design, Robert J. Lang), cited below:
 
> Zahavy, T., Hou, S., Tumiel, T., Doran, J., Faccio, F., Feng, X., ... Singh, S. (2026). *COrigami: An AI Pipeline for Co-Designing Flat-Foldable Visually Recognisable Origami*. arXiv. https://arxiv.org/abs/2606.26299
 
