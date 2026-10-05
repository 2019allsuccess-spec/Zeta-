# Zeta
Zeta-function-calculator:
________________________________________________________________________________________________________________________________________________
A zeta function calculator in C# and R languages. Using the logarithm scale of the ring of intergers (n) to reach the infinite sums compressed in a linear progression (DoubleSquare) through the exponential invariant of the Euler Xi function.

Uma calculadora da função zeta nas linguagens C# e R. Utilizando a escala logarítmica do anel dos números inteiros (n) para chegar à somas infinitas comprimidas em uma progressão linear (DoubeSquare) através do invariante exponencial da função Xi de Euler.
________________________________________________________________________________________________________________________________________________

* Introduction: mathematical fundaments


The Riemann zeta function is a Drichlet serie of the group of L-Function wich limit is defined at infinity and its domain is complex, its power series and sums runs over the complex numbers. The domain input is defined by the argument of the function represented by the variable (s). It was introduced by Bernhard Riemann in 1859. Bellow the zeta function:

<img width="131" height="68" alt="Captura de tela 2026-10-05 112401" src="https://github.com/user-attachments/assets/2a7d889d-acde-496c-8db2-8ea132ce2cf8" />


​
<p>Considering the caracteristics of the function introduced by Riemann, the limit at infinite and the complex domain, is needed a strict and rigorous method to study the behaviour of the function at infinity because the famous hypothesis conjectured by Riemann about the mistery of the distribution of the prime numbers, as well the undestanding of the infinity itself. In the shadow of these misteries, Riemann formulated his comkplex analyses from the estereographic projection, conjecturing a projective sphere with a point at infinity (the North), the complex plane as the Equator, the Origin (the South), and a special straigt line intersecting the sphere, connecting to a point at the infinite - which is known as the Riemann Sphere.<p/>

<p>However, the measure and simetry of the sphere is intringly missunderstood at the first sought. Our mathematical interpretation for that straight line is the logarithm progression, or logarithm scale, that compress the projection of all sets of numbers until infinity and allows all kind of computations.<p/>  


* The complex analyses through the Riemann sphere

<>pBefore a view of the complex analyses of the zeta function in the Riemann projective sphere, is of some importance to understanding the complex powers. The first studies of the complex powers was developed by scholars as Euler, who discover the natural constatnt (e), and with others contributors coined the natural logarithm. And in this context, Euler published his Xi function, that states: e<sup> Xi </sup> = cos(X)+i*sin(X).</p>

<p>However, alhough this formula being incomplete (do not work with algebraic complex numbers like Z = X + Yi; or z = Re + Im), is the basic lesson for the expanded Xi function and its integral invariant (presented in this paper and in the complex analyses). Bellow, follow the algebraic Xi expansion:</p>


 e<sup> Z </sup> = e<sup> Re(Z) </sup> [cos(Im(Z)) + i · sin(Im(Z))]



<p>From the statement of this algebraic expansion above is possible to expose here its applications, and how it connects to the zeta function complex analyses.

Let's make Z = s * ln(n)  to solve complex powers as the zeta function terms like 1/n<sup> s </sup>. Hence, the variable (n) is the base, and (s), the exponent to solve
the term do: e<sup> Z </sup> or


e<sup> Z </sup> = e<sup> - s * ln(n) </sup>


</p>


<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@4/tex-mml-chtml.js"></script>









