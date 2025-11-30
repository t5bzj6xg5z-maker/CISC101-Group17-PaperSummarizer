# CISC101-Group17-PaperSummarizer

Group Members:
- Zakkary
- Emmett
- Nathan

## What this repo has
- `system_prompt.md` + `modules/` (01–06) — already structured.

## How to run
1) Open your LLM and set `system_prompt.md` as the system instruction.
2) Provide options:  
   - `summary_level`: `short` or `detailed`  
   - `evidence_mode`: `default` or `strict`  
   - `audience`: `expert` or `lay`
3) Expect outputs in this order: Paper Summary → Section Table → Expert/Lay Summaries → Mini-Glossary → Checks & Warnings.

## Test Scenarios
- **Short Section Warning:** If a method is less than 50 words, expect a message like “Section very short: summary may be incomplete.”
- **Missing Section Warning:** If discussion is intentionally omitted, expect a message indicating the section was skipped and no usable text was provided.
- **Strict Evidence Mode:** To verify the standard message appears even when details aren’t explicit, set `evidence_mode=strict`.
- **Equation + Citation:** Detect the presence of the equation `$y = Wx + b$` and the citation `(Vaswani et al., 2017)`.


The generated `system_prompt.md` and `/modules` meet the requirements of Set 1: PS2 specification, including explicitly quoted inputs, outputs, and constraints.  They also contain the necessary system-prompt components, such as a greeting, tone, input handling, boundary setting, and mandated output sections.  Furthermore, they include the four core modules, two student-created modules, a strict evidence guardrail with the exact standard message, standardized warnings for missing, empty, or under 50-word content, deterministic formatting, and a modular flow consistent with the described architecture.  Module 02 features a `summary_level` option with “short” and “detailed” (paragraphs plus 3–5 bullets).  Module 03 specifies `evidence_mode = “strict”` and the exact warning strings.
