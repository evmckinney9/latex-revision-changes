# Reviewer Comments LaTeX Package

## Description

The Reviewer Comments LaTeX Package enhances the manuscript revision process by allowing authors to easily highlight and annotate text changes in response to reviewer feedback. It supports color-coding for different reviewers and integrates marginal notes for quick reference, streamlining the revision workflow in LaTeX documents.

![image](https://github.com/evmckinney9/latex-revision-changes/assets/47376937/1e72c5f8-4d40-4e11-b10d-433a15fc93bb)

## Installation

1. Download `reviewercomments.sty` from the repository.
2. Place it in your LaTeX document's directory or in your LaTeX distribution's package directory.
3. Add `\usepackage{reviewercomments}` to your document's preamble.

## Usage

**Highlight Text and Add Marginal Notes:**

```latex
\reviewer{ReviewerID}{CommentNumber}{Text changed in response to comment.}
```

- `ReviewerID`: Identifier for the reviewer.
- `CommentNumber`: Comment number or identifier.
- `Text changed in response to comment.`: The modified text.

**Suppress Additional Marginal Notes:**

To avoid clutter, suppress extra marginal notes for subsequent changes related to the same comment:

```latex
\reviewer[false]{ReviewerID}{CommentNumber}{Further text changes.}
```

## Example

For a full example, see `example.tex` in this repository.
