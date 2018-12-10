R Markdown
----------

R markdown has three components:
`to force the new line, I added 2 spaces at the end`  
1. metadata (between 2 `---` at top of document)  
2. text (of any kind, anywhere)  
3. and code, surrounded by 3 backticks for a code chunk, or a single
backtick for inline calculations (2x2=4).

### Metadata

`note the 3 hashes to make a subheading`

The YAML ("YAML ain't markup language") header is picky about
formatting, including indentation. Use examples or go to a reference to
solve more complicated problems. (see [bookdown.org](www.bookdown.org)
for lots of info)

### Text

Again, this is the stuff you are writing to either document your
analyses or discuss them (for example, in a paper).

### Code

Can be r, python, and many others an you can control whether the code
shows, the output shows, or both.

Compile
-------

Using the knit button or Ctrl-Shift-K.

This renders in a new R session ... a very important point because it
means that anything in the console from the previous session is now
gone. This is a good thing, related to why you shouldn't save your
.Rhistory as it can lead to issues with reproducibility.

You can also render via the command-line or a script, giving you the
ability to have automated report generation but you have to worry about
reproducibility in that case.

    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

Including Plots
---------------

You can also embed plots, for example:

![](learnRmd_files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
