---
layout: slide
title: The One-Loop Galaxy Bispectrum (IAP)
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
<!-- .slide: data-transition="slide-in fade-out"-->
# Why Go Beyond $P(k)$?

<p style="border:3px; border-style:solid; border-color:red; padding: 10px; border-radius:8px">
  `
  $
  \text{Bispectrum: } \quad \langle \delta(\boldsymbol{k}_1)\,\delta(\boldsymbol{k}_2)\,\delta(\boldsymbol{k}_3)\rangle = (2\pi)^3 B(k_1,k_2,k_3)\,\delta_D(\boldsymbol{k}_1+\boldsymbol{k}_2+\boldsymbol{k}_3)
  $
  `
</p>

<div class="fragment">
  <img src="/presentations/pdf01.png", style="width:300px; background:none; border:none; box-shadow:none; float:left"/>

  <div style="position: absolute; top: 17.3em; left: 0.0em; width: 300px; height: 50px;">
    <font size="-1">
      [<span style="color:DarkTurquoise">Credit: M. Schmittfull</span>]
    </font>
  </div>
  <div style="position: absolute; top: 19em; left: 0.0em; width: 300px; height: 50px;">
    The observed density field is non-Gaussian
</div>

Note:
- reason number 1: density is non-Gaussian (if Gaussian all info in P)
- reason number 2: bispectrum has different parameter dependencies
- reason number 3: cosmic variance limit

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="fade-in slide-out"-->
# Why Go Beyond $P(k)$?

<p style="border:3px; border-style:solid; border-color:red; padding: 10px; border-radius:8px">
  `
  $
  \text{Bispectrum: } \quad \langle \delta(\boldsymbol{k}_1)\,\delta(\boldsymbol{k}_2)\,\delta(\boldsymbol{k}_3)\rangle = (2\pi)^3 B(k_1,k_2,k_3)\,\delta_D(\boldsymbol{k}_1+\boldsymbol{k}_2+\boldsymbol{k}_3)
  $
  `
</p>

<div>
  <img src="/presentations/pdf02.png", style="width:300px; background:none; border:none; box-shadow:none; float:left"/>

  <img class="fragment" data-fragment-index="1", src="/presentations/pk_bisp_minerva_b1b2.png", style="width:320px; background:none; border:none; box-shadow:none; float:center"/>

  <img class="fragment" data-fragment-index="2", src="/presentations/spherex2.png", style="padding-left:15px; width:310px; background:none; border:none; box-shadow:none; float:right"/>
  </div>

  <div style="position: absolute; top: 17.3em; left: 0.0em; width: 300px; height: 50px;">
    <font size="-1">
      [<span style="color:DarkTurquoise">Credit: M. Schmittfull</span>]
    </font>
  </div>
  <div style="position: absolute; top: 19em; left: 0.0em; width: 300px; height: 50px;">
    The observed density field is non-Gaussian
  </div>

  <div class="fragment" data-fragment-index="1" style="position: absolute; top: 19em; left: 12.5em; width: 300px; height: 50px;">
    Breaking parameter degeneracies
  </div>

  <div class="fragment" data-fragment-index="2" style="position: absolute; top: 17.3em; left: 25.5em; width: 300px; height: 50px;">
    <font size="-1">
      [<span style="color:DarkTurquoise">Dore+ '14</span>]
    </font>
  </div>
  <div class="fragment" data-fragment-index="2" style="position: absolute; top: 19em; left: 25.5em; width: 300px; height: 50px;">
    Cosmic variance limit is approaching
</div>

Note:
- reason number 1: density is non-Gaussian (if Gaussian all info in P)
- reason number 2: bispectrum has different parameter dependencies
- reason number 3: cosmic variance limit

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
## <span style="color:#f0f1eb"> <b>Bias Expansion & State of the Art</b> </span>

---

<!-- {_style="text-align: center"}-->
# Bias Expansion

<div class="fragment" data-fragment-index="1"></div>

<p>
  `
  $$
  \begin{array}{c}\text{galaxy} \\[-0.3em]\text{abundance}\end{array} \quad \Leftarrow \quad
  \color{red}\begin{array}{c}\text{local gravitational}\\[-0.3em]\text{effects}\end{array}
  \color{black} \quad + \quad \color{#1a3f8b}
  \begin{array}{c}\text{matter distribution within}\\[-0.3em]\text{Lagrangian radius of halos}\\[-0.3em] \text{(non-local)} \end{array}
  $$
  `
</p>

<div style="position: absolute; top: 10.3em; left: 11.2em; width: 700px; height: 150px; font-size:80%">
[<span style="color:DarkTurquoise">Chan+ '12, Assassi+ '14, Marbabayi+ '15, Desjacques+ '16</span>]
</div>

<p>
  <hr style="height:0.8em; visibility:hidden;"/>
</p>

<p>
  `
  $$
  \newcommand\mystrut[1]{\vrule width0pt height0pt depth#1\relax}
  \begin{align}
  \fragment{1}{\delta_g(\boldsymbol{x}) = }\hspace{0.5em}& \fragment{1}{b_1\,\delta(\boldsymbol{x}) + \frac{b_2}{2}\,\delta^2(\boldsymbol{x}) + \gamma_2\,{\cal G}_2(\boldsymbol{x}|\Phi_v) \hspace{4em} \leftarrow \; \text{tree-level bias} } \\[0.5em]
  & \fragment{2}{\left.\begin{array}{l} \displaystyle \hspace{-0.3em} + \; \frac{b_3}{3!}\,\delta^3(\boldsymbol{x}) + \gamma_3^{\times}\,\delta(\boldsymbol{x})\,{\cal G}_2(\boldsymbol{x}|\Phi_v) \\[0.5em] \hspace{-0.3em} + \; \gamma_3^-\,\underbrace{\Delta_3{\cal G}(\boldsymbol{x}|\Phi,\Phi_v)}_{=\,{\cal G}_2(\Phi_v)-{\cal G}_2(\Phi)} + \gamma_3\,{\cal G}_3(\boldsymbol{x}|\Phi_v) \quad \\ \hspace{-0.3em} + \; \big[\text{fourth order terms}\big] \end{array}\right\} \hspace{1.6em} \leftarrow \; \text{one-loop bias} } \\[1em]
  & \fragment{4}{\hspace{-0.3em} \underbrace{\begin{array}{c} + \; \gamma_A\,\nabla^2 \delta(\boldsymbol{x}) + \gamma_B\,\nabla^2{\cal G}_2(\boldsymbol{x}) + \gamma_C\,\nabla^2 \delta^2(\boldsymbol{x}) + \gamma_D\, \left[\boldsymbol{\nabla}\delta(\boldsymbol{x})\right]^2 \\[-2em] \color{#f0f1eb}. \end{array}}_{\displaystyle \sim k^2\,R_L^2} }
  \end{align}
  $$
  `
</p>

<div class="fragment" data-fragment-index="2"></div>
<div class="fragment" data-fragment-index="3"></div>

<div class="fragment" data-fragment-index="4" style="position: absolute; top: 13.4em; left: 9em; width: 390px; height: 275px; font-size:75%;    border:3px; border-style:solid; border-color:red; padding: 10px; border-radius:8px"> </div>

<div class="fragment" data-fragment-index="5" style="position: absolute; top: 29.2em; left: 9em; width: 650px; height: 35px; font-size:75%;    border:3px; border-style:solid; border-color:#1a3f8b; padding: 10px; border-radius:8px"> </div>


---

<!-- .slide: data-transition="slide-in fade-out"-->
# The Observables <!-- {_style="text-align: center"}-->

<div style="position: absolute; top: 4em; left: 50%; width: 800px; height: 600px; margin: 0 0 0 -400px;">
  <p> Expand observables using <b>bias relation</b> and <b>perturbation theory</b>:
    `
    $$
    \begin{align}
    \\[0.1em]
    \Rightarrow \hspace{1em} P(k) &= \underbrace{P_{\mathrm{tree}}(k)}_{\langle\delta^{(1)}\delta^{(1)}\rangle} \hspace{0.3em} + \underbrace{P_{\mathrm{1-loop}}(k)}_{\langle\delta^{(1)}\delta^{(3)}\rangle,\hspace{0.25em}\langle\delta^{(2)}\delta^{(2)}\rangle} + \ldots + P_{\text{noise}}\\[1em]
    \Rightarrow \hspace{1em} B(k_1,k_2,k_3) &= \underbrace{B_{\mathrm{tree}}(k_1,k_2,k_3)}_{\langle\delta^{(1)}\delta^{(1)}\delta^{(2)}\rangle} \hspace{0.3em} + \underbrace{B_{\mathrm{1-loop}}(k_1,k_2,k_3)}_{\substack{\langle\delta^{(4)}\delta^{(1)}\delta^{(1)}\rangle,\hspace{0.25em}\langle\delta^{(3)}\delta^{(2)}\delta^{(1)}\rangle,\\ \langle\delta^{(2)}\delta^{(2)}\delta^{(2)}\rangle}} + \ldots + B_{\text{noise}}
    \end{align}
    $$
    `
  </p>
</div>


Note:
  - intend to use PT to describe the clustering of galaxies. What is being done in PT in general is to expand the density in functions, which contain increasing powers of the linear density field
  - remember from previous slide: Gaussian means that all information is contained in the power spectrum

---

<!-- .slide: data-transition="fade-in slide-out"-->
# The Observables <!-- {_style="text-align: center"}-->

<div style="position: absolute; top: 4em; left: 50%; width: 800px; height: 600px; margin: 0 0 0 -400px;">
  <p> Expand observables using <b>bias relation</b> and <b>perturbation theory</b>:
    `
    $$
    \begin{align}
    \\[0.1em]
    \Rightarrow \hspace{1em} P(k) &= \underbrace{\color{red}P_{\mathrm{tree}}(k)}_{\langle\delta^{(1)}\delta^{(1)}\rangle} \hspace{0.3em} + \underbrace{\color{red}P_{\mathrm{1-loop}}(k)}_{\langle\delta^{(1)}\delta^{(3)}\rangle,\hspace{0.25em}\langle\delta^{(2)}\delta^{(2)}\rangle} + \ldots + P_{\text{noise}}\\[1em]
    \Rightarrow \hspace{1em} B(k_1,k_2,k_3) &= \underbrace{\color{red}B_{\mathrm{tree}}(k_1,k_2,k_3)}_{\langle\delta^{(1)}\delta^{(1)}\delta^{(2)}\rangle} \hspace{0.3em} + \underbrace{B_{\mathrm{1-loop}}(k_1,k_2,k_3)}_{\substack{\langle\delta^{(4)}\delta^{(1)}\delta^{(1)}\rangle,\hspace{0.25em}\langle\delta^{(3)}\delta^{(2)}\delta^{(1)}\rangle,\\ \langle\delta^{(2)}\delta^{(2)}\delta^{(2)}\rangle}} + \ldots + B_{\text{noise}}
    \end{align}
    $$
    `
  </p>
</div>

<p>
  <hr style="height:11.5em; visibility:hidden;"/>
</p>

<span style="color:red"> <b>State of the Art!</b> </span> &mdash; Further model assumptions include:
<ul>
  <li>
    local <b>Lagrangian</b> bias:
      `
      $
      \displaystyle \quad \Rightarrow \hspace{0.5em} \gamma_2 = -\frac{2}{7} (b_1-1) \quad
      $
      `
      [<span style="font-size:80%; color:DarkTurquoise">Chan+ '12, Baldauf+ '12</span>]
  </li>
  <p><hr style="height:0.2em; visibility:hidden;"/></p>
  <li>
    treatment of noise:
      `
      $
      \quad
      \begin{array}{l}
      \displaystyle
      P_{\mathrm{noise}} = \epsilon_0\,P_{\mathrm{Poisson}} \\
      B_{\mathrm{noise}} = \epsilon_0\,B_{\mathrm{Poisson}}
      \end{array} \quad
      $
      `
      [<span style="font-size:80%; color:DarkTurquoise">Gil-Mar&iacute;n+ '16</span>]
  </li>
</ul>



Note:
  - intend to use PT to describe the clustering of galaxies. What is being done in PT in general is to expand the density in functions, which contain increasing powers of the linear density field
  - remember from previous slide: Gaussian means that all information is contained in the power spectrum

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/bspec_BOSSlike_nomodel.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 10em; left: 29.5em; width: 350px; height: 600px; font-size:75%">
  [Minerva Simulations: <span style="color:DarkTurquoise">Grieb+ '16</span>]
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/bspec_BOSSlike_3.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

<div style="position: absolute; top: 10em; left: 29.5em; width: 350px; height: 600px; font-size:75%">
  [Minerva Simulations: <span style="color:DarkTurquoise">Grieb+ '16</span>]
</div>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_pk+Bggg_BOSSlike_kmax0p10.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

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
      [<span style="font-size:80%; color:DarkTurquoise">Chan+ '12, Baldauf+ '12</span>]
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
      [<span style="font-size:80%; color:DarkTurquoise">Gil-Mar&iacute;n+ '16</span>]
    </li>
  </ul>
</div>

---

<!-- .slide: data-transition="fade-in fade-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_pk+Bggg_BOSSlike_kmax0p15.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

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
      [<span style="font-size:80%; color:DarkTurquoise">Chan+ '12, Baldauf+ '12</span>]
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
      [<span style="font-size:80%; color:DarkTurquoise">Gil-Mar&iacute;n+ '16</span>]
    </li>
  </ul>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# The State of the Art

<img src="/presentations/contours_pk+Bggg_BOSSlike_kmax0p20.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none; float:right"/>

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
      [<span style="font-size:80%; color:DarkTurquoise">Chan+ '12, Baldauf+ '12</span>]
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
      [<span style="font-size:80%; color:DarkTurquoise">Gil-Mar&iacute;n+ '16</span>]
    </li>
  </ul>
</div>

---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Bias Loops</b> </span>

---

<!-- .slide: data-transition="slide-in fade-out"-->
# Issues at 1-Loop and Beyond <!-- {_style="text-align: center"}-->

For simplicity consider **local** (in matter) bias expansion:

<div style="position: absolute; top: 6em; left: 50%; width: 500px; height: 600px; margin: 0 0 0 -300px;">
  <p>
    `
    $$
    \delta_g = b_1\,\delta_L + \frac{b_2}{2} \delta_L^2 + \frac{b_3}{3!} \delta_L^3 + \ldots = \sum_{n=1}^{\infty} \left(\frac{\partial^n \delta_g}{\partial \delta_L^n}\right) \frac{\delta_L^n}{n!}\,, \hspace{1em} \delta_L \equiv \delta^{(1)}
    $$
    `
  </p>
</div>

---

<!-- .slide: data-transition="fade-in slide-out"-->
# Issues at 1-Loop and Beyond <!-- {_style="text-align: center"}-->

For simplicity consider **local** (in matter) bias expansion:

<div style="position: absolute; top: 6em; left: 50%; width: 500px; height: 600px; margin: 0 0 0 -300px;">
  <p>
    `
    $$
    \delta_g = \color{red}b_1\color{black}\,\delta_L + \frac{\color{red}b_2\color{black}}{2} \delta_L^2 + \frac{\color{red}b_3\color{black}}{3!} \delta_L^3 + \ldots = \sum_{n=1}^{\infty} \left(\frac{\partial^n \delta_g}{\partial \delta_L^n}\right) \frac{\delta_L^n}{n!}\,, \hspace{1em} \delta_L \equiv \delta^{(1)}
    $$
    `
  </p>
</div>

<hr style="height:3.5em; visibility:hidden;"/>

<div>
  <span style="color:red"> These bias parameters are <b>NOT</b> measurable quantities! </span>
</div> <!-- {_style="text-align: center"}-->

<div class="fragment" data-fragment-index="1">
  <p>
    `
    $$
    \text{e.g.} \quad P_g(k) = b_1^2\,P_L(k) + \left[b_1 b_3 \langle\delta^2_L\rangle P_L(k) + \frac{b_2^2}{2} (P_L \otimes P_L)(k)\right] + \ldots
    $$
    `
  </p>
  $\rightarrow \hspace{0.5em}$ requires &quot;<b>renormalization</b>&quot; of bias parameters: `$\hspace{0.5em}b_1^R \equiv b_1 + b_3\frac{\langle\delta^2_L\rangle}{2} + \ldots$`
  <div style="font-size:75%">
    $\hspace{2.2em}$[<span style="color:DarkTurquoise">McDonald '07, Schmidt+ '13, Assassi+ '14, Mirbabayi+ '15</span>]
  </div>
</div>

<div class="fragment" data-fragment-index="2">
  <hr>
  <p>
    `
    $$
    \begin{align}
      \Rightarrow \hspace{0.5em}b_1^R &= b_1 + b_3 \frac{\langle\delta^2_L\rangle}{2} + \ldots = \sum_{n=0}^{\infty} \frac{b_{2n+1}}{n!} \left(\frac{\langle\delta^2_L\rangle}{2}\right)^n = \left<\frac{\partial \delta_g}{\partial \delta_L}\right> \\
      \Rightarrow \hspace{0.5em}b_2^R &= b_2 + b_4 \frac{\langle\delta^2_L\rangle}{2} + \ldots = \sum_{n=0}^{\infty} \frac{b_{2n+2}}{n!} \left(\frac{\langle\delta^2_L\rangle}{2}\right)^n = \left<\frac{\partial^2 \delta_g}{\partial \delta_L^2}\right>
    \end{align}
    $$
    `
  </p>
</div>

---

## Multi-point Propagator Expansion <!-- {_style="text-align: center"}-->

<p>
  `
  $$
  \text{Generalization:} \hspace{0.5em} \frac{\partial^n \delta_g}{\partial \delta_L^n} \hspace{0.5em} \rightarrow \hspace{0.5em} \left<\underbrace{\frac{\partial^n \delta_g(\boldsymbol{k})}{\partial \delta_L(\boldsymbol{k}_1) \cdots \partial \delta_L(\boldsymbol{k}_n)}}\right> \equiv (2\pi)^3\,\Gamma_g^{(n)} \delta_D(\boldsymbol{k}-\boldsymbol{k}_{1\cdots n})
  $$
  `
</p>

<div style="position: absolute; top: 7.2em; left: 2.5em; width: 1000px; height: 600px;">
  <span style="color:red">scale dependence due to environment dependence in bias expansion, e.g. `${\cal G}_2$`</span>
</div>

<hr style="height:0.8em; visibility:hidden;"/>

<div class="fragment" data-fragment-index="1">
  Modify expansion by using real observables as coefficients:
  <p style="border:2px solid black; padding:3px; border-radius:8px">
    `
    $$
    \begin{align}
      \delta_g(\boldsymbol{k}) = &\Gamma_g^{(1)}(\boldsymbol{k})\,\delta_L(\boldsymbol{k}) + \frac{1}{2} \Gamma_g^{(2)}(\boldsymbol{k}_1,\boldsymbol{k}_2) \otimes \Big[\delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2) - \langle\delta_L^2\rangle\Big] \\
      &\frac{1}{3!}\Gamma_g^{(3)}(\boldsymbol{k}_1,\boldsymbol{k}_2,\boldsymbol{k}_3) \otimes \Big[\delta_L(\boldsymbol{k}_1)\delta_L(\boldsymbol{k}_2)\delta_L(\boldsymbol{k}_3) - \langle\delta_L^2\rangle \delta_L(\boldsymbol{k}_1) - \text{cyc.}\Big] \hspace{-0.3em}+ \ldots
    \end{align}
    $$
    `
  </p>
</div>

<hr style="height:0.1em; visibility:hidden;"/>

<div class="fragment" data-fragment-index="2">
  <img src="/presentations/spaghetti.png", style="position:relative; top:-35px; left:0em; height:240px; background:none; border:none; box-shadow:none;"/>

  <div style="position: absolute; top: 18em; left: 9.5em; width: 300px; height: 200px;">
    `$\displaystyle \Gamma_g^{(n)}(\boldsymbol{k}_1,\ldots\,;\tau)$`
  </div>

  <div style="position: absolute; top: 17em; left: 7.5em; width: 500px; height: 250px;">
  <svg width="500" height="400">

      <defs>
          <marker id="arrow" markerWidth="13" markerHeight="13" refx="2" refy="6" orient="auto">
              <path d="M2,2 L2,11 L10,6 L2,2" style="fill:red;" />
          </marker>
      </defs>

      <path d="M-100,320 L50,100"
            style="stroke:red; stroke-width: 2.25px; fill: none;
                   marker-end: url(#arrow);"
      />

  </svg>  
  </div>

  <div style="position: absolute; top: 25em; left: 4.8em; width: 300px; height: 200px;">
    `$\displaystyle \Gamma_g^{(n)}(\boldsymbol{k}_1,\ldots\,;\tau=0)$`
  </div>

  <div style="position: absolute; top: 19em; left: 17.5em; width: 500px; height: 100px;">
    <div style="border:5px solid #f5d328; padding:10px; border-radius:8px;">
      Compute `$\Gamma_g^{(n)}({\boldsymbol{k}_1,\ldots,\boldsymbol{k}_n})$` and identify renormalized bias parameters on <b>initial</b> time slice, then <b>evolve</b>!
    </div>
    <div style="text-align:center; font-size:80%">
      (can be automated symbolically in <code>mathematica</code>)
    </div>
  </div>

  <div style="font-size:70%; position: absolute; top: 25em; left: 0em; width: 200px; height: 600px;">
    Picture: <br> Desjacques+ '16
  </div>
</div>

---

<!-- {_style="text-align: center"}-->
# An Inventory of the Model

<p>
  `
  $$
  \begin{align}
  B_g(k_1,k_2,k_3) &= \Big(b_1^R\Big)^3\,B_{\text{matter}}(k_1,k_2,k_3) \\[0.2em] &\fragment{1}{\,+\, \Big(b_1^R\Big)^2\,\Big[b_2^R\,P_L(k_1)\,P_L(k_2) + 2\gamma_2^R\,K(\boldsymbol{k}_1,\boldsymbol{k}_2)\,P_L(k_1)\,P_L(k_2) + \text{cyc.}\Big]} \\[0.2em]
  &\fragment{2}{\,+\, \text{37 bias loop integrals}} \\[0.2em]
  &\fragment{3}{\,+\, \underbrace{\epsilon_0\,C_1 + \eta_0\,C_2\,\Big[P_L(k_1) + P_L(k_2) + P_L(k_3)\Big]}_{\displaystyle B_{\text{noise}}}}
  \end{align}
  $$
  `
</p>

<hr style="height:0.5em; visibility:hidden;"/>

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
# Back to the Data!

<img src="/presentations/bspec_BOSSlike_3.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="fade-in slide-out"-->
<!-- {_style="text-align: center"}-->
# Back to the Data!

<img src="/presentations/bspec_BOSSlike_4.png", style="position:relative; top:-35px; height:610px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="slide-in fade-out"-->
<!-- {_style="text-align: center"}-->
# Combined Constraints


<img src="/presentations/contours_pk+Bggg_kmax0p10.png", style="position:relative; top:-35px; left:-80px; width:600px; background:none; border:none; box-shadow:none;"/>

---

<!-- .slide: data-transition="fade-in fade-out"-->
<!-- {_style="text-align: center"}-->
# Combined Constraints


<img src="/presentations/contours_pk+Bggg_kmax0p15.png", style="position:relative; top:-35px; left:-80px; width:600px; background:none; border:none; box-shadow:none;"/>

---

<!-- {_style="text-align: center"}-->
<!-- .slide: data-transition="fade-in slide-out"-->
# Combined Constraints

<img src="/presentations/contours_pk+Bggg_kmax0p20.png", style="position:relative; top:-35px; left:-80px; width:600px; background:none; border:none; box-shadow:none; font-size:75%"/>

<div style="position: absolute; top: 9em; left: 17em; width: 500px; height: 128px; border:2px solid black; padding:3px; border-radius:8px" class="fragment">
  <ul>
    <li>
      <b>consistency</b> between $P$ and $B$
    </li>
    <li>
      $b_2$ agrees with PBS prediction <span style="font-size:70%">[<span style="color:DarkTurquoise">Lazeyras+ '15</span>]</span>
    </li>
    <li>
      $\gamma_2$ slightly below local Lagrangian value <br> <span style="font-size:70%">[<span style="color:DarkTurquoise">Lazeyras & Schmidt '17</span>]</span>
    </li>
  </ul>
</div>


---

<!-- .slide: data-background-color="#1a3f8b"-->
<!-- {_style="text-align: center"}-->
# <span style="color:#f0f1eb"> <b>Summary</b> </span>

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




</script>
</section>


 <!-- &emsp; -->
