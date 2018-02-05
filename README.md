# travis-blogdown

[![Build Status](https://travis-ci.org/yihui/travis-blogdown.svg?branch=master)](https://travis-ci.org/yihui/travis-blogdown)

A minimal example of building and deploying a blogdown-based website via Travis CI. For more information, please see this section in the **blogdown** book: https://bookdown.org/yihui/blogdown/travis-github.html. (In short, I don't recommend you use this approach. Consider building your website locally, and [deploying through Netlify](https://bookdown.org/yihui/blogdown/netlify.html) instead.

David Selby has written a more detailed tutorial with screenshots that you may want to read, too: http://selbydavid.com/2017/06/22/blogdown-travis/.

## Example one
```{r linktable, echo=FALSE}
library(DT)
x<-iris[1:3,1:3] #create a small matrix from larger supplied one
link1<-"<a href='[go to Methods](#methods)"

link2<-"<a href='http://www.yahoo.com'>another link </a>"
link3<-"<a href='http://www.becu.com'>last link </a>"
#y<-c(link1,link2,link3)
x$links<-c(link1,link2,link3)
linktable<-datatable(x, escape = FALSE)
linktable
```
