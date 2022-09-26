Computer sometimes makes mistakes. It would be useful for simple ways to double-check the output. Randomness can be to efficiently verify the correctness of an output.

Suppose we have a program that multiplies together monomials. Consider the problem
of verifying the following identity, which might be output by our program:

$(x + 1)(x − 2)(x + 3)(x − 4)(x + 5)(x − 6) ≡^? x^6 − 7x^3 + 25$

An easy way to verify is to check the coefficients of terms on LHS and RHS. In this example, the coefficient term of constant term does not match the coefficient of constant term on the right.

$F(x)≡G(x)$

We can verify the polynomials by converting them to their canonical forms ($\sum\limits_{i=0}^{n}c_{i}x^i$); two polynomials are equivalent if and only if all the coefficients in their canonical forms are equal.

From now on, let's assume that $F(x)$ is given as a product $F(x) = \prod_{i=1}^{d}(x-a^i)$ and $G(x)$ is given in its canonical form. 

But our approach for checking the program is to write another program that does the same thing. This approach may be fatal if it is caused by a bug which would repeat in both the programs. Also, the verification should be done in less amount of time.

Let us instead utilize randomness to obtain a faster method. 
Assume the largest exponent in $F$ and $G$ is d. The algorithm is as follows:
- Choose an integer $r$ uniformly at random in the range $[1,....100d]$
- Compute the values of $F(r)$ and $G(r)$ 
- If $F(r)\neq G(r)$, then the two polynomials are not equal and if $F(r)=G(r)$ then the two polynomials are equivalent.

This approach (calculating $F(r)$) can be done in $O(d)$ time, which is faster than calculating the canonical form of $F(r)$. But this algorithm can give you a wrong answer. For this to occur, $r$ needs to be a root of the $F(r)- G(r)=0$.  The degree of $F(r)- G(r)=0$ is no more than $d$. This means there are at least $d$ roots in $[1,....100d]$ for which this algorithm proves wrong. Therefore, the chance that the algorithm return a wrong assumption is no more than $1/100$.