---
layout: post
title:  "Obstructions to analytic proofs of the Riemann Hypothesis"
date:   2018-09-29 10:38:00
author: Ralph Furman
categories: riemann
---

Given that the Riemann zeta function is defined by a few concrete sums and integrals, and the [Riemann Hypothesis](/blems/riemann/) seems to be a purely complex-analytic question, it is very tempting to attempt to tackle it via purely complex-analytic means.  However, a proof of any zero-free region generally requires the Euler Product, and hence information about the primes.  Furthermore the Riemann Hypothesis would make the zeta function so unique and special that there isn't a single proven example of a function with the same kinds of growth rates.  All such hypothesized functions (ie: the [Selberg Class](https://en.wikipedia.org/wiki/Selberg_class)) are defined by very complicated algebra, and are more properly seen via [p-adic](https://en.wikipedia.org/wiki/P-adic_analysis) and [adelic](https://people.maths.bris.ac.uk/~as12313/adele-course/) analysis.

#### There is no analytic function known to satisfy a Riemann Hypothesis

Consider the following properties of zeta and other L-functions \\(f(s)\\).
1. \\(f(s)\\) is complex-analytic on \\(\mathbb{C}\\) except for possibly a finite set of poles.
2. For some \\(\delta>0\\), \\(f(s)\\) is bounded when \\(\Re(s)>1+\delta\\).
3. \\(f(s)\\) is of order 1, in other words polynomial growth on vertical lines:  \\(f(\sigma+i T) = O(n^{A_\sigma})\\) for every \\(\sigma\in\mathbb{R}\\).
4. (Riemann Hypothesis) If \\(f(s)=0\\) and \\(0<\\Re(s)<1\\) then \\(\Re(s)=1/2\\)

There is no function that provably satisfies these properties, even though all Selberg Class functions are conjectured to.

Put another way, consider the growth rate of \\(\zeta(\sigma+iT)\\) as a function of \\(T\\) for various \\(\sigma\\).  Around \\(\sigma=1/2\\) this function undergoes a phase transition corresponding to the infinitude of zeros on the critical line, for example it transitions from having finite mean square to infinite mean square.  There is another phase transition at \\(\sigma=1\\) as the function goes from bounded to unbounded, and known constructions of such functions have an infinitude of zeros close to \\(\Re(s)=1\\).

#### A function satisfying RH would behave very differently from any known function
This is [expanded on by Ivic](https://arxiv.org/abs/math/0311162).

Entire functions that are nowhere vanishing are very restricted in behavior, for example their range [cannot miss any other value](https://en.wikipedia.org/wiki/Liouville%27s_theorem_(complex_analysis)), and they are linearly independent (See [Bocher](https://www.jstor.org/stable/pdf/2007186.pdf)).

Many of these theorems apply also to complex functions on a disc that are "very large" near their boundary.  For example, [Schottky's Theorem](https://en.wikipedia.org/wiki/Schottky%27s_theorem) is Liouville's function on a disc.  More applications are in [Functions of One Complex Variable by Conway](https://www.amazon.com/Functions-Complex-Variable-Graduate-Mathematics/dp/0387903283) and [Complex Hyperbolic Spaces by Lang](https://www.springer.com/us/book/9780387964478), along with results of value distributions by Nevanlinna.

Observing \\(\zeta(1.5+i T)\\) on a disc of radius 1, for very large \\(T\\), this function is uniformly bounded near the center, non-vanishing, and very large once \\(T\\) is sufficiently large, so the above theorems can be applied.  This shows in particular that the range will contain a very large torus, and the function will have zeros if you perturb it slightly by an analytic function.

#### Euler products appear to be necessary

Proofs of non-vanishing to the right of and [on the line \\(\Re(s)=1\\)](http://www-users.math.umn.edu/~garrett/m/complex/notes_2014-15/09_prime_number_theorem.pdf) require expressing \\(\log(\zeta)\\) as a sum over primes.  This is also a necessary ingredient in both growth-rate estimates and heuristics inside the critical strip.

It is generally expected that sum information from the Euler product is necessary for the Riemann Hypothesis.

[Other L-functions](https://en.wikipedia.org/wiki/Artin_L-function) require even more algebraic structure.


#### Other L-Functions have non-simple zeros

See [this comment by Terry Tao](https://terrytao.wordpress.com/2018/09/06/polymath15-tenth-thread-numerics-update/#comment-505250) and the [mentioned lecture by Peter Sarnak](https://aimath.org/rh2018/)

#### If true, it is "barely true"
The Riemann Hypothesis is true if and only if the [De Bruijn–Newman constant](https://en.wikipedia.org/wiki/De_Bruijn%E2%80%93Newman_constant) is non-positive.  Lower bounds on this constant have been repeatedly strengthened, and [Terry Tao](https://terrytao.wordpress.com/2018/01/19/the-de-bruijn-newman-constant-is-non-negativ/) has recently proven the constant is non-negative.  This is sometimes interpreted as the statement that if the Riemann Hypothesis is true then it is "barely true".

This also gives rigid results on compositions of the zeta function with other analytic functions, making Atiyah's approach very difficult to navigate.

This also shows that functions satisfying a Riemann Hypothesis are very isolated and very special, and one would expect that any small adjustment or perturbation would destroy this property, greatly restricted the set of techniques that are valid.

#### We have not seen where the zeta function gets complicated

There is a tight asymptotic for the number of zeros up to height \\(T\\).  The function \\(S(T)\\) measures the discrepancy from this asymptotic and is known to have mean 0, and is expected to grow somewhat like \\(\sqrt{\log T}\\).  Any counterexample to the Riemann Hypothesis would be a pair of zeros symmetric around the critical line, so \\(S(T)\\) would instantly jump by 2.

While there are verifications of the Riemann Hypothesis up to height \\(~10^{24}\\), there is no observation where \\(\|S(T)\|>3\\), so in a way the zeta function is very simple in this range and too restricted to expect to numerically check the Riemann Hypothesis.  Some heuristics have the complexity of the zeta function growing like \\(\log\log\log T\\) and imply that counterexamples might be generic once \\(T>\exp(\exp(\exp(3)))\\)

See [Sector 4.3.4 Behaviour of S(T)](http://numbers.computation.free.fr/Constants/Miscellaneous/zetazeros1e13-1e24.pdf).

#### Results on value distributions

[The Theory of the Riemann Zeta Function by Titchmarsh and Heath-Brown](https://www.amazon.com/Theory-Riemann-Zeta-Function-Science-Publications/dp/0198533691) contains detailed results on the distributions of values inside the critical strip, growth rates, mean values, and asymptotics on how often \\(\zeta(s)\\) takes on each non-zero value.  These make it very difficult to "separate" the values away from 0, since it does not leave much space for separation.

#### Heuristics may point more to 100% of zeros, rather than all zeros

There is often an appeal to randomness and to oscillating sums cancelling out, and the notion that so many "coincidences" would have to occur for the Riemann Hypothesis to be false.  This ironically may make the numerical evidence weaker because it shows that we may not expect to see counterexamples until height around \\(\exp(\exp(\exp(3)))\\).

Analogy is sometimes made to the proof of [The Riemann Hypothesis on Curves](https://en.wikipedia.org/wiki/Weil_conjectures).  In this case the functions in question are polynomials, so [bounds on moments](https://terrytao.wordpress.com/2018/06/07/heat-flow-and-zeroes-of-polynomials-ii-zeroes-on-a-circle/) can determine these all to lie on a circle.  In the case of the Riemann zeta function, corresponding moment bounds are known or expected, but since this is not a polynomial, it would just imply that 100% of zeros are arbitrarily close to the critical line, which is already a known result.  

#### There is no compelling reason to believe the Riemann Hypothesis

The conjecture was made due to simplicity, symmetry, and numerical calculation.  There is much more calculation now, but it is still far from the range of values where \\(\zeta(s)\\) begins to show its full complexity.  There are analogues to the finite field case, but those are arguably more related to the mean value and density results.  There is still no compelling reason to expect the Riemann Hypothesis to be true, nor is there any complex analytic function with similar growth rates that satisfies a Riemann Hypothesis.



****

### Have I forgotten something?
Please let me know in the comments, or [add it yourself!](https://github.com/rfurman/pnphard)

