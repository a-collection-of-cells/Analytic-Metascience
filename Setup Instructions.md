Setup Instructions
1. Start GROBID (PDF → TEI conversion)
docker run --rm -it -p 8070:8070 -p 8071:8071 lfoppiano/grobid:latest


Check it is alive:

curl http://localhost:8070/api/isalive

2. Start Ollama (local LLM)

Pull and run the model once:

ollama run phi3:mini

3. Run the Notebook

Open:

code/thesis.ipynb


Run cells in order:

Step 1: Retrieve citing works (OpenAlex).

Step 2: Download PDFs (OpenAlex/Unpaywall).

Step 3: Convert PDFs → TEI (GROBID).

Step 4: Parse TEI and extract citation windows.

Step 5: LLM stance classification and aggregation.

Step 6: Outputs (CSV/JSONL artefacts + pointer files).