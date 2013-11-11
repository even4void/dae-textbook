This is the main repository for the R Companion to Montgomery's *Design and
Analysis of Experiments* (2005). 

This project was started several years ago. Although it grew smoothly during
the first two years or so, it hasn't evolved much since then. I released
minor updates from time to time. Last update is 2012-12-02.

Problem is that TeX code is clearly outdated now, and it relies on a `tex ->
ps -> pdf` toolchain, with Python code to tangle R code and create a
pictures gallery. There are better options with `XeLaTeX` (which I tried
last year on this document) or `lualatex` (released with
[TeX Live](http://www.tug.org/texlive/) 2013). I should fix this at some
point. There are more serious issues though: Now, CRAN features many R
packages for
[DoE](http://cran.r-project.org/web/views/ExperimentalDesign.html), and I'm
afraid many code chunks should be updated to better reflect state of the
art. Lastly, I didn't use Sweave--and I can't remember why--,which makes
updating the whole document really painful at times.

So, here are the new development process, after I pushed everything on
GitHub:

- I will keep the old document for historical reason. It can be found in the
  `archive.tar.gz` tarball, without intermediate compilation files.
- The new version will be based on [knitr](http://yihui.name/knitr/) and
  XeLateX.
- I will try to update old code using available R packages inasmuch as
  possible.
- Newer editions of Montgomery's DAE have been published, but I will stay at
  Edition 5.
