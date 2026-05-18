Tatsuma Wada
Keio University

1. How can we generate uniform random numbers?

   (a) Set parameters $a = 1229$, $c = 351750$, $m = 1664501$, and $I_0 = 1990103011$.
   (b) Compute the remainder of $(aI_0 + c)/m$ (use, for example, a MATLAB function "mod(a*I0+c,m)")
   (c) Compute the $x_0 = \text{remainder}/m$
   (d) Set the remainder to $I_1$.
   (e) Iterate (b) to (d) 1,000 times, i.e., obtain $x_t$ and $I_t$ for $t = 1, \dots, T$ and $T = 1000$.
   (f) Make a histogram for $x$.

2. How can we generate normal random numbers from uniform random numbers?

   (a) Generate two uniform random variables $U_1$ and $U_2$.
   (b) Compute

       $$X_1 = \sqrt{-2 \log U_1} \cos(2\pi U_2)$$
