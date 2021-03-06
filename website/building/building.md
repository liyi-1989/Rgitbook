
# Building Gitbooks

Now that your Gitbook project is setup, you can edit the `.Rmd` files with your content. The `Rgitbook` package adds two important features: The ability to include R code directly in your documents and support for [MathJax](http://www.mathjax.org/). RStudio has an excellent tutorial on using R Markdown on their website at [http://www.rstudio.com/ide/docs/authoring/using_markdown](http://www.rstudio.com/ide/docs/authoring/using_markdown). However, the basic format is:

	```{r label, options}
	# R code
	```

The full list of options that alter how the R markdown chunck is processed and displayed is avaiable here: [http://yihui.name/knitr/options](http://yihui.name/knitr/options).

[MathJax](http://www.mathjax.org/) is a JavaScript library that allows for embedding LaTeX style formulas in HTML, for example \\( a^2 + b^2 = c^2 \\).

$${ e }^{ i\pi  }+1=0$$

For inline equations, use surround the equation with `\\(` and `\\)`. For equations on their own line, the typical LaTeX formatting applies by surround the equation between `$$`. If you are new to LaTeX equations, the Daum Equation Editor for [Google Chrome](https://chrome.google.com/webstore/detail/daum-equation-editor/dinfmiceliiomokeofbocegmacmagjhe?hl=en) or [Mac OS X](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CDUQFjAB&url=https%3A%2F%2Fitunes.apple.com%2Fus%2Fapp%2Fdaum-equation-editor%2Fid540665783%3Fmt%3D12&ei=fHJWU4nLKeHIsATbs4HgBQ&usg=AFQjCNH69beGYAfr5ojnPILLNOG-goN9sw&sig2=T_SN94407Vof0hIAmKRtAA&bvm=bv.65177938,d.cWc) provides a nice user interface for designing equations.

Building Gitbooks is a two step processes. First, R Markdown files must be converted to plain Markdown files and second, the Markdown files be converted to a Gitbook (either HTML, PDF, or eBook). The next two sections outline the functions and options for building.
