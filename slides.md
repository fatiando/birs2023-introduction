<!--
-------------------------------------------------------------------------------
This file defines the contents of each slide.
The reveal.js configuration can be found in index.html
-------------------------------------------------------------------------------
-->

<!-- .slide: class="slide-title" data-background-image="assets/title-slide.svg" data-background-color="#000000" data-background-size="contain" -->

<!-- Place the content at the bottom of the slide -->
<div class="r-stretch">
</div>

<h1 id="talk-title">
  The Fatiando a Terra project
</h1>
<p id="talk-authors">
  <a href="https://www.leouieda.com" id="talk-speaker">Leonardo Uieda</a>
</p>

<!-- Place location and date side-by-side with affiliation logos -->
<div class="row talk-info">
<div class="col-large">

<i class="fa fa-calendar-alt" style="margin: 0 10px 0 0"></i>
28 July 2023

BIRS Workshop:  Open-Source Tools to Enable Geophysical Data Processing and Inversion

<!-- Permission to reuse and CC-BY license logo -->
<i class="fa fa-camera" style="margin: 0 10px 0 0"></i>
Feel free to screenshot/share/reuse this presentation
<span style="margin: 0 20px"></span>
<a href="https://creativecommons.org/licenses/by/4.0/"><i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by" style="margin: 0 10px 0 2px"></i>CC-BY 4.0 License</a>

</div>
<div class="col-medium">

<!-- Add logos here. Need these wrappers to align them to the bottom right -->
<div class="talk-logos-container">
<div class="talk-logos">
  <a href="https://www.compgeolab.org"><img src="assets/compgeolab-banner-light.svg" alt="Computer-Oriented Geoscience Lab"></a>
</div>
</div>

</div>
</div>

===============================================================================

<!-- .slide: data-background-video="assets/brasil-sao-paulo-rio.mp4" data-background-size="contain" data-background-color="#000000" -->

<div class="r-stretch">
</div>
<div class="footnote-left dark">

Our journey starts in Brazil at the University of São Paulo and the National
Observatory in Rio de Janeiro

</div>

===============================================================================

<!-- .slide: data-background-image="assets/fatiando-as-a-gravmag-gui.svg" data-background-size="contain" data-background-color="#ffffff" -->

<div class="r-stretch">
</div>
<div class="footnote dark">

Initial idea developed around 2008 by **undergrads** at USP as a GUI for **2D
forward modelling**

</div>

===============================================================================

<!-- .slide: data-background-image="assets/fatiando-first-commit.svg" data-background-size="contain" data-background-repeat="no-repeat" -->

<div class="r-stretch">
</div>
<div class="footnote">

Became a **Python library** in 2010 when I started my MSc in Rio working on 3D
gravity gradient inversion
(commit: [928515b](https://github.com/fatiando/fatiando/commit/928515b0fcfdccecbc4f661ed2469390ef43ec1d))

</div>

===============================================================================

<!-- .slide: data-background-image="assets/fatiando-first-commit-vcs.svg" data-background-size="contain" data-background-repeat="no-repeat" -->

<div class="r-stretch">
</div>
<div class="footnote-left">

Went through 3 version control systems.
Learned a lot about software engineering

</div>

===============================================================================

<!-- .slide: data-background-video="assets/planting-inversion.mp4" data-background-size="contain" data-background-color="#ffffff" -->

<div class="r-stretch">
</div>
<div class="footnote-left">

Used it for my MSc thesis and included a lot of potential-field processing and
inversion functions
<br>
Animation from [Uieda & Barbosa (2012)](https://doi.org/10.6084/m9.figshare.91469.v1)

</div>

===============================================================================

<!-- .slide: data-background-video="assets/seismic-waves-demo.mp4" data-background-size="contain" data-background-color="#ffffff" -->

<div class="r-stretch">
</div>
<div class="footnote-left">

Included a bunch of other things as well that were useful in teaching
(notebook from <i class="fab fa-github"></i>
[leouieda/geofisica2](https://github.com/leouieda/geofisica2))

</div>

===============================================================================

<div class="row">
<div class="col">
<h1 style="color: #0000dd;">
<i class="far fa-thumbs-up" style="margin-right: 20px;"></i>
The good parts
</h1>
<ul class="fa-ul">
<li>
<span class="fa-li"> <i class="fa fa-lightbulb fa-fw"></i> </span>
State-of-the-art algorithms
</li>
<li>
<span class="fa-li"> <i class="fa fa-file-alt fa-fw"></i> </span>
Used in several thesis & papers (>70 citations)
</li>
<li>
<span class="fa-li"> <i class="fa fa-users fa-fw"></i> </span>
2-3 active contributors
</li>
<li>
<span class="fa-li"> <i class="fa fa-chalkboard-teacher fa-fw"></i> </span>
Enabled teaching through simulation
</li>
</ul>
</div>
<div class="col fragment">
<h1 style="color: #dd0000;">
<i class="far fa-thumbs-down" style="margin-right: 20px;"></i>
The bad parts
</h1>
<ul class="fa-ul">
<li>
<span class="fa-li"> <i class="fa fa-gamepad fa-fw"></i> </span>
Too many toy problems and experimental/untested code
</li>
<li>
<span class="fa-li"> <i class="fas fa-vial fa-fw"></i> </span>
Not designed for testability
</li>
<li>
<span class="fa-li"> <i class="fa fa-tools fa-fw"></i> </span>
Difficult to maintain
</li>
<li>
<span class="fa-li"> <i class="fa fa-landmark fa-fw"></i> </span>
Unstable foundations for growth
</li>
</ul>
</div>
</div>

===============================================================================

<!-- .slide: class="slide-transition" -->

<div class="r-stretch centered">
<div>
Enter

# The Geophysics Python Stack

<img style="width: 15%" src="assets/simpeg-logo.png">
<img style="width: 15%" src="assets/pygimli-logo.svg">
<img style="width: 15%" src="assets/gempy-logo.png">
<img style="width: 15%" src="assets/pyvista-logo.png">
<img style="width: 15%" src="assets/emsig-logo.svg">
</div>
</div>
<div class="footnote-left">

All of these tools were taking off around 2017-2018 so we had to do some
soul-searching to see where Fatiando fit in

</div>

===============================================================================

<!-- .slide: class="slide-transition" -->

<div class="r-stretch centered">
<div>

# Fatiando is dead.<br> <span class="fragment">Long live Fatiando!</span>

</div>
</div>
<div class="footnote-left fragment">

Read more about it in
[this blog post from 2018](https://www.leouieda.com/blog/future-of-fatiando.html)

</div>


===============================================================================

<div class="row small">
<div class="col fragment">

## Pooch

Data <b>download & caching</b>
<br>
(used by a lot of the Scipy stack)

<ul class="fa-ul">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/pooch">fatiando/pooch</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
<div class="col fragment">

## Verde

Spatial/point data processing and <b>interpolation</b> with a pinch of ML

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/verde">fatiando/verde</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
<div class="col fragment">

## Harmonica

Processing, modeling, and inversion of <b>gravity & magnetic</b> data

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/harmonica">fatiando/harmonica</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
</div>
<hr style="margin: 1em 0">
<div class="row small">
<div class="col fragment">

## Boule

Defines reference <b>ellipsoids</b> and calculates <b>normal gravity</b>

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/boule">fatiando/boule</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

## Ensaio

Collection for curated open-access **sample geophysics datasets**

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/ensaio">fatiando/ensaio</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

## Choclo

Highly optimized <b>forward modeling kernel</b> functions

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/choclo">fatiando/choclo</a>
</li>
<li><i class="fa-li fa fa-flask fa-fw" style="color: orange" title="Project status"></i>
    Early stages of design
</li>
</ul>

</div>
</div>


===============================================================================

<!-- .slide: data-background-image="assets/fatiando-community-call.jpg" data-background-size="contain" -->

<div class="quote dark">

Come for the <strong>code</strong> <i class="fas fa-code"></i>
<br>
Stay for the <strong>community</strong> <i class="fas fa-users"></i>

</div>

===============================================================================

<div class="r-stretch centered">
<div>

# Steering Council

<div class="row">
<div class="col">
<img src="https://github.com/aguspesce.png">

Agustina Pesce

</div>
<div class="col">
<img src="https://github.com/MGomezN.png">

Mariana Gomez

</div>
<div class="col">
<img src="https://github.com/leouieda.png">

Leonardo Uieda

</div>
<div class="col">
<img src="https://github.com/santisoler.png">

Santiago Soler

</div>
<div class="col">
<img src="https://github.com/LL-Geo.png">

Lu Li

</div>
</div>

</div>
</div>
<div class="footnote">

Read more about our
[project governance](https://github.com/fatiando/community/blob/main/GOVERNANCE.md)
(inspired by the SimPEG structure 😊)

</div>

===============================================================================

<!-- .slide: class="slide-transition" -->

# 1.<br> Full transparency<br> is the default

===============================================================================

<!-- .slide: class="slide-transition" -->

# 2.<br> Generously give <br> permission, responsibility, knowledge

===============================================================================

# Roadmap

1. <!-- .element: class="fragment" --> Full gravity processing in Harmonica
1. <!-- .element: class="fragment" --> Non-linear layer inversion in Harmonica
1. <!-- .element: class="fragment" --> 3D planting inversion in Harmonica
1. <!-- .element: class="fragment" --> Use Choclo in Harmonica and SimPEG
1. <!-- .element: class="fragment" --> What would a general-purpose inversion framework look like?
1. <!-- .element: class="fragment" --> Expand kernels in Choclo (polygonal prisms, polyhedra)
1. <!-- .element: class="fragment" --> Verde 2.0.0: New interpolators, better defaults
1. <!-- .element: class="fragment" --> Funding for workshops/events at conferences

===============================================================================

<!-- .slide: class="slide-contact" data-background-image="assets/contact-slide.svg" data-background-size="contain" data-background-color="#000000" -->

<i class="fas fa-info-circle"></i>
<br>
Find out more:
<a href="https://www.fatiando.org">www.fatiando.org</a>

<i class="fab fa-github"></i>
<br>
Source code for this presentation:
<br>
[github.com/fatiando/birs2023-introduction](https://github.com/fatiando/birs2023-introduction)

<i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by"></i>
<br>
Unless otherwise noted,
the contents of this presentation are
licensed under the
<br>
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
<br>
These license terms do not apply to project logos and profile photos.
