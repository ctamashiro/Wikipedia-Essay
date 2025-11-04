Literature Review Agent Workflow (Web Source Version)
Overview

This is a prompt script (AI workflow definition or agent instruction file) that guides an AI agent to conduct a structured literature review of web-based sources related to bias in Wikipedia.
Instead of PDF research papers, the agent analyzes the textual content of web articles and outputs standardized summaries and citations.

Input

All web articles listed in the Sources section below:

Ideological bias on Wikipedia (Wikipedia)

Finding Hidden Biases in Wikipedia’s Multilingual Content (Johns Hopkins University)

Wikipedia Facts Depend on Which Language You Read Them In (New Scientist)

Output

Create or update:

literature/literature-review.md — structured summaries of each article

paper/references.bib — BibTeX-style references for all reviewed web sources

Instructions

For each article listed above:

Fetch and preprocess the text

Extract the visible article text (ignore ads, menus, comments, and unrelated metadata).

Save a plain-text version as literature/<shortname>.txt, where <shortname> reflects the article topic (e.g., ideological-bias.txt).

Add structured entry to literature-review.md

Use the format below for each article.

Write concise academic-style summaries in 2–3 sentences per section.

Include hyperlinks for source access and Google Scholar keyword searches if applicable.

Template:

## [Article Title] (Year)

**Authors/Publisher**: [Author(s) or Publisher Name]

**Original Source**: [Clickable link to original article]

**Google Scholar**: [Link to Google Scholar search with article title]

**Summary**: [2 sentences describing the main argument or findings]

**Methodology**: [2 sentences explaining how the article investigates or presents bias — e.g., comparative analysis, case study, linguistic or cultural review]

**Results**: [1 sentence summarizing main findings or implications]

**Evaluation**: [Rating 1–5]/5 — [1 sentence justification comparing credibility, clarity, and relevance to the research topic]

**Resources**:
- Dataset / Examples: [if mentioned]
- Code or Data Links: [if available]
- Related Studies: [if cross-referenced]

---


Create corresponding BibTeX-style entry

Append to paper/references.bib in alphabetical order.

Use @online type for web sources.

Example format:

@online{jhu2025wikipedia,
  author    = {Johns Hopkins University},
  title     = {\href{https://hub.jhu.edu/2025/01/09/finding-hidden-biases-in-wikipedias-multilingual-content/}{Finding Hidden Biases in Wikipedia’s Multilingual Content}},
  year      = {2025},
  publisher = {Johns Hopkins University Hub}
}

Constraints

Summaries must be exactly 2 sentences per section (except “Results” and “Evaluation” which are 1 sentence each).

Preserve existing markdown structure and alphabetical order.

Do not duplicate entries if already present.

Check links for validity.

Only process listed URLs.

Verification

After execution, confirm that:

Each article in the Sources list has:

A .txt file in the literature/ folder

A complete markdown entry in literature-review.md

A corresponding BibTeX entry in paper/references.bib

All titles are clickable links.

Formatting renders correctly in Markdown preview.

Learning Objectives

Students following this workflow will learn to:

Conduct literature reviews using structured AI-assisted templates

Summarize web sources concisely and consistently

Integrate non-academic sources into reproducible research workflows

Maintain transparent documentation and version control practices