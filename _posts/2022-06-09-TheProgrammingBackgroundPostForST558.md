Programming Background
================
Chengxi Zou
2022-06-09

## My thoughts on R

1.  R vs SAS

I’ve taken ST555 3 times which is about SAS programming, it was a hard
course and I was struggling with it. One big difference between R and
SAS is that in R we could download many useful packages while SAS seems
to be already totally constructed so you couldn’t do more things on its
functionalities, you just use it.

2.  What functionality do you like about R? What parts do you miss about
    your other language? Do you consider R a difficult language to
    learn?

It’s just a few weeks that I’ve been learning R, I haven’t seen much
difference between R and SAS in their functionality so far, the logics
and the syntax are similar, so I would jsut say I like the function
*install.packages* in R and I will keep digging into it.

## example R Markdown output.

create an R code chunk that outputs a plot.

``` r
plot(iris)
```

![](../images/plotexample-1.png)<!-- -->

render(“\_Rmd/2022-06-09-TheProgrammingBackgroundPostForST558.rmd”,output_format
= “github_document”, output_dir = “/posts/”,output_options =
list(html_preview = FALSE))