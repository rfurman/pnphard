---
layout: page
title: "Profound Non-Proofs of: Riemann Hypothesis"
permalink: /blems/riemann/
---


*NOTE*{: style="color: red"}:
The Fields Medalist [Sir Michael Atiyah](https://en.wikipedia.org/wiki/Michael_Atiyah) has [claimed a proof](https://twitter.com/hlforum/status/1042670700652318720?s=21) and is [presenting](https://www.heidelberg-laureate-forum.org/) this Monday Sept 24, although there is no additional context for this.



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

1885
: Stieltjes wrote to Hermite that he proved the Riemann Hypothesis by bounding the summatory function of \\(\mu\\), although the proof was messy, so he set it aside to come up with a cleaner one, and could never reconstruct it afterwards.

1896
: Hadamard and de la Vallée Poussin filled in the gaps behind Riemann's intuitive proof, made it rigorous, and proved that there are no zeros with \\(\Re(s)=1\\).  Hadamard had to explain in his paper that he was publishing this because Stieltjes' proof of the Riemann Hypothesis was unpublished and probaby more difficult.

1900
: David Hilbert posed a [list of 23 important unsolved problems](https://en.wikipedia.org/wiki/Hilbert%27s_problems), the 8th of which was the Riemann Hypothesis.

1901
: von Koch shows that the Riemann Hypothesis is equivalent to the prime number theorem having an error term of \\(O(\sqrt{x}\log x)\\)

~1907
: [Littlewood](https://en.wikipedia.org/wiki/John_Edensor_Littlewood) is given the Riemann Hypothesis as a thesis problem.  

1914
: Hardy proves that there are infinitely many zeros on the critical line, later improved to positive proportions by Selberg, Levinson, and Conrey.

~1950s
: Atle Selberg works on the Riemann Hypothesis but ends up developing [a major field of study](https://en.wikipedia.org/wiki/Selberg_trace_formula)

~1969
: Paul Cohen works on the Riemann Hypothesis and is not heard from again (kidding)

1973
: Montgomery notices that the zeros behave statistically like eigenvalues of large random matrices, which kicks of the study of [Riemann Zeros and Random Matrix Theory](http://www.bourbaphy.fr/keating.pdf)

1976
: The [Miller-Rabin](https://en.wikipedia.org/wiki/Miller–Rabin_primality_test) primality test runs in polynomial time but only assuming the [Extended Riemann Hypothesis](https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis#Extended_Riemann_hypothesis_(ERH))

2000
: The Clay Math Institute listed its seven [Millenium Prize Problems](https://en.wikipedia.org/wiki/Millennium_Prize_Problems), each carrying a $1M prize and meant to be one of the hardest unsolved problems.  The Riemann Hypothesis was one of these.

Partial Results
=======================

### [Numerical verification](https://en.wikipedia.org/wiki/Riemann_hypothesis#Numerical_calculations)

Riemann originally verified the first 3 zeros, presently the [first 10 trillion zeros](http://numbers.computation.free.fr/Constants/Miscellaneous/zetazeros1e13-1e24.pdf) are known to satisfy the Riemann Hypothesis.

The general approach is as follows.  The functional equation determines the argument of the zeta function on the critical line, which allows one to study instead the real valued [Z function](https://en.wikipedia.org/wiki/Z_function).  Brute force evaluations of this function will find sign changes, which correspond to intervals containing zeros.  A particular contour integral counts the number of zeros in an rectangle, allowing a deterministic check for whether all zeros were found.

### [Zero-free regions](https://en.wikipedia.org/wiki/Riemann_hypothesis#Zero-free_regions)

When examining \\(\zeta(s)\\) for \\(s=\sigma+it\\) the result that there are no zeros with \\(\sigma\ge1\\) can be strengthened by taking \\(\sigma(t)<1\\) a function slowly converging to 1 as \\(t\rightarrow\infty\\).

De la Vallee-Poussin proved there is a constant \\(C\\) so that there are no zeros with \\(1-\sigma\le\frac{C}{\log t}\\), Littlewood strengthened this to \\(1-\sigma\le\frac{C\log\log t}{\log t}\\), and the strongest result is that there are no zeros with \\(1-\sigma\le\frac{1}{57.54(\log t)^{2/3}(\log\log t)^{1/3}}\\).

Explanations are in Titchmarsh and [here](https://vigoroushandwaving.wordpress.com/2013/04/22/the-zero-free-region-of-the-riemann-zeta-function/).

### [Proportion of zeros on the critical line](https://en.wikipedia.org/wiki/Riemann_hypothesis#Zeros_on_the_critical_line)

Hardy (1914) and Hardy & Littlewood (1921) showed there are infinitely many zeros on the critical line, by considering moments of certain functions related to the zeta function. Selberg (1942) proved that at least a (small) positive proportion of zeros lie on the line. Levinson (1974) improved this to one-third of the zeros by relating the zeros of the zeta function to those of its derivative, and Conrey (1989) improved this further to two-fifths.

Most zeros lie close to the critical line. More precisely, Bohr & Landau (1914) showed that for any positive ε, all but an infinitely small proportion of zeros lie within a distance ε of the critical line. Ivić (1985) gives several more precise versions of this result, called zero density estimates, which bound the number of zeros in regions with imaginary part at most T and real part at least 1/2+ε.

### Density results

### Riemann Hypothesis for Finite Fields


Approaches
=======================

### Bounds on summatory functions

When \\(\Re(s)>1\\) a formal calculation gives

$$1/\zeta(s) = \prod_{p\in\mathrm{prime}}(1-p^{-s}) = \sum \mu(s) n^{-s}$$

where \\(\mu(s)\\) is the [Mobius Function](https://en.wikipedia.org/wiki/M%C3%B6bius_function).

Defining the partial sums \\(M(x)=\sum_{n<x}\mu(n)\\) [Merten conjectured](https://en.wikipedia.org/wiki/Mertens_conjecture) that \\(-\sqrt(n)<M(x)<\sqrt(n)\\) for all \\(n>1\\).  Partial summation would then show that \\(1/\zeta(s)\\) is a well-defined analytic function for \\(\Re(s)>1/2\\) and prove the Riemann Hypothesis.

Odlyzko [disproved Merten's Conjecture](http://www.dtc.umn.edu/~odlyzko/doc/arch/mertens.disproof.pdf) but there is no specific counterexample known.  It is known that there exists a counterexample \\(x<e^{10^{41}}\\) and suspected that there is no counterexample \\(x<10^{20}\\) so an explicit counterexample might never be found.

Similarly,

$$\zeta(2s)/\zeta(s) = \prod_{p\in\mathrm{prime}}\frac1{1+p^{-s}} = \sum \lambda(s) n^{-s}$$

where \\(\lambda(s)\\) is the [Liouville Function](https://en.wikipedia.org/wiki/Liouville_function).

Defining the partial sums \\(L(x)=\sum_{n<x}\lambda(n)\\) [Polya conjectured](https://en.wikipedia.org/wiki/P%C3%B3lya_conjecture) that \\(L(n)\le0\\) for all \\(n>1\\).  Partial summation would then show that \\(1/\zeta(s)\\) is a well-defined analytic function until it reaches its rightmost pole at \\(s=1/2\\), thus proving the Riemann Hypothesis.  The smallest known counterexample is 906,150,257.


### Representation Theory

### Analogues to Function-Fields

### Bounding \\(\zeta(s)\\) away from 0

### Analytic arguments

### Random Matrix Theory

### Hilbert-Polya operators

### Selberg

Equivalent Formulations
======================

Generalizations
=======================

Almost-counter-examples, and other pitfalls
======================
