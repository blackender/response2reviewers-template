# neoresponse.sty

The neoresponse LaTeX class provides environments and macros to format a point by point response to a journal article review. A section can be defined for each reviewer and the reviewer's points are automatically numbered. Labels can be added to the reviewers' comments so that they can be cross referenced from responses.

The class can be used to format the response serially, i.e. reviewer's point followed by authors' response and corresponding recompose, or as two columns so that the authors' response appears alongside the reviewer's comment.

## Usage
The file neoresponse.sty from this package can either be placed in the directory in which the rebuttal document is being edited, or in one of the conventional places for storing local TeX and LaTeX files on your system. Then add one of the following lines to the preamble of your LaTeX document.

`\usepackage{neoresponse}`

`\usepackage[table]{neoresponse}`

The package accepts two options 'plain' and 'table'; 'plain' is the default option and can be omitted.

The package provides a pair of environments for the reviewer's `comment`, a authors' `response` and a corresponding `recompose`. A `reviewersection` macro is used to begin each reviewer's comments, e.g.:

```
\reviewersection

\begin{point}
  ...
\end{point}
\begin{response}
  ...
\end{response}
\begin{recompose}
  ...
\end{recompose}

```

See the example files included in this package for illustrations of how each option might be used (both source and PDF versions are provided). The default, plain option is the easiest to use. The table option has some formatting issues, can be brittle when used, and requires further refinement.

## Licence
The LaTeX package and examples are licensed under the terms of the Creative Commons CC-BY-SA v3.0.

* The LaTeX package and the example files are the work of Nathan Wu.
