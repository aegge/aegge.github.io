---
layout: slide
title: Probing Large-Scale Structure Beyond the Power Spectrum
description:
theme: serif
transition: slide
author_profile: false
categories: presentations
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
</style>

<script>
	var link = document.createElement( 'link' );
	link.rel = 'stylesheet';
	link.type = 'text/css';
	link.href = window.location.search.match( /print-pdf/gi ) ? 'css/print/pdf.css' : 'css/print/paper.css';
	document.getElementsByTagName( 'head' )[0].appendChild( link );
</script>

<section data-markdown data-separator="^\n---\n$"
         data-separator-vertical="^\n--\n$"
         data-element-attributes="{_\s*?([^}]+?)}"
         data-separator-notes="^Note:"             >
<script type="text/template">
<!-- {_style="text-align: center"}-->
<br>
# Probing Large-Scale Structure Beyond the Power Spectrum

<br><br>

### Alexander Eggemeier
<img src="/presentations/sussex_logo.png", style="width:125px; background:none; border:none; box-shadow:none;"/>

with Joyce Byun, Donough Regan, David Seery & Robert E. Smith

---

<!-- {_style="text-align: center"}-->
# Clustering Measures

<br>
**Two-point statistics** $\quad \quad \quad \quad \quad \quad$ **Three-point statistics**
<img src="/presentations/millennium_arrows.png", style="border:none; background:none; box-shadow:none; width:2000px; height:200px"/>
<p style="margin-top: -20px">
</p>

`$\text{density field: } \delta(\boldsymbol{x}) = \frac{n(\boldsymbol{x})-\bar{n}}{\bar{n}}$`

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


<div class="fragment" data-fragment-index="1">
`
$$
\hspace{-3em}\text{If $\delta$ is Gaussian} \, \rightarrow \, {\cal P}(\delta_1,\dots,\delta_N) \propto \exp{\left[-\frac{1}{2}(\delta_1,\dots,\delta_N) C^{-1}\left(\begin{array}{c} \delta_1 \\ \vdots \\ \delta_N \end{array}\right)\right]},\;
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
  \delta_g(\boldsymbol{x}) = b_1\,\delta(\boldsymbol{x}) + b_2\,\color{red}\delta(\boldsymbol{x})^2\color{black} + \gamma_2\, \color{red}{\cal G}_2(\boldsymbol{x})\color{black} + \ldots
  $$
  `
</div>

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="fade-in slide-out"-->
# Why Go Beyond $P(k)$?

### I) The observed density field is <span style="color:red">non-Gaussian</span>


<div>
`
$$
\hspace{-3em}\text{If $\delta$ is Gaussian} \, \rightarrow \, {\cal P}(\delta_1,\dots,\delta_N) \propto \exp{\left[-\frac{1}{2}(\delta_1,\dots,\delta_N) C^{-1}\left(\begin{array}{c} \delta_1 \\ \vdots \\ \delta_N \end{array}\right)\right]},\;
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
  \delta_g(\boldsymbol{x}) = b_1\,\delta(\boldsymbol{x}) + b_2\,\color{red}\delta(\boldsymbol{x})^2\color{black} + \gamma_2\, \color{red}{\cal G}_2(\boldsymbol{x})\color{black} + \ldots
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
\text{Power spectrum: } \quad &P_{\text{gg}} \sim b_1^2\,\sigma_8^2 \\[1em]
\text{Bispectrum: } \quad &B_{\text{ggg}} \sim \left[b_1^3\,\sigma_8^4\right] + \sim \left[b_1^2\,b_2\,\sigma_8^4\right]
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
\hspace{-8em}\text{Power spectrum: } \quad &P_{\text{gg}} \sim f^2\,\sigma_8^2 \\[1em]
\text{Bispectrum: } \quad &B_{\text{ggg}} \sim \left[f^3 + \ldots \right]\sigma_8^4
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
  <li style="border:3px; border-style:solid; border-color:red; padding: 5px; padding-left: 20px">
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

<!-- {_style="text-align: center"}-->
# Alternative Bispectrum Estimators

<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>

1. The Line Correlation Function

2. The Integrated Bispectrum

3. The Modal Bispectrum

---

# The Line Correlation Function <!-- {_style="text-align: center"}-->

Smoothed _phase field_: `$\displaystyle \;\epsilon_r(\boldsymbol{x}) = \int \frac{\text{d}^3k}{(2\pi)^3} \epsilon(\boldsymbol{k})
\text{e}^{i \boldsymbol{k} \cdot \boldsymbol{x}}\,W(k|r)\,, \quad \epsilon(\boldsymbol{k}) \equiv \frac{\delta(\boldsymbol{k})}{|\delta(\boldsymbol{k})|}$`

<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>

<div>
<img src="/presentations/lcf.png", style="background:none; border:none; box-shadow:none; float:right;"/>

<p>
  <hr style="height:1em; visibility:hidden;"/>
</p>

Define LCF as three-point phase correlator: [<span style="color:DarkTurquoise">Obreschkow+ '12</span>]

`
$$
\hspace{-4em}\fcolorbox{yellow}{}{$\ell(r) \equiv V^3\,\left(\frac{r^3}{V}\right)^{3/2} \langle \epsilon_r(\boldsymbol{x})\,\epsilon_r(\boldsymbol{x}+\boldsymbol{r})\,\epsilon_r(\boldsymbol{x}-\boldsymbol{r})\rangle$}
$$
`
<p>
  <hr style="height:1em; visibility:hidden;"/>
</p>

`
$$
\hspace{2em}\rightarrow \hspace{1em}\sim \iint\limits_{\substack{|\boldsymbol{k}_1|,|\boldsymbol{k}_2|,\\ |\boldsymbol{k}_1+\boldsymbol{k}_2|\leq 2\pi/r }} \text{d}^3k_1\,\text{d}^3k_2\,\frac{B(\boldsymbol{k}_1,\boldsymbol{k}_2,-\boldsymbol{k}_1-\boldsymbol{k}_2)}{\sqrt{P(k_1)\,P(k_2)\,P(|\boldsymbol{k}_1+\boldsymbol{k}_2|)}}\,j_0(|\boldsymbol{k}_2-\boldsymbol{k}_1|r)\,
$$
`
</div>
$\hspace{12em}$[<span style="color:DarkTurquoise">Wolstenhulme+ '15, <b>AE</b> & Smith '16</span>]

---

<!-- {_style="text-align: center"}-->
# The Integrated Bispectrum

### Power spectrum response to long wavelength modulation:

<img src="/presentations/iB.png", style="background:none; border:none; box-shadow:none; width:378px" align="left" hspace="20" />
<p class="fragment" data-fragment-index="1">
<img src="/presentations/Ppos.png", style="background:none; border:none; box-shadow:none; width:486px"/>
</p>

<div style="position: absolute; top: 16em; left: 3px; width: 240px; height: 150px;">
[<span style="color:DarkTurquoise">Chiang+ '14/15</span>]
</div>

Slice the survey volume up into $N_s$ _subcubes_: `$\displaystyle \delta(\boldsymbol{k,\boldsymbol{r}_L}) = \int \text{d}^3r\,\delta(\boldsymbol{r})\,W_L(\boldsymbol{r}-\boldsymbol{r}_L)\,\text{e}^{i\boldsymbol{k}\cdot\boldsymbol{x}}$`

<p class="fragment" data-fragment-index="2">
`
$$
\hspace{-2em}\fcolorbox{yellow}{}{$iB(k) \equiv \langle \overline{\delta}(\boldsymbol{r}_L)\,P(\boldsymbol{k},\boldsymbol{r}_L)\rangle$} \sim \int\limits_{\boldsymbol{q}_1,\boldsymbol{q}_2} \underbrace{B(\boldsymbol{k}-\boldsymbol{q}_1,-\boldsymbol{k}+\boldsymbol{q}_1+\boldsymbol{q}_2,-\boldsymbol{q}_2)} W_L(\boldsymbol{q}_1)\,W_L(\boldsymbol{q}_2)\,W_L(-\boldsymbol{q}_1-\boldsymbol{q}_2) \\[-3em]
\scriptsize \hspace{4em}\xrightarrow{k\,\gg\,1/L}\;B(\boldsymbol{k},-\boldsymbol{k},-\boldsymbol{q}_2) \quad \color{red} \text{squeezed limit!}
$$
`
</p>

Note:
- correlation of small scales to large scales
- for Gaussian field modes are not correlated (as described earlier), but non-Gaussian fields will have this effect as demonstrated by     
  measurements
- dominant contribution to integral is coming from squeezed configurations as window functions fall of on the scale $1/L$

---

<!-- {_style="text-align: center"}-->
# The Modal Bispectrum

### Decompose the bispectrum into set of _triangle shapes_:

<div style="position: absolute; top: 6em; left: 11em; width: 400px; height: 150px;">
[<span style="color:DarkTurquoise">Fergusson+ '10, Regan+ '11</span>]
</div>

<img src="/presentations/decomp.png", style="background:none; border:none; box-shadow:none; width:1000px;"/>

<p class="fragment">
`
$$
\fcolorbox{yellow}{}{$B_{\text{modal}}(k_1,k_2,k_3) \equiv \frac{1}{w(k_1,k_2,k_3)} \sum_{n=0}^{n_{\text{max}}-1} \beta_n\,{\cal Q}_n(k_1,k_2,k_3)$} \\
\hspace{7.5em} \uparrow \hspace{8.5em} \uparrow \\
\hspace{9em} \text{weight} \hspace{4.5em} \text{basis functions}
$$
`
</p>

<p class="fragment">
`
$$
\langle w\,B_{\text{modal}} \,,\, {\cal Q}_m\rangle = \sum_{n=0}^{n_{\text{max}}-1} \beta_n\,\underbrace{\langle {\cal Q}_n \,,\, {\cal Q}_m\rangle}_{\textstyle \equiv \gamma_{nm}} \quad \Rightarrow \quad \beta_n = \sum_{m=0}^{n_{\text{max}}-1} \langle w\,B_{\text{modal}} \,,\, {\cal Q}_m\rangle \gamma_{mn}^{-1}
$$
`
</p>

--

# The Modal Bispectrum <!-- {_style="text-align: center"}-->

### How to do this in practice? <!-- {_style="text-align: center"}-->

1. Choose inner product:
    `
    $$
    \color{#f0f1eb}.\\[-0.5em]\color{black}\langle f \,,\, g\rangle \equiv \int_{ {\cal V}_T} \text{d}k_1\,\text{d}k_2\,\text{d}k_3\, f(k_1,k_2,k_3)\,g(k_1,k_2,k_3)\,, \quad \color{red} {\cal V}_T = \begin{array}{c} \text{allowed triangle} \\ \text{configurations} \end{array} \\[2em]
    \hspace{-2em}\text{for} \; w(k_1,k_2,k_3) \equiv \sqrt{\frac{k_1\,k_2\,k_3}{P(k_1)P(k_2)P(k_3)}} \; \text{and }\textit{Gaussian }\text{errors} \; \Rightarrow \langle{\cal Q}_n \,,\, {\cal Q}_n \rangle = 6\,\left(\frac{ {\cal S}}{ {\cal N}}\right)^2_{ {\cal Q}_n} \\[2em]
    \beta_n \sim \sum_m \gamma_{mn}^{-1} \int_{ {\cal V}_T} \text{d}k_1\,\text{d}k_2\,\text{d}k_3\, \sqrt{k_1\,k_2\,k_3}\color{red}\underbrace{B_{\epsilon}(k_1,k_2,k_3)}_{\textstyle \text{phase bispectrum}}\color{black}\,{\cal Q}_m(k_1,k_2,k_3)
    $$
    `

2. Choose basis functions:
   $\; \rightarrow \;$ triples of 1d polynomials, orthonormal on ${\cal V}_T$
    `
    $$
    \color{#f0f1eb}.\\[-0.5em]\color{black}{\cal Q}_n(k_1,k_2,k_3) = q_{n_1}(k_1)\,q_{n_2}(k_2)\,q_{n_3}(k_3)
    $$
    `

Note:
- after choosing the weight to be w = ..., the inner product has a simple interpretation: as it gives the signal to
  noise of measuring a single Qn mode, it can be regarded as an integral over Fourier configurations, each of which are
  weighted according to their individual signal-to-noise

--

<!-- {_style="text-align: center"}-->
# The Modal Bispectrum

<img src="/presentations/bspecrecon.png", style="background:none; border:none; box-shadow:none; width:1000px;"/>

from <tt>ZBOX2</tt> N-body simulations: DM only, $V = 3.375\,(\text{Gpc}/h)^3$, $N_p = 750^3$
<span style="color:DarkTurquoise">Byun, **AE**, Regan+ 2017</span>

--

<!-- {_style="text-align: center"}-->
# The Modal Bispectrum

<img src="/presentations/bspec_modes.png", style="background:none; border:none; box-shadow:none; width:1000px;"/>

from <tt>ZBOX2</tt> N-body simulations: DM only, $V = 3.375\,(\text{Gpc}/h)^3$, $N_p = 750^3$
<span style="color:DarkTurquoise">Byun, **AE**, Regan+ 2017</span>

---

# Our Questions <!-- {_style="text-align: center"}-->

- <p> Can the alternative measures compete with the bispectrum? </p> <!-- {_style="font-size: 30px"}-->
  <p> $\hspace{2em}\rightarrow$ is it possible to <span style="color:red"><em>compress information</em></span>? </p>
<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>
- <p> How important are <span style="color:red"><em>non-Gaussian covariance matrices</em></span> for the various estimators? </p> <!-- {_style="font-size: 30px"}-->
<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>
- <p> What is the impact of <span style="color:red"><em>cross-covariance</em></span> with the power spectrum? </p> <!-- {_style="font-size: 30px"}-->

---

<!-- {_style="text-align: center"}-->
# Fisher Analysis

set of parameters: `$\displaystyle \quad\boldsymbol{\theta} = \{\Omega_m,\, \Omega_b,\, w_0,\, w_a,\, \sigma_8,\, n_s,\, h,\, \underbrace{b_1,\, b_2}\} \\ \hspace{14em} \color{blue}\text{galaxy bias}$`
<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>
observables: `$\displaystyle \quad \boldsymbol{d} = P + \{B\,,\,\ell\,,\,ib\,,\,\beta\}\quad$` with `$\displaystyle \quad k_{\text{max}} = 0.3\,h\,\text{Mpc}^{-1}$`
<p>
  <hr style="height:0.2em; visibility:hidden;"/>
</p>
`
$$
\Rightarrow \quad \fcolorbox{red}{}{$F_{ij} = \frac{\partial \boldsymbol{d}}{\partial \theta_i} \cdot C^{-1}_d \cdot \frac{\partial \boldsymbol{d}}{\partial \theta_j}$} \quad (\text{at redshift} \quad z=0.0,\,0.5,\,1.0)
$$
`
<p>
`
$
\hspace{9em}\style{display: inline-block; transform:rotate(0.5turn);}{\Large \Lsh} \quad \text{estimate} \; \frac{\partial \boldsymbol{d}}{\partial \theta_i} \; \text{and} \; C_d^{-1} \; \text{from N-body simulations}
$
`
</p>

<br>

simplifications: no survey geometry, no redshift space distortions, no systematic effects, $\ldots$

---

<!-- {_style="text-align: center"}-->
# Non-Gaussian covariance matrix

<img src="/presentations/cov.png", style="background:none; border:none; box-shadow:none; width:670px; float:right"/>

<div style="position: absolute; top: 8em; left: 0.em; width: 270px; height: 150px;">
<ul>
<li> estimated from $200$ N-body simulations </li> <br>
<li> far from <em>diagonal</em> Gaussian covariance matrix </li> <br>
<li> bins on smaller scales or with common k's are more correlated </li> <br>
</ul>
$\hspace{-2em}$[<span style="color:DarkTurquoise">Byun, **AE**, Regan+ '17</span>]
</div>


---

<!-- {_style="text-align: center"}-->

<img src="/presentations/fisher2.png", style="background:none; border:none; box-shadow:none; width:670px; float:right"/>

<div style="position: absolute; top: 0.5em; left: 0.em; width: 270px; height: 150px;">
<h1>Fisher Forecasts</h1>
<ul>
<li> Number of bins: <br> $B$ (95), $\;\beta$ (50), <br> $\ell$ (30), $\;ib$ (30) </li> <br>
<li> $P+B$ constraints on $\sigma_8$, $b_1$ & $b_2$ are $3$-$5$ times stronger than from $P$ alone </li> <br>
<li> $\beta$ has <b>identical constraints</b> as $B$ with half the number of bins or less </li> <br>
</ul>
$\hspace{-2em}$[<span style="color:DarkTurquoise">Byun, **AE**, Regan+ '17</span>]
</div>

--

<!-- {_style="text-align: center"}-->
<img src="/presentations/fisher_shotnoise.png", style="background:none; border:none; box-shadow:none; width:670px;"/>

---

<!-- {_style="text-align: center"}-->
# Gaussian vs. Non-Gaussian

Plotting the ratio: `$\displaystyle \frac{\sigma_{\text{NG}}}{\sigma_{\text{G}}}-1$`

<img src="/presentations/nGvsG.png", style="background:none; border:none; box-shadow:none; width:1200px;"/>

$\rightarrow \quad$ Gaussian covariances **underestimate** forecasted uncertainties by <span style="color:red">factor up to $4$</span> for bispectrum, somewhat less for other probes

[<span style="color:DarkTurquoise">Byun, **AE**, Regan+ '17</span>]

---

<!-- {_style="text-align: center"}-->
# Effect of Cross-Covariance

Plotting the ratio: `$\displaystyle \frac{\sigma_{\text{NG-no-}C_{\times}}}{\sigma_{\text{NG-with-}C_{\times}}}-1$`

<img src="/presentations/fisher_covx.png", style="background:none; border:none; box-shadow:none; width:1200px;"/>

$\rightarrow \quad$ cross-covariance can **enhance** information gain from three-point statistics

[<span style="color:DarkTurquoise">Byun, **AE**, Regan+ '17</span>]

--

<!-- {_style="text-align: center"}-->
# Signal-to-Noise

<img src="/presentations/SN.png", style="background:none; border:none; box-shadow:none; width:650px;"/>

</script>
</section>


 <!-- &emsp; -->
