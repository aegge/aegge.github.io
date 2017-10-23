---
layout: slide
title: The One-Loop Galaxy Bispectrum
description:
theme: serif
transition: slide
author_profile: false
categories: presentation
---

<style type="text/css">
  .reveal .slides {
        margin-top: -.1em;
        text-align: left; }      
  .reveal {
        font-size: 26px; }
  .reveal h1 {
        font-size: 2.5em; }
  .reveal h2 {
        font-size: 1.75em; }
  .reveal h3 {
        font-size: 1.25em;
        text-transform: none; }
  .reveal h4 {
        font-size: 1.em; }
}
</style>

<style>
  .column {
      float: left;
      width: 50%;
  }

  .row:after {
      content: "";
      display: table;
      clear: both;
  }
  .verticalLine {
    border-left: thick solid #ff0000;
  }
</style>

<!-- <script>
	var link = document.createElement( 'link' );
	link.rel = 'stylesheet';
	link.type = 'text/css';
	link.href = window.location.search.match( /print-pdf/gi ) ? 'css/print/pdf.css' : 'css/print/paper.css';
	document.getElementsByTagName( 'head' )[0].appendChild( link );
</script> -->


<section data-markdown data-separator="^\n---\n$"
         data-separator-vertical="^\n--\n$"
         data-element-attributes="{_\s*?([^}]+?)}"
         data-separator-notes="^Note:"             >
<script type="text/template">
<!-- {_style="text-align: center"}-->
<br>
<!-- # The Galaxy Bispectrum -->
<img src="/presentations/title.png", style="background:none; border:none; box-shadow:none;"/>

<br><br>

### Alexander Eggemeier
<img src="/presentations/sussex_logo_blue.png", style="width:125px; background:none; border:none; box-shadow:none;"/>

with Roman Scoccimarro & Robert E. Smith

---


<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Motivation</b> </span>

---

<!-- {_style="text-align: center"}-->
# Clustering Measures

<br>
**Two-point statistics** $\quad \quad \quad \quad \quad \quad$ **Three-point statistics**
<img src="/presentations/millennium_arrows.png", style="border:none; background:none; box-shadow:none; width:2000px; height:200px"/>
<p style="margin-top: -20px">
</p>

`$\text{density field: } \hspace{0.3em} \delta(\boldsymbol{x}) = \frac{n(\boldsymbol{x})-\bar{n}}{\bar{n}}
  \hspace{0.3em} \overset{\mathrm{FT}}{\longleftrightarrow} \hspace{0.3em} \delta(\boldsymbol{k})$`

<p>
  <hr style="height:1.5em; visibility:hidden;"/>
</p>

<div style="position:relative"><!-- {_style="text-align: left"}-->
  <span class="fragment fade-in" style="position:absolute; margin-left: auto; margin-right: auto; left: 0; right: 0; top:5;" data-fragment-index="3">
    `
    $
    \definecolor{blue}{RGB}{81,167,249}
    \definecolor{yellow}{RGB}{245,211,40}
    \langle \delta(\boldsymbol{k})\,\delta(\boldsymbol{k}')\rangle = (2\pi)^3 \fcolorbox{blue}{}{$P(k)$} \delta_D(\boldsymbol{k}+\boldsymbol{k}')
    $
    `
  </span>
  <span class="fragment fade-in" style="position:absolute; margin-left: auto; margin-right: auto; left: 40; right: 0; margin-top:20;" data-fragment-index="3">
    `
    $
    \langle \delta(\boldsymbol{k}_1)\,\delta(\boldsymbol{k}_2)\,\delta(\boldsymbol{k}_3)\rangle = (2\pi)^3 \fcolorbox{yellow}{}{$B(k_1,k_2,k_3)$} \\ \hspace{9em}\times\,\delta_D(\boldsymbol{k}_1+\boldsymbol{k}_2+\boldsymbol{k}_3)
    $
    `
  </span>
</div>

Note:
- to extract physics from LSS we measure statistics (don't know the initial conditions)

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="slide-in fade-out"-->
# Why Go Beyond $P(k)$?

### I) The observed density field is <span style="color:red">non-Gaussian</span>


<div style="font-size:98%" class="fragment" data-fragment-index="1">
`
$$
\hspace{-0.55em}\substack{\text{If $\delta$ is} \\ \text{Gaussian}} \, \rightarrow \, {\cal P}(\delta_1,\dots,\delta_N) \propto \exp{\left[-\frac{1}{2}(\delta_1,\dots,\delta_N) C^{-1}\left(\begin{array}{c} \delta_1 \\ \vdots \\ \delta_N \end{array}\right)\right]},\;
C \equiv \left(\begin{array}{ccc} \sigma^2 & \xi_{12} & \cdots \\ \xi_{21} & \sigma^2 & \cdots \\ \vdots & \vdots & \ddots \end{array}\right)
$$
`
</div>


<img class="fragment" data-fragment-index="2" src="/presentations/pdf01.png", style="width:430px; background:none; border:none; box-shadow:none; float:left"/>

<div class="fragment" data-fragment-index="2"><!-- {_style="text-align: left"}-->
  <br><br>
  Non-linear evolution, e.g.:
  `
  $$
  \frac{\partial \delta(\boldsymbol{x},\tau)}{\partial \tau} + \boldsymbol{\nabla} \cdot \Big[\Big(1+\color{red}\delta(\boldsymbol{x},\tau)\color{black}\Big)\color{red}u(\boldsymbol{x},\tau)\color{black}\Big] = 0
  $$
  `
</div>
<br>
<div class="fragment" data-fragment-index="3"><!-- {_style="text-align: left"}-->
  Galaxy bias:
  `
  $$
  \delta_g(\boldsymbol{x}) = b_1\,\delta(\boldsymbol{x}) + b_2\,\color{red}\delta(\boldsymbol{x})^2\color{black} + \ldots
  $$
  `
</div>

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="fade-in slide-out"-->
# Why Go Beyond $P(k)$?

### I) The observed density field is <span style="color:red">non-Gaussian</span>


<div style="font-size:98%">
`
$$
\hspace{-0.55em}\substack{\text{If $\delta$ is} \\ \text{Gaussian}} \, \rightarrow \, {\cal P}(\delta_1,\dots,\delta_N) \propto \exp{\left[-\frac{1}{2}(\delta_1,\dots,\delta_N) C^{-1}\left(\begin{array}{c} \delta_1 \\ \vdots \\ \delta_N \end{array}\right)\right]},\;
C \equiv \left(\begin{array}{ccc} \sigma^2 & \xi_{12} & \cdots \\ \xi_{21} & \sigma^2 & \cdots \\ \vdots & \vdots & \ddots \end{array}\right)
$$
`
</div>


<img src="/presentations/pdf02.png", style="width:430px; background:none; border:none; box-shadow:none; float:left"/>

<div><!-- {_style="text-align: left"}-->
  <br><br>
  Non-linear evolution, e.g.:
  `
  $$
  \frac{\partial \delta(\boldsymbol{x},\tau)}{\partial \tau} + \boldsymbol{\nabla} \cdot \Big[\Big(1+\color{red}\delta(\boldsymbol{x},\tau)\color{black}\Big)\color{red}u(\boldsymbol{x},\tau)\color{black}\Big] = 0
  $$
  `
</div>
<br>
<div><!-- {_style="text-align: left"}-->
  Galaxy bias:
  `
  $$
  \delta_g(\boldsymbol{x}) = b_1\,\delta(\boldsymbol{x}) + b_2\,\color{red}\delta(\boldsymbol{x})^2\color{black} + \ldots
  $$
  `
</div>

---

<!-- {_style="text-align: center"}-->
# Why Go Beyond $P(k)$?

### II) Breaking parameter <span style="color:red">degeneracies</span>

<br>

<div><ul>
 <li> between _bias_ and _amplitude of fluctuations_  $\,$ [<span style="color:DarkTurquoise">Fry '94, Verde+ '98, ... </span>] </li>
</ul></div> <!-- {_style="text-align: left"}-->
<p>
`
$$
\begin{align}
\text{Power spectrum: } \quad &P_{\text{g}} \sim b_1^2\,\sigma_8^2 \\[1em]
\text{Bispectrum: } \quad &B_{\text{g}} \sim \left[b_1^3\,\sigma_8^4\right] +  \left[b_1^2\,b_2\,\sigma_8^4\right] + \ldots
\end{align}
$$
`
</p> <!-- {_style="text-align: center"}-->

<div><ul>
 <li> between _growth rate_ and _amplitude of fluctuations_ $\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad\quad$ [<span style="color:DarkTurquoise">Scoccimarro+ '99, Gil-Marin+ '14/15, ... </span>] </li>
</ul></div> <!-- {_style="text-align: left"}-->
<p>
`
$$
\begin{align}
\hspace{-8em}\text{Power spectrum: } \quad &P_{\text{g}} \sim f^2\,\sigma_8^2 \\[1em]
\text{Bispectrum: } \quad &B_{\text{g}} \sim \left[f^3 + \ldots \right]\sigma_8^4
\end{align}
$$
`
</p>

---

<!-- {_style="text-align: center"}-->
# Why Go Beyond $P(k)$?

### III) <span style="color:red">Cosmic variance limit</span> is approaching [<span style="color:DarkTurquoise">Dore+ '14</span>]

<img src="/presentations/spherex2.png", style="width:680px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="slide-in none-out"-->
# The Challenges <!-- {_style="text-align: center"}-->

<ul>
  <li style="border:3px; border-style:solid; border-color:#f0f1eb; padding: 5px; padding-left: 20px">
    <p><b>Accurate covariance matrices for large data sets</b></p>

    <p>Bispectrum number of triangles scales as `$N_{\Delta} \sim \left(k_{\text{max}}/\Delta k\right)^3$` [power spectrum bins:
    `$\sim k_{\text{max}}/\Delta k$`]. The number of simulations to estimate `$C_B$` must be _larger_ then
    `$N_{\Delta}$ $\rightarrow\,{\cal O}(10^4)$`.</p>
  </li>
  <li style="border:3px; border-style:solid; border-color:#f0f1eb; padding: 5px; padding-left: 20px">
    <p><b>Complexity of theoretical modelling</b></p>

    <p>_Non-linear evolution_, _galaxy biasing_, _redshift space distortions_ are much harder to model for the bispectrum than for the
    power spectrum.</p>
  </li>
  <li style="border:3px; border-style:solid; border-color:#f0f1eb; padding: 5px; padding-left: 20px">
    <p><b>Observational systematics</b></p>

    <p>Survey geometry (window functions), fiber collisions, ...</p>
  </li>
</ul>

---

<!-- .slide: data-transition="fade-in slide-out"-->
# The Challenges <!-- {_style="text-align: center"}-->

<ul>
  <li style="border:3px; border-style:solid; border-color:#f0f1eb; padding: 5px; padding-left: 20px">
    <p><b>Accurate covariance matrices for large data sets</b></p>

    <p>Bispectrum number of triangles scales as `$N_{\Delta} \sim \left(k_{\text{max}}/\Delta k\right)^3$` [power spectrum bins:
    `$\sim k_{\text{max}}/\Delta k$`]. The number of simulations to estimate `$C_B$` must be _larger_ then
    `$N_{\Delta}$ $\rightarrow\,{\cal O}(10^4)$`.</p>
  </li>
  <li style="border:3px; border-style:solid; border-color:red; padding: 5px; padding-left: 20px">
    <p><b>Complexity of theoretical modelling</b></p>

    <p>_Non-linear evolution_, _galaxy biasing_, _redshift space distortions_ are much harder to model for the bispectrum than for the
    power spectrum.</p>
  </li>
  <li style="border:3px; border-style:solid; border-color:#f0f1eb; padding: 5px; padding-left: 20px">
    <p><b>Observational systematics</b></p>

    <p>Survey geometry (window functions), fiber collisions, ...</p>
  </li>
</ul>

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Introduction to Galaxy Bias</b> </span>

---

<!-- .slide: data-transition="slide-in fade-out" data-background-image="/presentations/pop_day.png"-->

---

<!-- .slide: data-transition="fade-in slide-out" data-background-image="/presentations/pop_night.png"-->

---

<!-- {_style="text-align: center"}-->
# The First Detection

<img src="/presentations/bias_peebles_hauser.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 26em; left: 20.5em; width: 400px; height: 150px;">
[<span style="color:DarkTurquoise">Peebles & Hauser '74</span>]
</div>


---

# The Modelling Perspective <!-- {_style="text-align: center"}-->

<ul>
  <li>
    goal of **Perturbation Theory (PT)**: expand nonlinear (evolved) density in increasing powers of linear (initial) matter density `$\delta^{(1)}(\boldsymbol{k})$`:
    <p>
      `
      $$
      \delta(\boldsymbol{k}) = \sum_n \delta^{(n)}(\boldsymbol{k})\,, \hspace{1em} \mathrm{where} \hspace{0.5em} \delta^{(n)}(\boldsymbol{k}) \sim \int {\cal K}(\boldsymbol{k}_1,\ldots,\boldsymbol{k}_n)\,\delta^{(1)}(\boldsymbol{k}_1) \cdots \delta^{(1)}(\boldsymbol{k}_n)
      $$
      `
    </p>
    <p><span style="color:red"> <b>Assumption:</b> `$\delta^{(1)}$` is Gaussian </span></p> <!-- {_style="text-align: center"}-->
  </li>
  <li>
    <p class="fragment"> use linear power spectrum as building block to construct observables:
      `
      $$
      \begin{align}
      \\[0.1em]
      \Rightarrow \hspace{1em} P(k) &= \underbrace{P_{\mathrm{tree}}(k)}_{\langle\delta^{(1)}\delta^{(1)}\rangle} \hspace{0.3em} + \underbrace{P_{\mathrm{1-loop}}(k)}_{\langle\delta^{(1)}\delta^{(3)}\rangle,\hspace{0.25em}\langle\delta^{(2)}\delta^{(2)}\rangle} + \ldots \\[1em]
      \Rightarrow \hspace{1em} B(k_1,k_2,k_3) &= \underbrace{B_{\mathrm{tree}}(k_1,k_2,k_3)}_{\langle\delta^{(1)}\delta^{(1)}\delta^{(2)}\rangle} \hspace{0.3em} + \underbrace{B_{\mathrm{1-loop}}(k_1,k_2,k_3)}_{\substack{\langle\delta^{(4)}\delta^{(1)}\delta^{(1)}\rangle,\hspace{0.25em}\langle\delta^{(3)}\delta^{(2)}\delta^{(1)}\rangle,\\ \langle\delta^{(2)}\delta^{(2)}\delta^{(2)}\rangle}} + \ldots
      \end{align}
      $$
      `
    </p>
  </li>
</ul>


Note:
  - remember from previous slide: Gaussian means that all information is contained in the power spectrum

---

# The Modelling Perspective <!-- {_style="text-align: center"}-->

In the spirit of PT: need to relate galaxy density to matter density:
<span class="fragment" data-fragment-index="1"></span>
<p>
`
$$
\fragment{1}{\delta_g(\boldsymbol{x}) = b_1\,\delta(\boldsymbol{x})} \fragment{2}{+ \color{red} \frac{b_2}{2!}\,\delta^2(\boldsymbol{x}) \color{black}} \fragment{3}{+ \color{#1a3f8b} \gamma_2\,{\cal G}_2(\boldsymbol{x})} \fragment{2}{\color{black} + \color{red} \frac{b_3}{3!}\,\delta^3(\boldsymbol{x}) \color{black} + \ldots}
$$
`
</p>

<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>

<ul>
  <li class="fragment" data-fragment-index="2">
    linear bias parameter: `$b_1$`, OK on large enough scales [Kaiser '84]
  </li>
  <p>
    <hr style="height:0.1em; visibility:hidden;"/>
  </p>
  <span style="color:red">
    <li class="fragment" data-fragment-index="3">
      local (Eulerian) bias expansion, depends only on matter density at <b>SAME</b> point in space [Fry & Gaztanaga '93]
    </li>
  </span>
  <p>
    <hr style="height:0.1em; visibility:hidden;"/>
  </p>
  <span style="color:#1a3f8b">
    <li class="fragment" data-fragment-index="4">
      galaxy density should depend on <b>ENVIRONMENT</b> $\rightarrow$ bias due to tidal field [McDonald & Roy '09, Chan+ '12, Baldauf+ '12]
    </li>
  </span>
</ul>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/bspec_BOSSlike_nomodel.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/bspec_BOSSlike.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_BOSSlike_kmax0p1.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

<div style="position: absolute; top: 5em; left: 0.em; width: 350px; height: 600px;">
  <h3> Model Assumptions: </h3>
  <ul>
    <li>
      full galaxy power spectrum to 1-loop order, <br> 1-loop matter bispectrum + <b>tree-level bias</b>
    </li>
    <p></p>
    <li class="fragment" data-fragment-index="2">
      local <b>Lagrangian</b> bias
      <p>
        `
        $$
        \Rightarrow \hspace{0.5em} \gamma_2 = -\frac{2}{7} (b_1-1)
        $$
        `
      </p>
    </li>
    <li class="fragment" data-fragment-index="3">
      treatment of noise:
      <p>
        `
        $$
        P_{\mathrm{noise}} = \epsilon_0\,P_{\mathrm{Poisson}} \\
        B_{\mathrm{noise}} = \epsilon_0\,B_{\mathrm{Poisson}}
        $$
        `
      </p>
    </li>
  </ul>
</div>

---

<!-- .slide: data-transition="fade-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_BOSSlike_kmax0p15.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

<div style="position: absolute; top: 5em; left: 0.em; width: 350px; height: 600px;">
  <h3> Model Assumptions: </h3>
  <ul>
    <li>
      full galaxy power spectrum to 1-loop order, <br> 1-loop matter bispectrum + <b>tree-level bias</b>
    </li>
    <p></p>
    <li>
      local <b>Lagrangian</b> bias
      <p>
        `
        $$
        \Rightarrow \hspace{0.5em} \gamma_2 = -\frac{2}{7} (b_1-1)
        $$
        `
      </p>
    </li>
    <li>
      treatment of noise:
      <p>
        `
        $$
        P_{\mathrm{noise}} = \epsilon_0\,P_{\mathrm{Poisson}} \\
        B_{\mathrm{noise}} = \epsilon_0\,B_{\mathrm{Poisson}}
        $$
        `
      </p>
    </li>
  </ul>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_BOSSlike_kmax0p2.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

<div style="position: absolute; top: 5em; left: 0.em; width: 350px; height: 600px;">
  <h3> Model Assumptions: </h3>
  <ul>
    <li>
      full galaxy power spectrum to 1-loop order, <br> 1-loop matter bispectrum + <b>tree-level bias</b>
    </li>
    <p></p>
    <li>
      local <b>Lagrangian</b> bias
      <p>
        `
        $$
        \Rightarrow \hspace{0.5em} \gamma_2 = -\frac{2}{7} (b_1-1)
        $$
        `
      </p>
    </li>
    <li>
      treatment of noise:
      <p>
        `
        $$
        P_{\mathrm{noise}} = \epsilon_0\,P_{\mathrm{Poisson}} \\
        B_{\mathrm{noise}} = \epsilon_0\,B_{\mathrm{Poisson}}
        $$
        `
      </p>
    </li>
  </ul>
</div>

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Taking Galaxy Bias <br> to the Next Order</b> </span>

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
<ol type="1" style="color:#f0f1eb; font-size:150%">
  <li>
    all <b>large-scale effects</b> due to galaxy evolution can be captured order by order in perturbation theory
  </li>
  <hr style="height:3.5em; visibility:hidden;"/>
  <li>
    renormalization of bias parameters can be easily dealt with in the <b>multi-point propagator formalism</b>
  </li>
</ol>

---

<!-- {_style="text-align: center"}-->
# Generalizing the Bias Expansion

<hr style="height:3.5em; visibility:hidden;"/>

<div style="font-size: 240%">
  <p>
    `
    $$
    \color{#1a3f8b}\delta_g(\boldsymbol{x},\tau) = \color{black}\underbrace{\color{#1a3f8b}F_g\left[\Phi(\boldsymbol{y},\tau=0)\right]}\color{#1a3f8b}(\boldsymbol{x},\tau)
    $$
    `
  </p>
</div>

<div style="position: absolute; top: 14em; left: 15.5em; width: 300px; height: 600px;">
  <b>functional</b> of initial potential perturbations $\Phi$
</div>

<hr style="height:7em; visibility:hidden;"/>

<p>
  <h2 class="fragment" data-fragment-index="2">... too complicated!!</h2>
</p>


---

# Spacetime Spaghettis <!-- {_style="text-align: center"}-->

<img src="/presentations/spaghetti.png", style="position:relative; top:-35px; left:8em; height:610px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 8em; left: 2em; width: 550px; height: 200px;">
  Galaxy formation is fairly **local** in space <br> (on scales $r \gg R_*$) ...
</div>

<div style="position: absolute; top: 18em; left: 20em; width: 480px; height: 200px;">
  ... but pretty **nonlocal** in time (of the order $\,\sim\,H^{-1}$)! <br><br>
  $\rightarrow \hspace{0.5em}$ must depend on entire fluid <br> $\hspace{1.6em}$ flow $\boldsymbol{x}_{\mathrm{fl}}(\tau')$
</div>

---

# What does a local observer see? <!-- {_style="text-align: center"}-->

<div style="border:5px solid #f5d328; padding:10px; border-radius:8px">
  <b>Equivalence Principle: </b> The leading locally observable effect is given by <span style="display:inline-block; width:10.3em;"></span> SECOND derivatives of the metric tensor, `$\partial_i \partial_j\,\Phi \equiv \nabla_{ij}\,\Phi$`
</div>

<p>
  `
  $$
  \\[0.5em]
  \Rightarrow \hspace{0.5em} \color{#1a3f8b}\delta_g(\boldsymbol{x},\tau) = F_g\Big[\nabla_{ij}\,\Phi(\boldsymbol{x}_{\mathrm{fl}}(\tau'))\Big](\boldsymbol{x},\tau)
  $$
  `
</p>

<hr style="height:0.15em; visibility:hidden;"/>

<p class="fragment" data-fragment-index="1">
  Dependence on fluid trajectory <b>equivalent</b> with series of (convective) derivatives:
  `
  $$
  \nabla_{ij}\,\Phi(\boldsymbol{x}_{\mathrm{fl}}(\tau')),\, \text{all } \tau' \leq \tau \hspace{0.6em} \Leftrightarrow \hspace{0.6em}
  \nabla_{ij}\,\Phi(\boldsymbol{x},\tau),\, \underbrace{\frac{\text{d}}{\text{d}\tau}\nabla_{ij}\,\Phi(\boldsymbol{x},\tau),\,\ldots}
  $$
  `
</p>

<div style="position: absolute; top: 17.3em; left: 17.5em; width: 550px; height: 200px;" class="fragment" data-fragment-index="1">
  only <b>finite</b> number of linearly independent <br> derivatives at each order in PT
</div>


<hr style="height:2em; visibility:hidden;"/>

<p class="fragment" data-fragment-index="2">
  $\rightarrow \hspace{0.3em}$ trade derivatives for dependency on <b>velocity potential</b>, `$\boldsymbol{v}(\boldsymbol{x},\tau) = \boldsymbol{\nabla} \Phi_v(\boldsymbol{x},\tau)$`
  <p class="fragment" data-fragment-index="2">
  `
  $$
  \\[0.5em]
  \Rightarrow \hspace{0.5em} \color{#1a3f8b}\delta_g(\boldsymbol{x},\tau) =  F_g\Bigg[\nabla_{ij}\,\Phi(\boldsymbol{x},\tau),\, \nabla_{ij}\,\Phi_v(\boldsymbol{x},\tau)\,;\,\tau\Bigg]
  $$
  `
  </p>
  <!-- $\rightarrow \hspace{1em}$ can replace dependency on `$\boldsymbol{x}_{\mathrm{fl}}(\tau')$` with series of derivatives `$\text{d}/\text{d}\tau$` -->
  <!-- `
  $$
  \\[0.5em]
  \text{So:} \hspace{0.5em} F_g\Big[\nabla_{ij}\,\Phi(\boldsymbol{x}_{\mathrm{fl}}(\tau'))\Big](\boldsymbol{x},\tau) \Leftrightarrow F_g\Bigg[\nabla_{ij}\,\Phi(\boldsymbol{x},\tau),\, \frac{\text{d}}{\text{d}\tau}\nabla_{ij}\,\Phi(\boldsymbol{x},\tau),\,\ldots\Bigg]
  $$
  ` -->
</p>  

Note:
  - final $\delta_g$ written only in terms of locally measurable terms
  - these are the only terms that can affect galaxy formation (to leading order in spatial derivatives)

--

<p>
  Let's consider a <b>single</b> contribution, `${\cal O}$`, to `$F_g$`:
    `
    $$
    \\[2em]
    \hspace{-3em}\int^{\tau} \text{d}\tau' f_{\cal O}(\tau,\tau')\,{\cal O}(\boldsymbol{x}_{\mathrm{fl}},\tau')
    \fragment{1}{= \Bigg[\int^{\tau} \text{d}\tau' f_{\cal O}(\tau,\tau') \Bigg]\,{\cal O}(\boldsymbol{x},\tau) \\
    \hspace{15.3em}+ \Bigg[\int^{\tau} \text{d}\tau' (\tau' - \tau) f_{\cal O}(\tau,\tau') \Bigg]\,\frac{\text{d}}{\text{d}\tau}{\cal O}(\boldsymbol{x},\tau) + \ldots}
    $$
    `
</p>  

---

# The Galileons <!-- {_style="text-align: center"}-->

<div style="border:5px solid #f5d328; padding:10px; border-radius:8px">
  <b> $\delta_g$ is a SCALAR quantity: </b> it must be independent under general coordinate $\hspace{10.6em}$ transformations
</div>

<hr style="height:0.5em; visibility:hidden;"/>

<p class="fragment" data-fragment-index="2">
  For a $3 \times 3$ tensor (such as `$\nabla_{ij}\Phi$`) there are three fundamental <b>invariants</b>:
  `
  $$
  \hspace{-6em}
  \begin{align}
    \\[0.1em]
    \left.\begin{array}{l}
      {\cal G}_1(\Phi) = \nabla^2\Phi = \delta \\
      {\cal G}_2(\Phi) = \Big(\nabla_{ij}\Phi\Big)^2 - \Big(\nabla^2\Phi\Big)^2 \\
      {\cal G}_3(\Phi) = \Big(\nabla^2\Phi\Big)^3 + 2 \nabla_{ij}\Phi\,\nabla_{jk}\Phi\,\nabla_{ki}\Phi - 3\Big(\nabla_{ij}\Phi\Big)^2\,\nabla^2\Phi
    \end{array}\right\}
  \end{align}
  $$
  `
  <!-- {\cal G}_1(\Phi) &= \nabla^2\Phi = \delta \\
  {\cal G}_2(\Phi) &= \Big(\nabla_{ij}\Phi\Big)^2 - \Big(\nabla^2\Phi\Big)^2 \\
  {\cal G}_3(\Phi) &= \Big(\nabla^2\Phi\Big)^3 + 2 \nabla_{ij}\Phi\,\nabla_{jk}\Phi\,\nabla_{ki}\Phi - 3\Big(\nabla_{ij}\Phi\Big)^2\,\nabla^2\Phi -->  

  <div style="position: absolute; top: 15.3em; left: 29.5em; width: 350px; height: 200px;" class="fragment" data-fragment-index="2">
    <b>Galileons!</b>
  </div>
</p>

<div style="color:red" class="fragment" data-fragment-index="3">
  <b>Conclusion: </b> all contributions to `$\delta_g$` can be written as linear independent `$\hspace{5.3em}$` combinations of `${\cal G}_{1/2/3}(\Phi)$` and `${\cal G}_{1/2/3}(\Phi_v)$`
</div>

<!-- style="border:5px solid red; padding:10px; border-radius:8px" -->

---

<!-- .slide: data-transition="slide-in fade-out"-->
# The Happy End <!-- {_style="text-align: center"}-->

<hr style="height:1em; visibility:hidden;"/>

<p style="border:2px solid black; padding:10px; border-radius:8px">
  `
  $$
  \begin{align}
  \delta_g(\boldsymbol{x}) &= b_1\,\delta(\boldsymbol{x}) \\
  &+\frac{b_2}{2}\,\delta^2(\boldsymbol{x}) + \gamma_2\,{\cal G}_2(\boldsymbol{x}|\Phi_v) \\
  &\fragment{1}{\hspace{0.23em}+\,\frac{b_3}{3!}\,\delta^3(\boldsymbol{x}) + \gamma_3^{\times}\,\delta(\boldsymbol{x})\,{\cal G}_2(\boldsymbol{x}|\Phi_v) + \gamma_3^-\,\underbrace{\Delta_3{\cal G}(\boldsymbol{x}|\Phi,\Phi_v)}_{=\,{\cal G}_2(\Phi_v)-{\cal G}_2(\Phi)} + \gamma_3\,{\cal G}_3(\boldsymbol{x}|\Phi_v)} \\
  &\fragment{2}{\hspace{0.23em}+\,\frac{b_4}{4!}\,\delta^4(\boldsymbol{x}) + \gamma_4^{(1)}\,\delta^2(\boldsymbol{x})\,{\cal G}_2(\boldsymbol{x}|\Phi_v) + \gamma_4^{(2)}\,\delta(\boldsymbol{x})\,\Delta_3{\cal G}(\boldsymbol{x}|\Phi,\Phi_v) + \ldots \, \text{(3 terms)} }
  \end{align}
  $$
  `
</p>

<hr style="height:2em; visibility:hidden;"/>

<div style="font-size:150%"> <!-- {_style="text-align: center"}-->
  <span style="color:#f0f1eb"> <b> NONE of these parameters are measurable!</b> </span>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
# The Happy End <!-- {_style="text-align: center"}-->

<hr style="height:1em; visibility:hidden;"/>

<p style="border:2px solid black; padding:10px; border-radius:8px">
  `
  $$
  \begin{align}
  \delta_g(\boldsymbol{x}) &= \color{red}b_1\color{black}\,\delta(\boldsymbol{x}) \\
  &+\frac{\color{red}b_2\color{black}}{2}\,\delta^2(\boldsymbol{x}) + \color{red}\gamma_2\color{black}\,{\cal G}_2(\boldsymbol{x}|\Phi_v) \\
  &+\frac{\color{red}b_3\color{black}}{3!}\,\delta^3(\boldsymbol{x}) + \color{red}\gamma_3^{\times}\color{black}\,\delta(\boldsymbol{x})\,{\cal G}_2(\boldsymbol{x}|\Phi_v) + \color{red}\gamma_3^-\color{black}\,\underbrace{\Delta_3{\cal G}(\boldsymbol{x}|\Phi,\Phi_v)}_{=\,{\cal G}_2(\Phi_v)-{\cal G}_2(\Phi)} + \color{red}\gamma_3\color{black}\,{\cal G}_3(\boldsymbol{x}|\Phi_v) \\
  &+\frac{\color{red}b_4\color{black}}{4!}\,\delta^4(\boldsymbol{x}) + \color{red}\gamma_4^{(1)}\color{black}\,\delta^2(\boldsymbol{x})\,{\cal G}_2(\boldsymbol{x}|\Phi_v) + \color{red}\gamma_4^{(2)}\color{black}\,\delta(\boldsymbol{x})\,\Delta_3{\cal G}(\boldsymbol{x}|\Phi,\Phi_v) + \ldots \, \text{(3 terms)}
  \end{align}
  $$
  `
</p>

<hr style="height:2em; visibility:hidden;"/>

<div style="font-size:150%"> <!-- {_style="text-align: center"}-->
  <span style="color:red"> <b> NONE of these parameters are measurable!</b> </span>
</div>

<div style="position: absolute; top: 1.65em; left: 11.5em; width: 350px; height: 200px;">
  <hr color="red" width="200em" size="7px">
</div>

---

<!-- {_style="text-align: center"}-->
# The Need for Renormalization

### Example: 1-Loop Galaxy Power Spectrum

<div style="font-size:150%">
  `
  $$
  \rightarrow \hspace{0.1em} P_g(k) = \underbrace{\Big(b_1^2 + \color{red}b_1\,b_3\,\sigma^2_{\Lambda}\color{black}\Big)}_{\substack{\sigma^2_{\Lambda}\,\sim\,\int^{\Lambda}_0 \text{d}q\,q^2\,P_L(q) \\ \hspace{-2em}\sim\,\log{\Lambda}}}\,P_L(k) + \ldots
  $$
  `
</div>

<div style="position: absolute; top: 15em; left: 7.5em; width: 500px; height: 200px;">
  `$\Lambda \equiv $` <b>arbitrary</b> cut-off scale, e.g. where you think PT is breaking down ...
</div>

<hr style="height:4em; visibility:hidden;"/>

<p class="fragment" data-fragment-index="1">
  <b>Solution:</b> define <span style="color:red">renormalized bias parameters</span>
  <p class="fragment" data-fragment-index="1">
    `
    $$
    \rightarrow \hspace{0.1em} b_1^R = b_1 + \frac{b_3}{2}\,\sigma_{\Lambda}^2 + \text{contributions from higher orders}
    $$
    `
  </p>
</p>

---

<!-- {_style="text-align: center"}-->
# The Gamma Expansion

<div style="border:5px solid #f5d328; padding:10px; border-radius:8px">
  <b>New idea: </b> Expand `$\delta_g$` in terms of (generalized) Hermite polynomials
</div>
[<span style="color:DarkTurquoise"> Szalay '88, Matsubara '95, Bernardeau+ '08 </span>]

<hr style="height:0.1em; visibility:hidden;"/>

<div class="row">
  <div class="column">
    <p style="font-size:85%">
      `
      $$
      \begin{align}
      \delta_g(\boldsymbol{k}) &= \Gamma_g^{(1)}(\boldsymbol{k})\,{\cal H}_1(\boldsymbol{k}) \\
      &\fragment{1}{\,+\, \Gamma_g^{(2)}(\boldsymbol{k}_1,\boldsymbol{k}_2)\, * \,{\cal H}_2(\boldsymbol{k}_1,\boldsymbol{k}_2)} \\
      &\fragment{2}{\,+\, \Gamma_g^{(3)}(\boldsymbol{k}_1,\boldsymbol{k}_2,\boldsymbol{k}_3)\, * \,{\cal H}_3(\boldsymbol{k}_1,\boldsymbol{k}_2,\boldsymbol{k}_3)} \\ &\fragment{2}{\,+\, \ldots}
      \end{align}
      $$
      `
    </p>
  </div>
  <div class="column">
    <div style="border-left:solid black">
    <p style="font-size:85%">
      `
      $$
      \begin{align}
      \hspace{0.2em}{\cal H}_1(\boldsymbol{k}) &\equiv \delta_L(\boldsymbol{k}) \\[0.5em]
      \fragment{1}{ {\cal H}_2(\boldsymbol{k}_1,\boldsymbol{k}_2)} &\fragment{1}{\,\equiv \delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2) - \langle\delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2)\rangle} \\[0.5em]
      \fragment{2}{ {\cal H}_3(\boldsymbol{k}_1,\boldsymbol{k}_2,\boldsymbol{k}_3)} &\fragment{2}{\,\equiv \delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2)\delta_L(\boldsymbol{k}_3)} \\ &\fragment{2}{\,-\, \langle\delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2)\rangle\,\delta_L(\boldsymbol{k}_3) - \text{cyc.}}
      \end{align}
      $$
      `
    </p>
    </div>
  </div>
</div>

<!-- {_style="text-align: left"}-->
<span class="fragment" data-fragment-index="1"></span>
<span class="fragment" data-fragment-index="2"></span>
<span class="fragment" data-fragment-index="3"></span>
<p class="fragment" data-fragment-index="4">
  Because of <b>orthogonality</b> of Hermite polynomials:
  <p class="fragment" data-fragment-index="4">
    `
    $$
    P_g(k) = \underbrace{\Big[\Gamma_g^{(1)}(\boldsymbol{k})\Big]^2}\,P_L(k) + 2 \int \text{d}^3q \underbrace{\Big[\Gamma_g^{(2)}(\boldsymbol{q},\boldsymbol{k}-\boldsymbol{q})\Big]^2}\,P_L(q)\,P_L(|\boldsymbol{k}-\boldsymbol{q}|)
    $$
    `
  </p>
  <div style="position: absolute; top: 22.7em; left: -0.4em; width: 500px; height: 200px;" class="fragment" data-fragment-index="4">
    <span style="color:red">renormalized!</span>
  </div>
  <div style="position: absolute; top: 22.7em; left: 13em; width: 500px; height: 200px;" class="fragment" data-fragment-index="4">
    <span style="color:red">renormalized!</span>
  </div>
</p>

---

<!-- .slide: data-transition="slide-in fade-out"-->
# I'm a (Multipoint) Propagator <!-- {_style="text-align: center"}-->

<p>
  `
  $$
  \color{red}(2\pi)^3\,\Gamma_g^{(n)}\,\delta_D(\boldsymbol{k}-\boldsymbol{k}_1 - \ldots - \boldsymbol{k}_n) = \Bigg<\frac{\partial^n\delta_g(\boldsymbol{k})}{\partial\delta_L(\boldsymbol{k}_1)\,\cdots\,\partial\delta_L(\boldsymbol{k}_n)}\Bigg>
  $$
  `
</p>

<hr>

E.g. first order Gamma: <!-- {_class="fragment" data-fragment-index="1"}-->

<p class="fragment" data-fragment-index="1">
  `
  $$
  \begin{align}
  \Gamma_g^{(1)}(\boldsymbol{k}) &= \underbrace{b_1 + \Bigg[\frac{34}{21}b_2 + \frac{1}{2}b_3 - \frac{4}{3}\gamma_3^{\times}\Bigg]\,\sigma_{\Lambda}^2}_{\large \rightarrow \hspace{0.5em} b_1^R}
  - \frac{8}{7}\gamma_3^{-} \int \text{d}^3q\,K(\boldsymbol{q},\boldsymbol{k}-\boldsymbol{q})\,K(\boldsymbol{q},\boldsymbol{k})\,P_L(q)
  \end{align}
  $$
  `
</p>

<p class="fragment" data-fragment-index="2">
  Unfortunately, <b>troublemaker</b> in second order Gamma:
  `
  $$
  \Gamma_g^{(2)}(\boldsymbol{k}_1,\boldsymbol{k}_2) \supset \underbrace{\int \text{d}^3q\,F_2(\boldsymbol{k}_1,\boldsymbol{q})\,F_2(\boldsymbol{k}_2,-\boldsymbol{q})\,P_L(q)}
  $$
  `
</p>

<div style="text-align:center; position: absolute; top: 22.5em; left: 8em; width: 800px; height: 200px;" class="fragment" data-fragment-index="2">
  `$\rightarrow \hspace{0.5em}$` contains terms dependent <b>and</b> independent of `$\Lambda$` <br>
  <span style="color:red"> HOW TO SEPARATE? </span>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
# I'm a (Multipoint) Propagator <!-- {_style="text-align: center"}-->

<p>
  `
  $$
  \color{red}(2\pi)^3\,\Gamma_g^{(n)}\,\delta_D(\boldsymbol{k}-\boldsymbol{k}_1 - \ldots - \boldsymbol{k}_n) = \Bigg<\frac{\partial^n\delta_g(\boldsymbol{k})}{\partial\delta_L(\boldsymbol{k}_1)\,\cdots\,\partial\delta_L(\boldsymbol{k}_n)}\Bigg>
  $$
  `
</p>

<hr>

<img src="/presentations/spaghetti.png", style="position:relative; top:-35px; left:0em; height:450px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 10em; left: 14em; width: 300px; height: 200px;">
  `$\displaystyle \Gamma_g^{(n)}(\boldsymbol{k}_1,\ldots\,;\tau)$`
</div>

<div style="position: absolute; top: 10em; left: 10.3em; width: 500px; height: 500px;">
<svg width="500" height="800">

    <defs>
        <marker id="arrow" markerWidth="13" markerHeight="13" refx="2" refy="6" orient="auto">
            <path d="M2,2 L2,11 L10,6 L2,2" style="fill:red;" />
        </marker>
    </defs>

    <path d="M-100,450 L150,100"
          style="stroke:red; stroke-width: 2.25px; fill: none;
                 marker-end: url(#arrow);"
    />

</svg>  
</div>

<div style="position: absolute; top: 24em; left: 6.3em; width: 300px; height: 200px;">
  `$\displaystyle \Gamma_g^{(n)}(\boldsymbol{k}_1,\ldots\,;\tau=0)$`
</div>

<div style="position: absolute; top: 15em; left: 17.5em; width: 500px; height: 100px;">
  <div style="border:5px solid #f5d328; padding:10px; border-radius:8px;">
    Compute `$\Gamma_g^{(n)}({\boldsymbol{k}_1,\ldots,\boldsymbol{k}_n})$` and identify renormalized bias parameters on <b>initial</b> time slice, then <b>evolve</b>!
  </div>
  <hr style="height:0.1em; visibility:hidden;"/>
  <div style="text-align:center">
    (can be automated symbolically in <code>mathematica</code>)
  </div>
</div>

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>The 1-loop Bispectrum <br> in Action</b> </span>

---

<!-- {_style="text-align: center"}-->
# The 1-loop Galaxy Bispectrum

<hr style="height:2.5em; visibility:hidden;"/>

<img src="/presentations/diagrams.png", style="position:relative; top:-35px; left:0em; width:1000px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 18em; left: 3.3em; width: 300px; height: 200px;" class="fragment" data-fragment-index="1">
  `
  $$
  \sim \Gamma_g^{(2)}\,\Gamma_g^{(1)}\,\Gamma_g^{(1)}\,P_L^2
  $$
  `
</div>

<div style="position: absolute; top: 18em; left: 13.8em; width: 300px; height: 200px;" class="fragment" data-fragment-index="1">
  `
  $$
  \sim \int \Big[\Gamma_g^{(2)}\Big]^3\,P_L^3
  $$
  `
</div>

<div style="position: absolute; top: 18em; left: 24.3em; width: 300px; height: 200px;" class="fragment" data-fragment-index="1">
  `
  $$
  \sim \int \Gamma_g^{(3)}\,\Gamma_g^{(2)}\,\Gamma_g^{(1)}\,P_L^3
  $$
  `
</div>

---

<!-- {_style="text-align: center"}-->
# An Inventory of the Model

<p>
  `
  $$
  \begin{align}
  B_g(k_1,k_2,k_3) &= \Big(b_1^R\Big)^3\,B_{\delta}(k_1,k_2,k_3) \\[0.2em] &\fragment{1}{\,+\, \Big(b_1^R\Big)^2\,\Big[b_2^R\,P_L(k_1)\,P_L(k_2) + 2\gamma_2^R\,K(\boldsymbol{k}_1,\boldsymbol{k}_2)\,P_L(k_1)\,P_L(k_2) + \text{cyc.}\Big]} \\[0.2em]
  &\fragment{2}{\,+\, \text{37 bias loop integrals}} \\[0.2em]
  &\fragment{3}{\,+\, \epsilon_0\,C_1 + \eta_0\,C_2\,\Big[P_L(k_1) + P_L(k_2) + P_L(k_3)\Big]}
  \end{align}
  $$
  `
</p>

<hr style="height:1em; visibility:hidden;"/>

<span class="fragment" data-fragment-index="1"></span>
<span class="fragment" data-fragment-index="2"></span>
<span class="fragment" data-fragment-index="3"></span>
<span class="fragment" data-fragment-index="4"></span>
<div class="fragment" data-fragment-index="5">
  <hr>
  <hr style="height:1em; visibility:hidden;"/>
  <ul>
    <li> 7 <b>free</b> bias parameters </li>
    <li> assume <b>local Lagrangian bias</b> for fourth order biases </li>
    <li> two <b>noise parameters</b> for `$B_g$`, one for `$P_g$`
  </ul>
</div>
<p style="color:red" class="fragment" data-fragment-index="6">
  `$\Rightarrow \hspace{0.3em}$` 10 free parameters for joint power spectrum and bispectrum analysis
</p>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# Data. Finally!

<img src="/presentations/bspec_BOSSlike_1.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# Data. Finally!

<img src="/presentations/bspec_BOSSlike_2.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="slide-in none-out"-->
<!-- {_style="text-align: center"}-->
<img src="/presentations/contours_Bggg_bincorr2_kmax0p1.png", style="position:relative; top:-35px; width:700px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 5em; left: 20em; width: 300px; height: 600px;">
  <h2>Constraints from Galaxy Bispectrum</h2>
</div>

---

<!-- .slide: data-transition="fade-in none-out"-->
<!-- {_style="text-align: center"}-->
<img src="/presentations/contours_Bggg_bincorr2_kmax0p15.png", style="position:relative; top:-35px; width:700px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 5em; left: 20em; width: 300px; height: 600px;">
  <h2>Constraints from Galaxy Bispectrum</h2>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
<img src="/presentations/contours_Bggg_bincorr2_kmax0p2.png", style="position:relative; top:-35px; width:700px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 5em; left: 20em; width: 300px; height: 600px;">
  <h2>Constraints from Galaxy Bispectrum</h2>
</div>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# Combined Constraints


<img src="/presentations/contours_pk+Bggg_bincorr2_kmax0p1.png", style="position:relative; top:-35px; width:600px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="fade-in fade-out"-->
<!-- {_style="text-align: center"}-->
# Combined Constraints


<img src="/presentations/contours_pk+Bggg_bincorr2_kmax0p15.png", style="position:relative; top:-35px; width:600px; background:none; border:none; box-shadow:none;"/>

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="fade-in slide-out"-->
# Combined Constraints

<img src="/presentations/contours_pk+Bggg_bincorr2_kmax0p20.png", style="position:relative; top:-35px; width:600px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 11em; left: 18em; width: 300px; height: 600px;" class="fragment">
  <h2>It works!</h2>
</div>


---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Summary and Outlook</b> </span>

---

<!-- {_style="text-align: center"}-->
# Conclusions

<hr style="height:1em; visibility:hidden;"/>
<ul>
  <li>
    bispectrum contains a lot of extra information, <b>inaccessible</b> to <br> the power spectrum <br>
    `$\hspace{0.5em} \rightarrow \hspace{0.3em}$` extraction requires <b>reliable</b> model on small scales
  </li>
  <hr style="height:0.5em; visibility:hidden;"/>
  <li>
    galaxy bias can be incorporated into perturbative schemes <br> `$\hspace{0.5em} \rightarrow \hspace{0.3em}$`
    <b>multipoint propagators</b> greatly facilitate computation <br> <span style="color:#f0f1eb">`$\hspace{0.5em} \rightarrow \hspace{0.3em}$`</span>  of renormalized bias parameters
  </li>
  <hr style="height:0.5em; visibility:hidden;"/>
  <li>
    inclusion of bias loops and correct treatment of noise <br> makes $P_g$ and $B_g$ <b>CONSISTENT</b>
  </li>
</ul>


---

<!-- {_style="text-align: center"}-->
# Some Future Directions

<hr style="height:1em; visibility:hidden;"/>
<ul>
  <li>
    What about <b>spatial non-locality</b>? `$\hspace{0.5em} \rightarrow \hspace{0.3em}$` higher derivatives:
    <p>
      `
      $$
      \Rightarrow \hspace{0.5em} 1) \hspace{0.2em} \nabla^2\delta^{(2)}\,, \hspace{1em} 2) \hspace{0.2em} \nabla^2{\cal G}_2\,, \hspace{1em} 3) \hspace{0.2em} \nabla^2\Big(\delta^{(1)}\Big)^2\,, \hspace{1em} 4) \hspace{0.2em} \Big(\boldsymbol{\nabla}\delta^{(1)}\Big)^2
      $$
      `
    </p>
    Also need to include EFT and additional noise parameters: <br> 8 new <b>free parameters in total!</b>
  </li>
  <hr style="height:0.5em; visibility:hidden;"/>
  <li>
    Which loop corrections are actually <b>necessary</b>?
  </li>
  <hr style="height:0.5em; visibility:hidden;"/>
  <li>
    Can we <b>fix a subset</b> of the bias parameters? <br>
    `$\hspace{0.5em} \rightarrow \hspace{0.3em}$` local Lagrangian bias <br>
    `$\hspace{0.5em} \rightarrow \hspace{0.3em}$` universal bias relations
  </li>  
</ul>

--

<!-- {_style="text-align: center"}-->
# Some Future Directions

<img src="/presentations/contours_Bggg_looptree_kmax0p2.png", style="position:relative; top:-35px; width:600px; background:none; border:none; box-shadow:none;"/>




</script>
</section>


 <!-- &emsp; -->
