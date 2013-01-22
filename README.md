# D Template Tutorial


## What's it's about

This project is about a wonderful part of the [D programming language](www.dlang.org "D Website"): templates.
It contains a markdown document on templates aiming to be a kind of tutorial.

It's divided in 6 chapters:

* `Introduction` is just, well, the introduction text, explaining the goal of this document and the formatting conventions used.
* `Basics` is about templates syntax, basic building blocks (`static if`, eponymous trick) and function, struct and class templates.
* `Some More Advanced Considerations` is about more advanced ideas, like constraints, tuples or operator overloading.
* `Around Templates` deals with other metaprogramming constructs interacting with templates: traits, compile-time function evaluation (CTFE) and string mixins.
* `Examples` presents some more detailed examples of what can be done with D templates.
* The `Appendix` gives some explanation on the `is` expression and links on other templates resources.


If you find any inexactitude, plain error or missing subject, don't hesitate to open an issue on github!


## Other formats

The markdown syntax used for the doc is the extended version used by Pandoc (mainly for tables or code sections).
Using markdown files and [Pandoc](http://johnmacfarlane.net/pandoc/), I generate the HTML, pdf and epub versions. Feel free to comment on them also.


## LaTeX notes

This tutorial doc used to be made of LaTeX files. You can still find them in the `latex` folder, but I'll phase them out (I just keep

The master document is `dtemplates.tex` and calls the other subfiles:

* `dtemplates_intro.tex`
* `dtemplates_basics.tex`
* `dtemplates_advanced.tex`
* `dtemplates_around.tex`
* `dtemplates_examples.tex`
* `dtemplates_appendix.tex`


The LaTeX files use the [minted](http://code.google.com/p/minted/) package. `minted` uses Python's [Pygment](pygments.org) highlighter.
D code blocks are between `\begin{dcode}` and `\end{dcode}` commands. Transform them into `verbatim` commands if you do not want to use `minted`.
