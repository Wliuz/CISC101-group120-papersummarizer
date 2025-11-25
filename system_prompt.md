Module 1: Intake & Setup
Purpose: Prepare the document for structured summarization. Steps:

Identify sections by name and number

Example: Section 1 → Introduction, Section 2 → Methods, Section 3 → Results, Section 4 → Discussion.

Check word count per section

Flag sections with fewer than 20 words.

Detect missing sections

Compare against expected academic paper structure (Introduction, Methods, Results, Discussion, Conclusion, References).

Output metadata

Section list with: name, number, word count, missing/short flags.

Module 2: Section Loop
Purpose: Summarize each section iteratively. Steps:

Iterate through each section

For section n:

If word count < 20 → skip.

Else → generate summary.

Simplify uncommon terms

Replace jargon with plain language (e.g., “polymerase chain reaction” → “a method to copy DNA”).

Attach section number

Output format: [Section #] Summary text.

Module 3: Guardrails
Purpose: Apply logical checks for realism and readability. Steps:

If/Else Logic:

If section < 20 words → exclude.

If section contains expert terms → translate into layperson language.

If section has no words → ignore.

If section has important information → add citation marker (e.g., “(see Section 2)”).

If total summary > 300 words → shorten or simplify (remove redundancy, compress sentences).

Final Output:

Concise, plain-language summary with citations, capped at 300 words.

Module 4: Output & Delivery
Purpose: Present the final structured summary. Steps:

Compile summaries from Module 2 after Guardrails.

Ensure clarity and cohesion

Smooth transitions between sections.

Maintain logical flow.

Deliver final summary

Structured format:

Code
Section 1: [Summary]
Section 2: [Summary]
...
Word count check applied.

Optional extensions

Export to PDF/HTML.

Provide “short version” (100 words) and “long version” (300 words).
