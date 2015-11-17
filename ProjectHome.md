zhspacing fine-tunes several details in typesetting Chinese using XeTeX and XeLaTeX, such as automatic font switch between Chinese and Western characters, skip adjustment of fullwidth punctuations, punctuation prohibitions, automatic skip insertion between Chinese and Western characters or math formulas, etc.


---

**Notice** 08.4.5.

For your information, currently zhspacing is not the only package for Chinese typesetting under XeLaTeX, and it doesn't update often. Mr. Sun Wenchang's xeCJK is probably a better choice for most users.

---


The basic usage is like this:
```
\documentclass{article}
\usepackage{zhspacing}
\zhspacing
\begin{document}
中Eng文混排，“标点压缩”，间 距 调 整 ……
\end{document}
```

Typesetting Chinese document using XeLaTeX + zhspacing is much like using LaTeX + CJK + CJKpunct, except that you don't need to add the annoying ~ between Chinese and English for spacing adjustment, and opening punctuations (line-end prohibition) can occur at the beginning of the line, which is forbid in CJKpunct. The amount of adjusted space can be easily customized to your own taste.

A recent feature of zhspacing is that it supports typesetting Chinese in math formulas, using zhmath.sty. And using zhfont.sty can simplify font definition. Underdot is now supported using zhfont.