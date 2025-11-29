Purpose: Summarize each section iteratively. Steps:

Iterate through each section

For section n:

If word count < 20 → skip.

Else → generate summary.

Simplify uncommon terms

Replace jargon with plain language (e.g., “polymerase chain reaction” → “a method to copy DNA”).

Attach section number

summary_level = "short" (1–2 sentence summary per section)
  
summary_level = "detailed" (A short paragraph **plus** a bullet list of 3–5 key points for each section)

if summary_level = "short" --> generate only a compact summary

If summary_level = "detailed" → generate summary + bullet list.

Make sure the instructions are clearly written in `02_section_loop.md` in the same style as the existing loop logic.

Output format: [Section #] Summary text.

