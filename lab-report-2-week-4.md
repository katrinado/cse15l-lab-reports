# Lab Report 2, Week 4

## Code Change 1
![Image](/labpics2/change1.png)

File containing *failure-inducing input*: [test-file.md](https://github.com/katrinado/markdown-parser/blob/main/test-file.md)

![Image](/labpics2/fail1.png)

The bug that correlates to this edit in the code was an infinite loop. The *failure-inducing input* was the new line character at the end of the file. The original code was unable to find where the markdown file ended so it would endlessly continue until eventually resulting with an out of memory error for its output. In order to fix this, the code was changed to locate where the final closed bracket in the markdown file.

---

## Code Change 2
![Image](/labpics2/change2.png)

File containing *failure-inducing input*: [new-test-file.md](https://github.com/katrinado/markdown-parser/blob/main/new-test-file.md)

![Image](/labpics2/fail2.png)

An error that occurs from this file is another out of memory error. This resulted from the the new-test-file having many parentheses following the link rather than a new line similar to the previous code error. In order to fix this closeParen was edited so that the code wouls successfully print something and not display an error message.


---

## Code Change 3
![Image](/labpics2/change3.png)

File containing *failure-inducing input*: [new-test-file.md](https://github.com/katrinado/markdown-parser/blob/main/new-test-file.md)

![Image](/labpics2/fail3.png)

The new issue I was presented with was that the code would print the link as many times as there were closed parentheses following. The code is using the initial open parentheses and pairing it with each following closed parentheses which results in the multiple prints of the same link. The code was changed so that the loop would stop if the closing parentheses is repeated.