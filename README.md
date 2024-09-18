
# Chicken LMD compilation for method development

Analyses of all the metagenomic microsamples from chicken

## Bioinformatic procedures

Data processing to generate the count data was conducted using the following Snakemake pipeline: [mg_quant](https://github.com/3d-omics/mg_quant). Data analysis procedures source from the outputs of this pipeline.

## Analysis procedures

The raw code used for data analysis is in the **Rmd** files stored in the root directory of this repository, while the bookdown-rendered webbook is available at:
[3d-omics.github.io/ANMI014_chicken_LMD_methods](https://3d-omics.github.io/ANMI014_chicken_LMD_methods)

While the webbook provides a user-friendly overview of the procedures, analyses can be directly reproduced using the Rmd documents. Note that the code chunks that require heavy computation have been tuned off using 'eval=FALSE'. To re-render the webbook, you can use the following code:

```r
library(bookdown)
library(htmlwidgets)
library(webshot)

render_book(input = ".", output_format = "bookdown::gitbook", output_dir = "docs")
```
>>>>>>> ace4cec (Initial commit)
