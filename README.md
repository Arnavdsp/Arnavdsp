# Arnav Deshpande

### AI / ML Engineer | LLM Systems | RAG | Agents | Evaluation

I build AI systems that are meant to be tested, measured, and used.

My work sits around the engineering layer of modern AI: retrieval pipelines, agentic workflows, evaluation, tool use, inference, and computer vision. I enjoy taking a model or research idea and turning it into something I can actually run, benchmark, inspect, and improve.

Currently pursuing a **B.Tech in Space Science & Engineering at IIT Indore (2023–2027)**.

[LinkedIn](https://www.linkedin.com/in/arnav-deshpande-26a792290/) · [Portfolio](https://arnav-portfolio-arp8-dc7rqha06-arnav-deshpande.vercel.app/) · [Email](mailto:arnavhpd@gmail.com)

---

## What I work on

**AI Systems**
- Retrieval-augmented generation and hybrid search
- Agentic workflows and tool calling
- LLM evaluation and failure analysis
- MCP-based tool servers
- Inference and system-level optimisation

**Machine Learning**
- PyTorch and TensorFlow
- Computer vision and object detection
- Transformers, ViTs, DETR / RT-DETR
- Fine-tuning, LoRA and DPO
- Representation learning and clustering

**Engineering**
- Python and C++
- FastAPI
- Docker
- LangGraph
- Hugging Face
- Vector retrieval
- Evaluation pipelines

---

## Projects I would start with

### [edgar-mcp](https://github.com/Arnavdsp/edgar-mcp)

**MCP server + evaluation harness for SEC EDGAR data**

Built an MCP server exposing six tools over SEC EDGAR filing data, together with an evaluation harness built around a gold question set.

The interesting part for me was not just exposing tools. It was making the system testable and checking whether the tools actually supported reliable answers.

**Focus:** MCP · tool calling · retrieval · evaluation · Python

---

### [DocuMind](https://github.com/Arnavdsp/DocuMind)

**Document question answering with evidence-aware retrieval**

A document QA system for PDFs using text extraction, hybrid retrieval, reranking, citations, and evidence-aware answering.

A key design goal is that the system should be able to recognise when the retrieved evidence is insufficient instead of confidently producing an unsupported answer.

**Focus:** RAG · hybrid retrieval · reranking · citations · LLMs

---

### [Automatron](https://github.com/Arnavdsp/Automatron)

**Multi-agent decision-support workflows**

An agentic workflow system where multiple components can perform specialised tasks, validate intermediate results, and route important decisions through human approval.

The project explores a question I find increasingly important in agentic systems: how do we make an agent workflow more reliable than simply giving an LLM more autonomy?

**Focus:** agents · orchestration · validation · human-in-the-loop

---

### [Evaluation Assurance](https://github.com/Arnavdsp/Evaluation-assurance-for-Deccan-AI)

**Finding PASS verdicts that deserve a second look**

A research prototype exploring whether execution-side signals can identify cases where an LLM evaluator incorrectly returns PASS.

The experiments use synthetic data with known ground truth. The system ranks questionable PASS decisions for human review rather than attempting to replace the evaluator completely.

**Focus:** evaluation · failure detection · ranking · human review · reliability

---

### [ai-systems-lab](https://github.com/Arnavdsp/ai-systems-lab)

**An engineering notebook for AI systems**

A collection of small implementations and experiments covering areas such as:

- DAG-based planning
- retrieval and rank fusion
- evaluation metrics
- agent workflows
- inference and memory estimates
- experiments around failure modes

I use this repository as a place to test ideas, record observations, and understand the trade-offs behind AI systems rather than treating every experiment as a finished product.

**Focus:** experimentation · agents · RAG · evaluation · inference

---

### [DRDO Internship](https://github.com/Arnavdsp/DRDO-Internship-Overview)

**Tiny-object detection in aerial imagery**

Internship work involving object detection on the VisDrone2019-DET dataset, with experiments around RT-DETR and small-object detection.

The work also involved studying image resolution, super-resolution, detection performance, and the challenges of detecting small objects in aerial imagery.

**Focus:** computer vision · RT-DETR · object detection · aerial imagery

---

## Research

Alongside AI engineering, I have worked on research-oriented ML projects across astrophysics and computer vision.

### [Lost in the Middle](https://github.com/Arnavdsp/lost-in-the-middle-2026)

Reproduction work around the "Lost in the Middle" long-context retrieval phenomenon using the authors' data and prompts with current models.

### [GRB Analysis](https://github.com/Arnavdsp/Research-Internship-IITI-DAASE-Overview)

Research on gamma-ray burst light curves using dimensionality reduction and clustering, including UMAP and HDBSCAN.

### [Optical Transient Classification](https://github.com/Arnavdsp/Optical-Transient-Hierarchial-Classification)

A two-stage classification system for optical transients using light-curve features from TNS labels, ZTF, and TESS photometry.

### [Bridge Detection](https://github.com/Arnavdsp/Water-Bridge-Detection-Through-Satellite-Imagery)

YOLOv8-OBB experiments for detecting bridges over water in aerial satellite imagery.

---

## How I approach projects

I generally follow the same loop:

**Build → Measure → Inspect failures → Change one thing → Measure again**

That means I try not to stop at "the model works."

For systems involving LLMs, I am particularly interested in questions such as:

- Does retrieval actually improve the answer?
- When should a system abstain?
- What happens when an agent chooses the wrong tool?
- How do we evaluate an agent when the final answer alone is not enough?
- Where does latency or memory become the bottleneck?
- Which part of the system is actually responsible for an improvement?

---

## Technical stack

**Languages**

Python · C++ · JavaScript

**Machine Learning**

PyTorch · TensorFlow · Hugging Face Transformers · YOLO · RT-DETR · ViT · DETR

**LLM / AI Systems**

RAG · Hybrid Retrieval · Reranking · LangGraph · MCP · Agentic Workflows · LoRA · DPO

**Backend / Infrastructure**

FastAPI · Docker · Git · Hugging Face Spaces

**Data / Scientific Computing**

NumPy · Pandas · OpenCV · scikit-learn

---

## Experience

**DRDO / DRDL — Research / Internship**

Worked on computer vision and tiny-object detection using aerial imagery, with experiments involving VisDrone2019-DET, RT-DETR, image enhancement, and detection performance.

**IIT Indore**

B.Tech in Space Science & Engineering, with research and project work spanning astrophysics, computer vision, machine learning, and AI systems.

---

## What you will find in my repositories

I keep a distinction between:

**Experiment**

Something I built to answer a technical question.

**Research**

Something where I am reproducing, testing, or extending an existing idea.

**Project**

A more complete system intended to be used or demonstrated.

**Production**

A standard I only use when the system has actually been deployed and operated under real production conditions.

I care about that distinction because being able to explain what a system does, how it was evaluated, where it fails, and what I would change next matters more to me than making every project sound impressive.

---

## Currently exploring

- Reliable agentic systems
- Evaluation and observability for LLM applications
- Retrieval quality and context selection
- MCP and tool-using systems
- Efficient inference
- AI engineering patterns for production systems

---

## Connect

[LinkedIn](https://www.linkedin.com/in/arnav-deshpande-26a792290/)

[Portfolio](https://arnav-portfolio-arp8-dc7rqha06-arnav-deshpande.vercel.app/)

[Email](mailto:arnavhpd@gmail.com)
