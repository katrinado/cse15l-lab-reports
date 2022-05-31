---
title: Lab Report 4, Week 8
---

# Report 4

## 1. [Snippet 1](https://katrinado.github.io/cse15l-lab-reports/snippets/snippet1.html)
```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```
![Image](/labpics4/preview1.png)

**Expected Output:** `['google.com, google.com, ucsd.edu]`



## 2. [Snippet 2](https://katrinado.github.io/cse15l-lab-reports/snippets/snippet2.html)
```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```
![Image](/labpics4/preview2.png)

**Expected Output:** `[a.com, a.com(()), example.com]`




## 3. [Snippet 3](https://katrinado.github.io/cse15l-lab-reports/snippets/snippet3.html)
```
[this title text is really long and takes up more than
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```
![Image](/labpics4/preview3.png)

**Expected Output:** `[[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]]`

---

## [My MarkdownParse](https://github.com/katrinado/markdown-parser)

Results of Added Tests for my implementation:
![Image](/labpics4/mine.png)


## [Reviewed MarkdownParse](https://github.com/ezh247467/markdown-parser)

Added tests for their implementation:
![Image](/labpics4/reviewed.png)

## Answers:
1.
2.
3.


