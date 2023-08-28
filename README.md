# Reviewer Comments LaTeX Package

## Description

This LaTeX package provides an easy and consistent way to highlight text changes in response to reviewer comments during the paper revision process. The package allows you to color-code changes according to the reviewer and link the changes to a marginal note. It supports multiple reviewers and can suppress additional marginal notes while coloring disjoint text within the same paragraph.

![image](https://github.com/evmckinney9/latex-revision-changes/assets/47376937/1e72c5f8-4d40-4e11-b10d-433a15fc93bb)

## Installation

1. Download the `reviewercomments.sty` file from this repository.
2. Place it in the same directory as your main LaTeX document or in your LaTeX distribution's package directory.
3. In your LaTeX document, add `\usepackage{reviewercomments}` in the preamble to include the package.

## Usage

### Basic Usage

In your LaTeX document, use the `\reviewer` command to highlight text and add a marginal note:

```latex
\reviewer{A}{1}{This is some changed text.}
```

- `A` is the reviewer identifier.
- `1` is the comment number from that reviewer.
- `This is some changed text.` is the text that has been changed.

### Suppressing Marginal Notes

If you have multiple changes within the same paragraph that address the same reviewer comment, you can suppress additional marginal notes like this:

```latex
\reviewer[false]{A}{1}{Additional changed text in the same paragraph.}
```

## Example

See the `example.tex` file in this repository for a full example.
