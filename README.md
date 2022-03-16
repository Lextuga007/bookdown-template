# Template

The original [template](https://github.com/rstudio/bookdown-demo) was from RStudio but required some changes to make it work as html and be published through GitHub. I made this work for a repository about [Professional Registration](https://github.com/Lextuga007/professional-registration) and although I attempted to replicate the changes I made there, I got muddled so starting again I have just taken all the files from my repository to make this template. 

## Packages required

```r
install.packages("bookdown")
#install.packages("remotes")
remotes::install_github("rstudio/bslib")

```

# Changes to make

In file `_output.yml` the following can be changed:

```yaml
      before: |
        <li><a href="./">Bookdown Template</a></li>
      after: |
        <li><a href="https://github.com/rstudio/bookdown" target="blank">Published with bookdown</a></li>
    edit: https://github.com/Lextuga007/bookdown-template%s
```

Note that the `%s` is always required in this url.  

# Render the book

```r
rmarkdown::render_site(encoding = 'UTF-8')

```
Or use the Build Book button that appears with the Build tab (where the tabs read Environment, History, Connections and maybe Git if that's connected.)

# GitHub pages

To publish through GitHub go to Settings/Pages and change Source to `main` and `/docs`. It will take a few minutes to load the pages.
