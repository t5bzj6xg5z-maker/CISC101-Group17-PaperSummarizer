# CISC101-Group17-PaperSummarizer

Group Members:
- Zakkary
- Emmett
- Nathan

Research Paper Summarizer

This project develops a structured summarizer for research papers, adhering to the PS2 specification.

Features:

Provide a concise summary of each section, approximately 100–150 words. 
Conclude with a comprehensive summary, no longer than 400 words.  
Ensure summaries cater to both experts and laypersons.  
Include a glossary of technical terms.  
Implement checks and warnings for missing or incomplete sections.  Highlight key contributions, 
identifying 3–5 significant points.
Simplify equations and technical terms for clarity.
Module Architecture

Intake & Setup — Normalize sections, detect issues, and chunk text during intake and setup.
Section Loop — Summarize each section, keeping in mind the PS2 constraints.
Guardrails — Guardrails prevent hallucinations and enforce evidence rules.
Rendering & Refinement — Rendering and refinement involve formatting outputs and ensuring clarity.
Key Contributions Extractor — Key Contributions Extractor:  Highlight the main contributions.
Equation & Technical Term Explainer — Simplify technical content with our Equation & Technical Term Explainer.


Provide:

Provide the full text of the paper (e.g., “Attention is All You Need”). Include section titles and boundaries. Specify the target audience (expert or lay). The system will return:

Paper Summary
Section-by-Section Summary Table
Expert Summary
Lay Summary
Mini-Glossary
Checks & Warnings
