---
layout: page
title: Riemann Hypothesis
permalink: /blems/riemann/
---


*NOTE*{: style="color: red"}:
The Fields Medalist [Sir Michael Atiyah](https://en.wikipedia.org/wiki/Michael_Atiyah) has [claimed a proof](https://twitter.com/hlforum/status/1042670700652318720?s=21) and is [presenting](https://www.heidelberg-laureate-forum.org/) this Monday Sept 24, although this is no additional context for this.



Resources
=======================

For an overview there is:
* a great [explanation by Brian Conrey](https://www.ams.org/notices/200303/fea-conrey-web.pdf)
* a detailed [Wikipedia article](https://en.wikipedia.org/wiki/Riemann_hypothesis)
* an [introduction by Chris Caldwell](https://primes.utm.edu/notes/rh.html) .

For further reading there are some great books:
* [Edwards](https://www.amazon.com/Riemanns-Zeta-Function-Harold-Edwards/dp/0486417409) presents the historical context and intuition, along with a translation of Riemann's original paper, and detailed proofs.
* [Titchmarsh](https://www.amazon.com/Theory-Riemann-Zeta-Function-Science-Publications/dp/0198533691) is somewhat more modern (for a 1986 book) and presents a wider range of results, great for diving into the complex analysis of the Zeta function.

Also

* [On some reasons for doubting the Riemann Hypotheis](https://arxiv.org/abs/math/0311162) by Aleksandar Ivic.
* [An Essay on the Riemann Hypothesis](http://www.alainconnes.org/docs/rhfinal.pdf) by Alain Connes

Introduction
=======================

The function \\(\zeta(s)\\) has several consistent definitions depending on the range of \\(s\\).  For \\(s\in\mathbb{C}\\) with \\(\Re(s)>1\\):

$$\zeta(s)=1+2^{-s}+3^{-s}+\cdots.$$

Factoring yields the following formula relating to the primes, as long as \\(\Re(s)>1\\).  This also shows that \\(\zeta(s)\\) is never zero in this range.

$$\zeta(s) = \prod_{p\in \mathrm{primes}}\frac1{1-p^{-s}}.$$

A simple rearrangement yields a formula valid for \\(\Re(s)>0\\):

$$\zeta(s)=(1-2/2^s)^{-1}(1-2^{-s}+3^{-s}-\cdots.$$

Riemann proved a functional equation valid for all \\(s\in\mathbb{C}\\).

$$\zeta(s) = 2^s\pi^{s-1}\ \sin\left(\frac{\pi s}{2}\right)\ \Gamma(1-s)\ \zeta(1-s)$$

\\(\zeta(s)\\) can be expressed both as a product over primes and a product over its zeros, there is a Fourier duality between primes and zeros, which leads to an
[Explicit Formula](https://en.wikipedia.org/wiki/Explicit_formulae_(L-function)#Weil's_explicit_formula) turning a sum over primes into a sum of zeros and vice versa.  In particular this gives an explicit formula for [the number of primes up to x](http://empslocal.ex.ac.uk/~mwatkins/zeta/NTfourier.htm) as a sum of waves with discrete frequencies determines by the zeros.

History
=======================

1859
: Riemann published [On the number of primes less than a given quantity](http://www.claymath.org/publications/riemanns-1859-manuscript), using the analytic continuation of \\(\zeta(s)\\) and noting that there are no zeros \\(\Re(s)\ge1\\) to prove the [Prime Number Theorem](https://en.wikipedia.org/wiki/Prime_number_theorem)
: Via the [Riemann-Siegel formula](https://en.wikipedia.org/wiki/Riemann%E2%80%93Siegel_formula) (which Riemann discovered in the 1850s and Siegel found in Riemann's notes and published in 1932), Riemann was able to numerically compute the first zeros, and hypothesized that all non-trivial zeros have \\(\Re(s)=1/2\\)

1860
: stuff


Approaches
=======================
foo

Equivalent Formulations
======================
foo

Generalizations
=======================
foo

Almost-counter-examples, and other pitfalls
======================
foo
