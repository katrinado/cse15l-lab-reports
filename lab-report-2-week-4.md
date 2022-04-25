# Lab Report 2, Week 4

## Code Change 1
![Image](/labpics2/change1.png)

[test-file.md](https://github.com/katrinado/markdown-parser/blob/main/test-file.md)

![Image](/labpics2/fail1.png)

The bug that correlates to this edit in the code was an infinite loop. The *failure-inducing input* was the new line character at the end of the file. The original code was unable to find where the markdown file ended so it would endlessly continue until eventually resulting with an error for its output. In order to fix this, the code was changed to locate where the final closed bracket in the markdown file.

---

## Code Change 2
![Image]()

---

## Code Change 3
![Image]()

