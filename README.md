# Tips for LaTeX Academic Writing

## General
* Always leave a whitespace after a punctuation, and between a letter and a bracket, e.g. "word` `(a)" and "reference` `[1]". *NO* whitespace before a punctuation.
* When referring to a section, table, figure, equation, or algorithm, the first letter should be capitalised. For example, "Section I, Table II, Figure 4, Eq. (3)".

## Mathematical Notations/Equations
* Always put mathematical symbols and equations into math environment.
* Examples of **in-line** math environment include `$a$`, `$b+1$`, and `$y = 2x+3$`.
* Examples of **standalone** math environment include `\begin{equation} y = x + z \end{equation}`.
* When using words in notations, better to use `\textit{text}` rather than `$text$`. This will give you smaller separation between letters in the word.
* When using multiple letters in superscript or subscript, remember to use `{}`, e.g. `$x_{rt}$`.
* Keep the style consistant for different types of notations. For example, use **lowercase letters (e.g. `x`, `a`) as scalars**, **boldface lowercase symbols (e.g. `\boldsymbol{x}`) as vectors**, and **uppercase letters (e.g. `A`, `X`) as matrices**. 

## `\label` and `\ref`
Whenever there is a need for reference, such as referring to a **Section**, a **Table**, a **Figure**, and an **Algorithm**, always use `\label` and `\ref`.

Example:

\section{Referred Section} \label{referredsection}

This is somewhere else where you want to refer to the referred section by `Section \ref{referredsection}`.

## Tables
* Use \begin{table}[!ht] for the best layout.
* For printing a wide table in a double-column template, use \begin{table*}[!ht]. 
* Use \footnotesize can reduce the font size in the table a bit, but still clear to see.
* A good guide to make nice tables: "https://www.inf.ethz.ch/personal/markusp/teaching/guides/guide-tables.pdf".
* **For printing results, always try to create LaTeX tables automatically using script, rather than typing the results manually.** Scripting the tables can save time, and remove the potential typing error.
* If you write scripts to process your result data, you can **print the processed results in the format of LaTeX table**.
* If your processed data is an Excel spreadsheet, you can transform it into LaTeX table source code using this Excel add-on: https://github.com/krlmlr/Excel2LaTeX. Or Google "Excel to LaTeX".

## Figures
* Use \begin{figure}[!ht] for the best layout.
* For printing a wide figure in a double-column template, use \begin{figure*}[!ht].
