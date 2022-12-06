Introduction to parallel processing, using R
==============================

*Contributors: Timothée Bacri<sup>†</sup> University of Bergen,
Norway.*

*Correspondence to: <timot@bacri.eu>*

This repository contains the code used for the presentation on December 6 2022 of the self selected topic of Timothée Bacri, during his PhD at the University of Bergen.
The presentation was held physically, and the slides and talk were recorded.

The video of the presentation can be found at https://youtu.be/3wbqr1D04Bw.

## Building / compiling the PDF slides

You need to unzip [monitoring_progress_bar.zip](https://github.com/timothee-bacri/introduction-parallel-processing/blob/main/code%20and%20slides/monitoring_progress_bar.zip).
The video was too heavy to upload on GitHub, so I had to compress it.

A PDF for the slides can be compiled with the `knitr` and `rmarkdown` packages using `R` from the file [fast_computing.Rmd](https://github.com/timothee-bacri/introduction-parallel-processing/blob/main/code%20and%20slides/fast_computing.Rmd) file.
It is advised to open the file [Self-selected topic.Rproj](https://github.com/timothee-bacri/introduction-parallel-processing/blob/main/code%20and%20slides/Self-selected%20topic.Rproj) to set the working directory automatically.

The code on the slide **Race condition / concurrent writing** is cached because otherwise, it intentionally causes some errors and the user must click OK on the windows that pops up. Remove `cache=TRUE` or change it to `cache=FALSE` to compile these parts.

You can click on the `knit` button on RStudio. Alternatively, you can execute the following `R` command to compile the .Rmd file
```r
rmarkdown::render('fast_computing.Rmd',  encoding = 'UTF-8');
```

## Author

**Timothée Bacri** - [timothee-bacri](https://github.com/timothee-bacri)

## License

© 2020 Timothée Bacri

The content of this project itself is licensed under the [MIT License](LICENSE), and the underlying source code is
licensed under the [GNU GPLv3 License](LICENSE_GNU.md).
