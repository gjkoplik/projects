+++
title = "Projects"
template = "page.html"
+++

Short introductions and links for the projects in my portfolio. If you have questions or suggestions, reach out on [LinkedIn](https://www.linkedin.com/in/garykoplik/).

## [Hiveplotlib](https://hiveplotlib.readthedocs.io/stable/)

*2020 - present*

I created hiveplotlib, an open-source Python package for generating hive plots. Originally developed by Martin Krzywinski, hive plots produce well-defined figures that allow for interpretable, visual explorations of network data. Current work includes speedups for hive plots as an exploratory data analysis tool, a custom multi-agent Claude Code harness, and an LLM-maintained project wiki that drives research and architecture decisions.

<p class="project-links">
<a href="https://gitlab.com/hiveplotlib/hiveplotlib"><i class="fa-brands fa-gitlab"></i>GitLab</a>
<a href="https://pypi.org/project/hiveplotlib/"><i class="fa-brands fa-python"></i>PyPI</a>
<a href="https://hiveplotlib.readthedocs.io/stable/"><i class="fa-solid fa-book"></i>Documentation</a>
<a href="https://medium.com/data-science/introducing-hiveplotlib-31014cefc7ac"><i class="fa-solid fa-newspaper"></i>Blog post</a>
</p>

{{ img(path="images/karate_club.png", class="project-img project-img-narrow", alt="Hive plot of the karate club network") }}

<hr>

## [Topological Signal Compression](https://geomdata.gitlab.io/topological-signal-compression/index.html)

*2021 - 2023*

I led a four-person research effort at Geometric Data Analytics to assess a persistent homology-based signal compression algorithm, published to PyPI with online documentation. We presented at the 2023 IEEE Aerospace Conference and received the Best Paper award for the Remote Sensing Track.

<p class="project-links">
<a href="https://gitlab.com/geomdata/topological-signal-compression"><i class="fa-brands fa-gitlab"></i>GitLab</a>
<a href="https://pypi.org/project/topological-signal-compression/"><i class="fa-brands fa-python"></i>PyPI</a>
<a href="https://geomdata.gitlab.io/topological-signal-compression/index.html"><i class="fa-solid fa-book"></i>Documentation</a>
<a href="https://ieeexplore.ieee.org/abstract/document/10115654"><i class="fa-solid fa-file-lines"></i>IEEE Xplore</a>
<a href="https://arxiv.org/abs/2206.07486"><i class="fa-solid fa-file-lines"></i>arXiv</a>
<a href="../slides/topological_signal_compression_3_9_23.pdf"><i class="fa-solid fa-person-chalkboard"></i>Slides</a>
</p>

{{ img(path="images/accuracy_numeric_axes.png", class="project-img", alt="Classification accuracy across compression levels, with Topological Signal Compression outperforming other lossy methods") }}

<hr>

## [Polar Parallel Coordinates Plots](https://arxiv.org/abs/2109.10193)

*2021*

With Ashlee Valente, I developed a novel visualization technique combining concepts from parallel coordinates plots and hive plots. Implemented in hiveplotlib as of v0.16.

<p class="project-links">
<a href="https://gitlab.com/hiveplotlib/hiveplotlib"><i class="fa-brands fa-gitlab"></i>GitLab</a>
<a href="https://pypi.org/project/hiveplotlib/"><i class="fa-brands fa-python"></i>PyPI</a>
<a href="https://hiveplotlib.readthedocs.io/stable/"><i class="fa-solid fa-book"></i>Documentation</a>
<a href="https://arxiv.org/abs/2109.10193"><i class="fa-solid fa-file-lines"></i>arXiv</a>
</p>

{{ img_pair(path1="images/p2cp_3_space.jpg", alt1="Four Gaussian blobs at the corners of a cube in 3-space", path2="images/p2cp.png", alt2="The same data shown as a polar parallel coordinates plot") }}

<hr>

## [Downloading and Parsing U.S. Treasury Auctions Data](https://gjkoplik.github.io/get_treasury_data/)

*2018*

I wrote a batch file to run Python and R code that downloads and parses U.S. Treasury auctions data. The resulting datasets offer more detail than other freely available resources. The writeup walks through the implementation and demonstrates some of the richness of the data through an exploratory analysis of 2-year note auctions.

<p class="project-links">
<a href="https://github.com/gjkoplik/get_treasury_data"><i class="fa-brands fa-github"></i>GitHub</a>
<a href="https://gjkoplik.github.io/get_treasury_data/"><i class="fa-solid fa-newspaper"></i>Project write-up</a>
</p>

{{ img(path="images/two_year_source_of_bids.png", class="project-img", alt="Source of bids for 2-year note auctions over time") }}

<hr>

## [Normalized Cross Correlation](https://gjkoplik.github.io/normalized_cross_correlation/)

*2018*

I go through the math and implementation of normalized cross correlation for object detection with a toy example.

<p class="project-links">
<a href="https://github.com/gjkoplik/normalized_cross_correlation"><i class="fa-brands fa-github"></i>GitHub</a>
<a href="https://gjkoplik.github.io/normalized_cross_correlation/"><i class="fa-solid fa-newspaper"></i>Project write-up</a>
</p>

{{ img(path="images/webpage_figure_cross_cor.png", class="project-img", alt="Normalized cross correlation example") }}

<hr>

## [Spectral Clustering](https://gjkoplik.github.io/spectral_clustering/)

*2017*

I go through the theory of k-means and spectral clustering, with examples of their varying performance.

<p class="project-links">
<a href="https://github.com/gjkoplik/spectral_clustering"><i class="fa-brands fa-github"></i>GitHub</a>
<a href="https://gjkoplik.github.io/spectral_clustering/"><i class="fa-solid fa-newspaper"></i>Project write-up</a>
</p>

{{ img(path="images/swiss_roll_combine.gif", class="project-img", alt="k-means versus spectral clustering on a swiss roll dataset") }}

<hr>

## [Interactive Index of Well-Being](https://gjkoplik.github.io/Index-of-Well-Being/)

*2017*

I created a county-level index of well-being using data on obesity, poverty, unemployment, and high-school graduation rates. The interactive map assigns equal weights to each variable, and a companion R Shiny app lets the user change the weights.

<p class="project-links">
<a href="https://github.com/gjkoplik/Index-of-Well-Being"><i class="fa-brands fa-github"></i>GitHub</a>
<a href="https://gjkoplik.github.io/Index-of-Well-Being/"><i class="fa-solid fa-newspaper"></i>Project write-up</a>
<a href="https://gary-koplik.shinyapps.io/index_of_well_being_shiny/"><i class="fa-solid fa-sliders"></i>Shiny app</a>
</p>

{{ embed(path="index_well_being_map.html", title="Interactive county-level index of well-being map") }}
