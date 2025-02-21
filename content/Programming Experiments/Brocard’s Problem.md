---
dg-publish: "true"
---
One [[Programming Experiments|Programming Project]] I have worked on is an algorithm to solve Brocard's Problem. 

**Brocard's Problem:** 
According to Wikipedia, "Brocard's Problem is a problem in mathematics that seeks integer values of n such that n! + 1 is a perfect square, where n! is the factorial. Only three values of n are known - 4, 5, 7 and it is not known whether there are any more".
![[Pasted image 20250220163005.png]]

**My Theory**
Reverse Engineering Using $Γ^{-1}$

The factorial is a special case of the Gamma function, $n! = Γ(n+1)$. Using the inverse Gamma function $Γ^{-1}$, we can calculate $n$ from a given value. However, directly using $Γ^{-1}$ may not give integer results, so we need to verify if $n$ is an integer.

1. Start with $m = 1$ and iterate upwards.
2. Compute $m^2−1$ to find potential values of $n!$.
3. Use $Γ−1$ to compute $n$.
4. Verify if $n$ is a positive integer and satisfies $n!+1=m^2$.

**Github Repository**: [Link](https://github.com/Barkeydog/Brocards-Problem)


