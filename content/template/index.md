---
title: Introduction to Research Skills
date: "2023-10-08"
format: hugo-md
type: revealjs
execute:
  echo: true
draft: true
---

## Heading

<!-- these fences CANNOT be nested -->

::{.incremental}

-   something
-   another thing

not a bullet point but still incremental

::

## Image captions

-   `.frame` class adds a white border to image and caption
-   `.rot` class slightly rotates image and caption
-   `source=` attribute adds link to source in caption

<img src="../humanChimpChromosomes.png" class="frame rot" data-source="http://book.bionumbers.org/how-many-chromosomes-are-found-in-different-organisms/" height="500" alt="Human chromosome 2 and analogous chimp chromosomes, adapted from Yunis+&amp;+Prakash, Science, 215:1525, 1982" /> --\>

<!-- The below produces an animated timeline of CV -->
 <h2 class="hidden" auto-animate="true" auto-animate-easing="ease-in-out">Who am I?</h2>
<div class="animate-title" data-id="animate-title">Who am I?</div>
<div class="timeline">
<div class="line" data-id="line"></div><ul><li data-id="p1"><div class="when">2011-2015</div>
<div class="what">PhD Psychology</div>
<div class="where">University of Edinburgh</div></li></ul></alt-div>
<h2 class="hidden" auto-animate="true" auto-animate-easing="ease-in-out"></h2>
<div class="animate-title" data-id="animate-title">Who am I?</div>
<div class="timeline">
<div class="line" data-id="line"></div><ul><li data-id="p1"><div class="when">2011-2015</div>
<div class="what">PhD Psychology</div>
<div class="where">University of Edinburgh</div></li><li data-id="p2"><div class="when">2015-2017</div>
<div class="what">Psychometrics</div>
<div class="where">Royal College of Surgeons of Edinburgh</div></li></ul></alt-div>
<h2 class="hidden" auto-animate="true" auto-animate-easing="ease-in-out"></h2>
<div class="animate-title" data-id="animate-title">Who am I?</div>
<div class="timeline">
<div class="line" data-id="line"></div><ul><li data-id="p1"><div class="when">2011-2015</div>
<div class="what">PhD Psychology</div>
<div class="where">University of Edinburgh</div></li><li data-id="p2"><div class="when">2015-2017</div>
<div class="what">Psychometrics</div>
<div class="where">Royal College of Surgeons of Edinburgh</div></li><li data-id="p3"><div class="when">2017-2022</div>
<div class="what">Teacher/Lecturer in research methods & statistics</div>
<div class="where">Universities of Edinburgh and Sussex</div></li></ul></alt-div>
<h2 class="hidden" auto-animate="true" auto-animate-easing="ease-in-out"></h2>
<div class="animate-title" data-id="animate-title">Who am I?</div>
<div class="timeline">
<div class="line" data-id="line"></div><ul><li data-id="p1"><div class="when">2011-2015</div>
<div class="what">PhD Psychology</div>
<div class="where">University of Edinburgh</div></li><li data-id="p2"><div class="when">2015-2017</div>
<div class="what">Psychometrics</div>
<div class="where">Royal College of Surgeons of Edinburgh</div></li><li data-id="p3"><div class="when">2017-2022</div>
<div class="what">Teacher/Lecturer in research methods & statistics</div>
<div class="where">Universities of Edinburgh and Sussex</div></li><li data-id="p4"><div class="when">2022-present</div>
<div class="what">Research associate</div>
<div class="where">InfAR @ Bauhaus</div></li></ul></alt-div>
 

## scatter

-   `R` plots are displayed in tabsets with code available
-   custom `ggplot2` theme set by default

``` r
df <- tibble::tibble(x = rnorm(100), y = x + rnorm(100))
df |>
    ggplot(aes(x, y)) +
    geom_point() +
    labs(x = "blah", y = "blee")
```

<img src="index.markdown_strict_files/figure-markdown_strict/unnamed-chunk-2-1.png" width="768" />