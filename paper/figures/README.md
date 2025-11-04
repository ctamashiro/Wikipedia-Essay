# Figures Directory

This folder contains all figures used in the research paper **“Language Bias in Wikipedia.”**

## Purpose
Figures are included to visualize our findings on how Wikipedia articles differ across languages.  
They support the results and discussion sections by highlighting examples of variation in tone, emphasis, and content.

## Recommended Figure Types
- **Comparison Tables (PDF):** Visuals comparing English, Japanese, and Spanish Wikipedia summaries for the same topic.  
- **Word Frequency Charts (PDF or PNG):** Bar plots showing common keywords across languages.  
- **Language Distribution Diagram (PNG):** A simple flow diagram showing how summaries were retrieved and analyzed.  
- **Screenshot Samples (JPG):** Example snippets of actual API outputs or Wikipedia pages (used sparingly for illustration).  

## Naming Convention
Use clear and descriptive filenames (avoid `fig1.pdf`). Examples:
- `language-summary-comparison.pdf`
- `keyword-frequency-chart.png`
- `api-data-flow-diagram.pdf`

## How to Include Figures in LaTeX
Include figures in your `.tex` sections using the following syntax:

```latex
\begin{figure}[h]
  \centering
  \includegraphics[width=\linewidth]{figures/language-summary-comparison.pdf}
  \caption{Comparison of Wikipedia article summaries for the same topic across English, Japanese, and Spanish editions.}
  \label{fig:languagecomparison}
\end{figure}
