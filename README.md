This is my 3rd Blog!
================
Chengxi Zou
2022-06-09

## My thoughts on R

**Write a post about what you consider the coolest thing you’ve learned
about programming in R. Include an example of it (or at least the code
to do it) in your post (for instance, if it was ggplot you could read in
a data set and create a cool plot).**

I really like ggplot2 package. The base packages in R produces some
graphs that are’t very fancy, but using the ggplot2 package we can
generate some beautiful graphs and it’s easy to understand its syntax of
“layers”.

``` r
library(rmarkdown)
library(ggplot2)

ggplot(iris, aes(x = Sepal.Length, Petal.Length)) +
geom_boxplot(aes(color = Species)) +
ggtitle("Box Plot Example")
```

![](D:\5th%20semester\ST558\Rrepo\ChengxiZou.github.io\README_files/figure-gfm/p1-1.png)<!-- -->

``` r
ggplot(iris, aes(x = Sepal.Length)) +
geom_histogram(aes(fill = Species), position = "dodge") +
ggtitle("Histogram Example")
```

![](D:\5th%20semester\ST558\Rrepo\ChengxiZou.github.io\README_files/figure-gfm/p2-1.png)<!-- -->

``` r
ggplot(iris, aes(x = Sepal.Length, Petal.Length)) +
geom_point(aes(color = Species)) +
ggtitle("Scatter Plot Example")
```

![](D:\5th%20semester\ST558\Rrepo\ChengxiZou.github.io\README_files/figure-gfm/p3-1.png)<!-- -->

run render function in the console:

render(“\_Rmd/2022-06-29-Third Blog Post.rmd”,output_format =
“github_document”, output_dir = “\_posts/“,output_options =
list(html_preview = FALSE))
