[this has been copied from the Etherpad doc and is being formatted for Markdown]


# Workshop *Open data and reproducibility v2.1*
## An introduction to R Markdown, dashboards and Binder
### :round_pushpin: [CarpentryCon@Home 2020](https://2020.carpentrycon.org/schedule/)

### Pablo Bernabeu and [Florencia D'Andrea](https://github.com/flor14)
p.bernabeu@lancaster.ac.uk  &nbsp; | &nbsp;  florencia.dandrea@gmail.com 

<br>

### Prior information 

Real data and code of varying complexity will be used. Basic and advanced R users are welcome.
Please sign up to RStudio Cloud (https://rstudio.cloud/), which may become useful if you encounter any issues in your local R. 

 Also suggested: 
 installing or updating R (https://www.r-project.org/) and RStudio  (https://rstudio.com/products/rstudio/download/); 
 perusing the links here; 
 having some of your own data and R code ready, preferably in a Github repository. 


 Content 
 For definitive information, please check this programme right before the workshop. 

 Introduction  |  5 min 

This workshop provides a stepping stone into a suite of interrelated tools—R Markdown, data dashboards and Binder environments—, which are all underlain by reproducible workflows and open-source software. 

 The resources in the programme and a video recording of the workshop will remain available afterwards. 
 
 We have two RStudio Cloud projects, one corresponding up to the Flexdashboard section (including), and one for the Shiny section: 
 
 - R Markdown and Flexdashboard: https://rstudio.cloud/project/1520963  
 - Shiny: https://rstudio.cloud/project/1514617 


 1.  R Markdown  |  20 min 

 RStudio Cloud project (not required if local RStudio fine): https://rstudio.cloud/project/1520963  

 Keep your input and output in check using R Markdown (https://rmarkdown.rstudio.com/). 
 
 Examples: https://bookdown.org/yihui/rmarkdown/journals.html,  http://rpubs.com/  

- Markdown  5 min 
- background: https://rmarkdown.rstudio.com/authoring_pandoc_markdown.html 
- examples: https://rmarkdown.rstudio.com/gallery.html 
- code demo: https://hackmd.io/@pablobernabeu/S1rnZkseP 

- HTML, CSS  3 min 
- background: https://html.com/ 
- example and code demo: https://github.com/pablobernabeu/UKCLC2020-workshop-Open-data-and-reproducibility/tree/master/R%20Markdown 

- Running code and cross-referencing  12 min 
- background: https://rmarkdown.rstudio.com/lesson-4.html, https://rmarkdown.rstudio.com/lesson-3.html 
https://bookdown.org/yihui/rmarkdown-cookbook/cross-ref.html
- examples: https://bookdown.org/yihui/rmarkdown/journals.html,  http://rpubs.com/ 
- code demo: https://rpubs.com/pcbernabeu/R-Markdown-Madison-parks 


 2.  Data dashboards / web applications  |  15 min 

 RStudio Cloud project (same as above): https://rstudio.cloud/project/1520963  

On a further step in reproducible, open data, we will learn how to publish dashboards online presenting data in the form of plots and tables. These all-reproducible dashboards are displayed as websites; thus, they can include hyperlinks and downloadable files. Some of the R packages used are rmarkdown, knitr, ggplot, plotly, flexdashboard, and shiny. The aim is to practise with different forms of dashboards (Flexdashboard, Shiny, Flexdashboard-Shiny) and the suitable hosting platforms (personal website, RPubs, Binder, Shinyapps, and custom servers).

- Flexdashboard  10 min 
- background: https://rmarkdown.rstudio.com/flexdashboard/ 
- examples: https://rmarkdown.rstudio.com/flexdashboard/examples.html 
- code demo: https://rpubs.com/pcbernabeu/Butterfly-species-richness-in-LA 

- Flexdashboard + Shiny  5 min 
- background: https://rmarkdown.rstudio.com/flexdashboard/shiny.html 
- examples: https://rmarkdown.rstudio.com/flexdashboard/shiny.html 
- code demo: https://pablo-bernabeu.shinyapps.io/experimental-data-simulation 

--- Tasks  🔨   25 min --- 
RStudio Cloud project (same as above): https://rstudio.cloud/project/1520963  
 Materials 

 1.  R Markdown doc: https://rpubs.com/pcbernabeu/R-Markdown-Madison-parks 
 Code: https://github.com/pablobernabeu/Data-is-present/blob/master/examples-documents-dashboards/R%20Markdown/R-Markdown-amidst-Madison-parks.Rmd

 2.  Flexdashboard: https://rpubs.com/pcbernabeu/Butterfly-species-richness-in-LA 
 Code: https://github.com/pablobernabeu/Data-is-present/blob/master/examples-documents-dashboards/Dashboards/Flexdashboard/Butterfly-species-richness-in-LA.Rmd 

 3.  Your own data, or any other data, if you like. 

 N.B. Flexdashboard is actually a type of R Markdown document, even if we're referring to them separately here. 
 Options (several possibilities, subject to preference and experience) 

 Tasks are ordered from easier to more difficult below. Please choose freely (or even create your own task, if you prefer). Feel free to ask the presenter any questions. 
 
 In any of the code chunks, set the chunk options `warning` and `message` both to TRUE. What's the result? 
 
Change the labels of the code chunks (e.g., largest-parks) as well as the calls to them in the cross-references (e.g., /@ref(tab:largest-parks)). You can replace the labels with any other word or words you like. 

In the R Markdown document, please look at the cross-reference in the last code chunk. Modify the options of that chunk in these ways: 
 1. Change the cross-reference (\@...) to that of the figure ('park-types'), instead of the table as it is now. 
 2. Change the options to display the plot but not the code. 

What changes in the R Markdown doc if you delete the argument shown below this line from the plot code? Hint: notice that the plot is an interactive plotly plot. 

 , tooltip = 'text' 

Insert an image into an R Markdown of Flexdashboard document, using either Markdown (https://guides.github.com/features/mastering-markdown/) or HTML (https://www.w3schools.com/tags/tag_img.asp) code. 

In the code for the table, remove the `%>% head(20)` bit to display the entire data. Then use the DT package to present the table nicely, and to allow the download of the data (https://rstudio.github.io/DT/). 

Create an R Markdown template or a Flexdashboard template, and apply some of the options we've viewed. For this purpose, you may use some of the classic built-in data in R (http://www.sthda.com/english/wiki/r-built-in-data-sets). 

Create an R Markdown or Flexdashboard document presenting some of your own data. 

Transform the R Markdown document into a Flexdashboard; then, vice versa, transform the Flexdashboard into an R Markdown document. For this purpose, please draw on the background links, and of course, the two documents themselves which serve as templates. This exercise is largely a matter of transposing code across templates. 

 [Homework]  Add Shiny user inputs to a Flexdashboard  (https://rmarkdown.rstudio.com/flexdashboard/shiny.html). Find out about Shiny and user inputs in the following section! 


 Last 5 minutes devoted to outstanding questions and other input (impressions, resources) from participants. 


--- Optional break  |  5 min ---   (Presenter available) 

Shiny ✨
Links
Books: 
- https://mastering-shiny.org
- https://engineering-shiny.org/
Examples of Shiny apps 
- https://shiny.rstudio.com/gallery 
- https://pablobernabeu.shinyapps.io/ERP-waveform-visualization_CMS-experiment/
- https://mybinder.org/v2/gh/flor14/shinyssd/binder?urlpath=shiny/shinyssd/inst/shiny/ (https://github.com/flor14/shinyssd ) 
 Demo  |  25 min 
Tasks 🔨  10 min 

RStudio Cloud (different from the one above): https://rstudio.cloud/project/1514617

I have prepared different kind of exercises. Are you new to shiny? This is a good exercise to start:
Allow the user the option of changing the y axis too, adding a new set of radiobuttons. Let the user to select among the options petal length and sepal length. 
      Hint: Remember to check how the variable names in the iris dataset are written.

RStudio cloud -> iris folder

If you have some experience or you finish quickly the first task:
I have 3 examples of this same app that are not working. Could you fix the apps? 
The apps are in the folders called 

RStudio cloud ->
shiny_ex1
shiny_ex2
shiny_ex3

 3.  Binder 🗂  10 min 

Did you know that you can enable public access to your data and analysis code in RStudio, on a simple internet browser? There are various options for this, and one of the most accessible ones is Binder (https://mybinder.org). We’ll look at Binder’s requirements and possibilities. 

RStudio environment example: http://mybinder.org/v2/gh/binder-examples/r/master?urlpath=rstudio
Dashboard environment example: https://mybinder.org/v2/gh/pablobernabeu/Modality-switch-effects-emerge-early-and-increase-throughout-conceptual-processing/eab65b392a8817454824f11c4efacea2e8a927f3?urlpath=shiny/Shiny-app/ 

Links

Git: https://happygitwithr.com/
Binder:
- https://the-turing-way.netlify.app/welcome
- https://github.com/binder-examples/r

Example of shiny app in GitHub repo
https://github.com/flor14/shiny_carpentrycon.git

Binder URLs
Shiny
https://mybinder.org/v2/gh/<user>/<repo>/<branch>?urlpath=shiny/<folder>/
RStudio IDE
https://mybinder.org/v2/gh/<user>/<repo>/<branch>?urlpath=rstudio

Binder URLs for the example 
Shiny
https://mybinder.org/v2/gh/flor14/shiny_carpentrycon/master?urlpath=shiny/iris/
RStudio IDE
https://mybinder.org/v2/gh/flor14/shiny_carpentrycon/master?urlpath=rstudio


 Conclusion  |  5 min 

 - Recap of the content. 
 - Please feel free to reach out with any outstanding questions. 
