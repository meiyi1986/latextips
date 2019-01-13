# Tips for LaTeX Writing

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
