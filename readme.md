# Dynamic Documents with R and knitr

In the very beginning, I planned to write this book with Markdown, but later
I changed my mind and wrote it in LyX instead. For those who are still
interested in the Markdown source, please see the [markdown](markdown)
directory.

Now this book has been published by [Chapman &
Hall](https://www.crcpress.com/Dynamic-Documents-with-R-and-knitr-Second-Edition/Xie/9781498716963). You can also find
it on [Amazon](https://www.amazon.com/dp/1498716962/). There is a
[book review](http://www.jstatsoft.org/v56/b02/) published in the Journal of
Statistical Software, which may give you a better idea of this book than my
own introduction.

## The book source

Besides the old Markdown source which is really only an empty sketch, this
repository also provides the real source files for the first three chapters
of the book, so that you can learn how the book was written and quickly get
started with writing books using the LaTeX style by Chapman & Hall.

The main file is `DDR-Yihui-Xie-Chap1-3.lyx`; the Rnw file
`DDR-Yihui-Xie-Chap1-3.Rnw` was exported from LyX; `krantz.cls` is the LaTeX
class provided by Chapman & Hall, and I wrote a simple LyX layout file
`krantz.layout`; `DDR-Yihui-Xie.bib` contains some bibliography entries, and
`DDR-packages.bib` is dynamically generated from **knitr** (see the last
chunk in the LyX or Rnw file).

The PDF of the first three chapters can be downloaded
[here :arrow_down:](https://github.com/yihui/knitr/releases/download/doc/DDR-Yihui-Xie-Chap1-3.pdf).

For Linux users, the minimal version of LyX for this book is 2.0.3 (as you can
get from Debian). For Windows/Mac OS X users, just download the latest binaries
from the [LyX website](http://lyx.org). If you do not use LyX, you can simply
open the Rnw file and start from there.

Be sure to read the session info in the preface because your R packages may
not be up-to-date to reproduce the PDF. Normally I use development versions
of my packages, because I often find little problems that I need to solve
for the book, and these changes will end up in the development versions.

## Contact

GitHub issues (<https://github.com/yihui/knitr-book/issues>) is the
preferred way for feedbacks. You can also reach me by email if you really
want:

```bash
echo oybuwycxy.trpb | tr bopcrbtucwxyc+ exmiaen@iyuih
```
