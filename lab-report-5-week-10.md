---
title: Lab Report 5, Week 10
---

# Report 5

## Lab 9: Markdown Parse with Multiple Files
![Image](/labpics5/vimdiff.png)

* After saving results to each of the markdown-parsers, the action `vimdiff` for a side-by-side of the two results. With this action, the differences in the two documents will be highlighted for the user.

## [Test File 1](https://katrinado.github.io/cse15l-lab-reports/test-files/12.html):
![Image](/labpics5/testfile1.png)

Actual for markdown-parser: `--------------`

Actual for cse15lsp22-markdown-parser: `[]`

Expected: `[]`

* By looking at the outputs of both markdown parsers, the cse15lsp22-markdown-parser has the correct implentation of the markdown parser. My markdown parser did not print an empty list meaning that there was an error when trying to use my code for that test-file. The correct output, an empty list, was given by the cse15lsp22-markdown-parser.
* The missing output is due to the incorrect implementation that elicited an error.

## [Test File 2](https://katrinado.github.io/cse15l-lab-reports/test-files/170.html):
![Image](/labpics5/testfile2.png)

Actual for markdown-parser: `["demo"]`

Actual for cse15lsp22-markdown-parser: `[]`

Expected: `[]`

* By looking at the outputs of both markdown parsers, the cse15lsp22-markdown-parser has the correct implentation of the markdown parser. My markdown parser printed "demo" because it was between parentheses. The correct output, an empty list, was given by the cse15lsp22-markdown-parser.
* The incorrect output that printed is due to the code printing the text between the parentheses meaning that more conditions need to be implemented to prevent text that aren't links from being printed.