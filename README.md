# Analytic Metascience – Citing Paper Stance Classifier

This repo contains a semi-automated pipeline to classify citing papers as **Supportive / Neutral / Rebuttal** for a target work.  
Pipeline: OpenAlex → OA PDF acquisition → GROBID TEI → TEI parsing & counts → window extraction (±1 sentence) → local LLM (Ollama) → paper-level aggregation.

## Quickstart (10–15 min demo)
**Prereqs**
- Python 3.10+ with `pip` (or Conda)
- Docker Desktop (for GROBID) with WSL2 on Windows
- Ollama installed locally (`ollama run phi3:mini` once to pull)

**1) Install Python deps**
```bash
pip install -r requirements.txt
# or: conda env create -f environment.yml; conda activate analytic-meta
