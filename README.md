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
<p>Considering the caracteristics of the function introduced by Riemann, the limit at infinite and the complex domain, is needed a strict and rigorous method to study the behaviour of the function at infinity because the famous hypothesis conjectured by Riemann about the mistery of the distribution of the prime numbers, as well the undestanding of the infinity itself. In the shadow of these misteries, Riemann formulated his comkplex analyses from the estereographic projection, conjecturing a projective sphere with a point at infinity (the North), the complex plane as the Equator, the Origin (the South), and a special straight line intersecting the sphere, connecting to a point at the infinite - which is known as the Riemann Sphere.<p/>

<p>However, the measure and simetry of the sphere is intringly missunderstood at the first sought. Our mathematical interpretation for that straight line is the logarithm progression, or logarithm scale, that compress the projection of all sets of numbers until infinity and allows all kind of computations.<p/>  


* The complex analyses through the Riemann sphere

<p>Before a view of the complex analyses of the zeta function in the Riemann projective sphere, is of some importance to understanding the complex powers. The first studies of the complex powers was developed by scholars as Euler, who discover the natural constatnt (e), and with others contributors coined the natural logarithm. And in this context, Euler published his Xi function, that states: e<sup> Xi </sup> = cos(X)+i*sin(X).</p>

<p>However, alhough this formula being incomplete (do not work with algebraic complex numbers like Z = X + Yi; or z = Re + Im), is the basic lesson for the expanded Xi function and its integral invariant (presented in this paper and in the complex analyses). Bellow, follow the algebraic Xi expansion:</p>


 e<sup> Z </sup> = e<sup> Re(Z) </sup> [cos(Im(Z)) + i · sin(Im(Z))]



<p>From the statement of this algebraic expansion above is possible to expose here its applications, and how it connects to the zeta function complex analyses.

Let's make Z = s * ln(n)  to solve complex powers as the zeta function terms like 1/n<sup> s </sup>. Hence, the variable (n) is the base, and (s), the exponent to solve
the term do: e<sup> Z </sup> or


e<sup> Z </sup> = e<sup> - s * ln(n) </sup>


</p>


<p>At this point, to introduce the complex analyses through the Riemann sphere, attempting to avoid mistakes and computation errors on the behaviour of the zeta function, we have to give attention paticularly to the Riemann hyphotesis. This way, Riemann asserts that the roots (zeroes) of the zeta function are liying in a certain line, called critical line - which is a sucession of critical points defined by the function argument (s) that implies (in hyphotesis) in z(s)=0.</p>

However, the definition of these critical points is precisely given by:



<img width="164" height="45" alt="Captura de tela 2026-10-05 181417" src="https://github.com/user-attachments/assets/00e0ad8e-7ea1-4928-8dd4-f1d048716bdb" />



<p>Riemann has conjectured that the possible function roots, or critical points (s), have real part equal to 1/2, and this make much more sense when computing Re(s)>1, because the function converges, which implies in z(s)->1 (the function tends to 1). Now, lets visualize the behaviour of the function at the superior limit (n->Inf), taking the reference of the infinit limits definition  1/Inf = 0. Also by opposition: 1/0 = Inf (division by zero was introduce by Riemann in his complex analyses, now we have the definition of the North (1/0 = Inf) and the South (1/Inf = 0) of the Riemann sphere. Bellow, we can see more clearly in practice the domain of the zeta function illustrated by the ninth term, and the argument settled in the subspace of the complex plane (half plane - Riemann hypothesis):</p>



<img width="202" height="67" alt="Captura de tela 2026-10-05 160708" src="https://github.com/user-attachments/assets/4f805ad8-3120-4e2c-bc16-d7c87e0d0f9a" />

<p>Hence, making n<sup> s </sup> = X the maximum term of the function can be conjectured as 1/X. A big integer value of (n) to the power of (s) that produces 1/X = 0. This will be the last term in the sum. And this value is a point at infinity. Such value is referenced by the exponential function (EXP) oscillation, and is defined at around 10 <sup> 308 </sup>, because 1/10<sup> 308 </sup> = 0 for the majority of compilers (or 10<sup> -308 </sup>. And here we find the most  possible common error for the zeta function computation, because X depends on X(n, s), and the argument (s) assumes preciselly 1/2 as the real part, which will decrease the value of (n) until the region of its own square root, do not satifying the nontriviality of 1/X = 0,  because n<sup> 1/2+it </sup> -> sqrt(n).  To solve the problem is necessary to define X = 10<sup> 616 </sup>, that is the square of 10<sup>308</sup>, axpanding the domain of the function to the halfplane and then integring the whole domain, turning possible the computation of the hypothesis. </p> Then,

Lim 1/X (n, s = 1/2 + it),  n -> 10<sup> 616 </sup> 


<p>This limiar seens astronomicaly big, and the present complex analyses take the role to turn possible to compute until its "infinity" because X will reaches the region limit of the computation that is settled by <i>double</i> (IEE754) - which is 10<sup> 308 </sup>  in the exponential decrement/oscillation of (n) by (s). Here we begin the complex analyses to effectively define a compact serie for the zeta function at the Riemann sphere.  

Back to the integral invariant of the Euler formula Xi, we see that (n) stay in the logarithm scale and (n) -> 10^616: </p>

e<sup> Z </sup> = e<sup> - s * ln(n) </sup>

<p>Considering the ring of integers n -> {1 to 10<sup> 616 </sup>} in the logarihtm scale we have a compact range ln(n) -> {0 to 1418,3924...}. The linear progression of ln(n) turns possible to compute all terms of a divergent complex power serie as the zeta function. Simplifying the function to the most compact equivalence, in the zeta case: </p>


<img width="207" height="83" alt="Captura de tela 2026-10-05 180732" src="https://github.com/user-attachments/assets/f2b97d96-13e2-4be2-a5bd-cb1a84602625" />


as well, 

<img width="181" height="77" alt="Captura de tela 2026-10-05 180824" src="https://github.com/user-attachments/assets/515a24df-44f6-4ab4-9c19-d1f155321e78" />



<p>In practice is possible to visualize the graphic linear progression of all terms of a complex function until the point at infinity. Is inferred that is also possible the summation of the whole of it, becauses they have the same magnitude. As proposed by Riemann in his complex analyses through the projective sphere. The integral complex analyses may guide the path to the computation of infinite sums through the Riemann sphere. In this way, lets define the straight line P(z) = X at the Riemann sphere.

Making X = log(n) , X being the measurement space (Lebesgue) of the terms,  n<sup> -s </sup> = e<sup> -sX </sup> gives the following undefinite integral:</p>


<img width="298" height="86" alt="Captura de tela 2026-10-05 194239" src="https://github.com/user-attachments/assets/8e6fb7d7-66b8-44c8-a95a-c456f5ab3dfb" />


<p>Then we can define two segments or partitions of X, {X' + X"} = X,  creating two ranges for the sums:

X' runs between 0 to 709,1962...            
X" runs between 709,1962... to 1418,3924...  

The integration of these two regions is given by:</p>

<img width="144" height="71" alt="Captura de tela 2026-10-05 204948" src="https://github.com/user-attachments/assets/5f204667-a331-483c-a684-a50091db5415" />



And then the definite integral:

<img width="229" height="68" alt="Captura de tela 2026-10-05 204845" src="https://github.com/user-attachments/assets/3fac3a9b-5828-428b-96ed-21e9f1de13c3" />



Goes to:


<img width="471" height="84" alt="Captura de tela 2026-10-05 204827" src="https://github.com/user-attachments/assets/20b08107-4343-4ce6-beee-d73018c54da9" />
































<script><id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@4/tex-mml-chtml.js"></script>









