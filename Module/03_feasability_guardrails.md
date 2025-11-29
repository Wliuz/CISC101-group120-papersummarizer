Change Log: Added warning message will output if (section has less than 20 words/section has no words or missing). Added evidence mode, summary must include claims/equations and results from the paper.

Purpose: Apply logical checks for realism and readability. Steps:

evidence_mode = "strict"

summary must include claims/equations/and results from the paper

If/Else Logic:

If section < 20 words → exclude. (output warning message "section # was skipped due to lack of words")

If section contains expert terms → translate into layperson language.

If section has no words → ignore. (output warning message "section # is missing")

If section has important information → add citation marker (e.g., “(see Section 2)”).

If section doesn't have enough information --> State there is not enough detail

If total summary > 300 words → shorten or simplify (remove redundancy, compress sentences).

Final Output:

Concise, plain-language summary with citations, capped at 300 words.
