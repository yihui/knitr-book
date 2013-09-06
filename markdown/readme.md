# Dynamic Report Generation with R

This book is mainly about the R package **knitr**, which is on CRAN (<http://cran.r-project.org/package=knitr>) and has detailed documentation and examples (<http://yihui.name/knitr/>). I think it may be a good idea to organize these materials in a better form, and explain more details about **knitr** which are not covered in the online documentation. It is also a good opportunity to [eat my own dog food](http://en.wikipedia.org/wiki/Eating_your_own_dog_food) and see how **knitr** performs in the real world.

## License

All the content in this repository is licensed under [CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/), and you are always welcome to participate the writing by [forking](https://github.com/yihui/knitr-book/fork_select) this repository.

## Ebook

I do not know if this repository can grow into a real book in the end. At the moment, it can be easily turned into an ebook with [pandoc](http://johnmacfarlane.net/pandoc/), which you can read on iPad or Kindle or other electronic book readers. There are also other formats that you can use, such as HTML or GitHub markdown. The conversion is simple if you have installed `pandoc`:

```bash
./knit epub    # EPub ebook
./knit html    # a single html page
./knit pdf     # PDF through XeLaTeX
./knit github  # markdown for github
````

I use the above commands to knit my source documents and convert them into different formats. I work under Ubuntu, and the bash script `./knit` may not work for your OS (it is essentially an R script), but you are encouraged to read its source code to know what is happening behind the scene.

All source files are under the [`source`](https://github.com/yihui/knitr-book/source/) directory, and all the rest of markdown files are the output from **knitr**. If you want to modify anything in this repository, please always go to the source directory. In other words, only manage the source, and forget about the output.

## Help me

Currently I need help on designing the CSS styles for the HTML and EPub output; I do not have much time for that. The default style is not optimal for reading. You are welcome to contribute if you know `pandoc` and CSS, and you can probably look at [bootstrap](http://twitter.github.com/bootstrap/) for an appealing design.

If you have more time to kill, I also need help on the TeX style so that the PDF output looks better. I just picked up three free fonts in my library and throwed them to XeLaTeX.
