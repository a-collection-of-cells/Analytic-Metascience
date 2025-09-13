Outputs

Each run generates timestamped outputs (under code/sample_outputs/ in this submission):

citing_*.csv — citing works metadata

downloaded_files_*/ — PDFs (excluded here for size)

grobid_outputs_/tei/.xml — TEI structured texts

tei_counts_robust_*.csv — counts per citing paper + section

tei_contexts_robust_*.jsonl — evidence windows (±1 sentence)

stance_llm_*.csv — per-paper stance (supportive/neutral/rebuttal)

stance_llm_evidence_*.jsonl — per-window labels + rationales

pointer files — latest_citing_papers_path.txt, latest_download_dir.txt, latest_tei_dir.txt, target_work.json