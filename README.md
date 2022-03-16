# Template

The original [template](https://github.com/rstudio/bookdown-demo) was from RStudio but required some changes to make it work as html and be published through GitHub. I made this work for a repository about [Professional Registration](https://github.com/Lextuga007/professional-registration) and although I attempted to replicate the changes I made there, I got muddled so starting again I have just taken all the files from my repository to make this template. 

# Render the book

```r
bookdown::render_book('index.Rmd', 'bookdown::html_book')
```