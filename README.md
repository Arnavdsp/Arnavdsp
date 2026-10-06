# Arnav Deshpande

**AI / ML Engineer** · LLM systems, retrieval, agents, evaluation

I build LLM and ML systems that say when they don't know. Most of my projects ship with the evaluation that tells you where they break, because a system that is confidently wrong costs more than one that refuses.

B.Tech, Space Science & Engineering, IIT Indore (2023–2027).

[LinkedIn](https://www.linkedin.com/in/arnav-deshpande-26a792290/) · [Portfolio](https://arnav-portfolio-arp8-dc7rqha06-arnav-deshpande.vercel.app/) · [Email](mailto:arnavhpd@gmail.com)

---

## Experience

**DRDO, DRDL** · Deep Learning and ML Internship, Transformer based  Computer Vision · *completed June 2026*
Tiny-object detection in aerial imagery with RT-DETR and YOLO on VisDrone2019-DET, on constrained compute. I tested how image resolution and super-resolution (ESRGAN, SwinIR) affect detection of objects only a few pixels wide. Two findings: NWD-based scoring gave a more reliable signal than IoU for tiny boxes, and super-resolution tuned for the detector mattered more than super-resolution tuned for visual quality.

**[`DRDO-Internship-Overview`](https://github.com/Arnavdsp/DRDO-Internship-Overview)**

**IIT Indore** ·Machine Learning Internship

Scientific ML on gamma-ray burst light curves, then computer vision and LLM systems. The habit I took from research: before trusting a clean result, check whether noise alone could produce it.

[`DAASE-Internship-Overview`](https://github.com/Arnavdsp/Research-Internship-IITI-DAASE-Overview)
---

## Selected Projects

### [edgar-mcp](https://github.com/Arnavdsp/edgar-mcp) · MCP server + eval harness
Six MCP tools over SEC EDGAR filings, scored against 25 hand-verified questions run 3 times each. Each response reports which XBRL tag matched and which tags were tried. If the top two company matches score within 0.05 of each other, the tool refuses rather than answering about the wrong filer. Results are broken out by question type instead of averaged: lookups pass 83%, restatement questions 17%. The README lists the failure modes.
`MCP` `tool calling` `retrieval` `evaluation`

### [DocuMind](https://github.com/Arnavdsp/DocuMind) · document Q&A with citations and abstention
PDF and image Q&A that retrieves by vector similarity, then reranks with lexical overlap or a cross-encoder. Every answer is tied to chunk, page and snippet. When evidence is too thin, a code path returns "not enough information" before the model can make up an answer. Sparse pages fall back to Tesseract OCR, which records its confidence and flags low-quality extractions.
`RAG` `reranking` `pdfplumber` `Tesseract` `FastAPI` `Docker` · [demo](https://huggingface.co/spaces/ADP123456/DocuMind)

### [Aura](https://github.com/Arnavdsp/Aura-The-Mental-Wellness-Coach)

A multimodal mental wellness coach built with **Gemma 3n**, combining conversational AI, OCR, and safety-aware response handling. The project also explores **LoRA fine-tuning and DPO** for adapting model behaviour.

`Gemma 3n` · `Multimodal AI` · `OCR` · `LoRA` · `DPO` . [demo](https://huggingface.co/spaces/ADP123456/aura-wellness-coach)

### [Automatron](https://github.com/Arnavdsp/Automatron) · multi-agent decision support
LangGraph workflows with four roles: coordinator, researcher, analyst and executor. Each role has a tool allowlist enforced in code. A deterministic verifier rejects any decision brief containing a number that no tool produced, and sends it back through a capped revision loop. Every run stops at a human approval gate and is recorded in a hash-chained audit log. A model router fails over across 6 providers on rate limits or context overflow. Deployed to Cloud Run through GitHub Actions. All bundled data is synthetic. ( Currently not Live...Do Contact me if you want to see it in action or know more about it)
`LangGraph` `LlamaIndex` `Qdrant` `FastAPI` `Cloud Run` · [live](https://automatron-413625269952.us-central1.run.app/)

### [Evaluation Assurance](https://github.com/Arnavdsp/Evaluation-assurance-for-Deccan-AI) · auditing an LLM judge
A research prototype on synthetic data with known ground truth. It asks: when an automated evaluator says PASS, which of those verdicts should a human re-check? It ranks PASS verdicts by execution-side signals the evaluator never saw: database read-back, tool-argument audits, replay checks. With a 20% review budget it catches 48.4% of wrong PASSes, against 20.4% for random spot-checks. At 5% review, its precision is 92%. The failure modes are simulated, and the README says so.
`evaluation` `scikit-learn` `synthetic data`


## Research & Other Work

| Project | What it is |
|---|---|
| [Lost in the Middle (2026)](https://github.com/Arnavdsp/lost-in-the-middle-2026) | Replication on `gpt-oss-20b`: with the answer mid-prompt, accuracy (6.7%) fell below the no-context baseline (15.0%) |
| [GRB Analysis](https://github.com/Arnavdsp/Research-Internship-IITI-DAASE-Overview) | Clustering 226 gamma-ray burst light curves; a synthetic-noise control showed clean clusters can come from noise alone |
| [Optical Transient Classification](https://github.com/Arnavdsp/Optical-Transient-Hierarchial-Classification) | Two-stage classifier for transients, then supernova subtypes, with variance reported across splits |
| [Bridge Detection](https://github.com/Arnavdsp/Water-Bridge-Detection-Through-Satellite-Imagery) | YOLOv8-OBB on GLH-Bridge and DOTA, with dataset work for heavy class imbalance |
| [Quick-Commerce Case Study](https://github.com/Arnavdsp/Quick-Comerce-Case-Study) | Unit economics of Blinkit, Instamart and Zepto from public filings, with a Streamlit simulator |

---

## Stack

**LLM systems** `LangGraph` `LlamaIndex` `MCP` `Qdrant` `Sentence Transformers` `Hugging Face`

**ML / CV** `PyTorch` `scikit-learn` `RT-DETR` `YOLO` `SAHI` `ESRGAN` `SwinIR` `OpenCV`

**Engineering** `Python` `FastAPI` `Docker` `pytest` `GitHub Actions` `Cloud Run`

---

## How I Work

Build it, measure it, find where it breaks, then fix that and measure again. The questions I keep coming back to:

- When should a system answer, and when should it refuse?
- Did retrieval improve the answer, or only make it longer?
- How do you score an agent on its intermediate steps, not just its final output?
- What happens downstream when one tool call silently returns something wrong?
- Can you trust the evaluator?

## Currently Exploring

Agent evaluation beyond final answers · retrieval quality measurement · MCP tool design · efficient local inference

---

arnavhpd@gmail.com · [LinkedIn](https://www.linkedin.com/in/arnav-deshpande-26a792290/) · [Portfolio](https://arnav-portfolio-arp8-dc7rqha06-arnav-deshpande.vercel.app/)
