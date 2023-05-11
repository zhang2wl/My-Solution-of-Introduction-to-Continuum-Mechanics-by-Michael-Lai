# Chapter 2 Part A: Indicial Notation

## Introduction

This section covers basics about summation convention, dummy index, free index, Kronecker delta, and Permutation symbol

## Basic Concepts

### Summation and dummy index

Einstein's summation convention.

<!-- equation with equal sign aligned btween multiple lines -->
$$
\begin{equation}
  \begin{aligned}
  s &= a_1x_1 + a_2x_2 + a_3x_3 \\
    &= a_ix_i = a_jx_j = a_kx_k
  \end{aligned}
\end{equation}
$$

In Equation (1), $i, j, k$ are called dummy index because it does not matter which symbol we use. Summation convention can be used to express double sum, triple sum, and so on, for example:
$$
  \begin{equation}
    α = a_{ij}x_ix_j
  \end{equation}
$$

<div align="center" style="border: 2px solid black; background-color: #F5F5F5; padding: 10px;">
Dummy index should not apprear more than twice in a term. The following is not allowed:

$$
s = x_i y_i z_i
$$
</div>

### Free index

An index that only appears once in a term is called free index:
$$
\begin{equation}
x_i^m = a_{im}x_m
\end{equation}
$$
Unless otherwise stated, free index takes on the integral number 1, 2, and 3. Thus, Equation (3) is short hand for 3 equations:
$$
\begin{equation}
  \begin{aligned}
    x_1^m &= a_{1m}x_m \\
    x_2^m &= a_{2m}x_m \\
    x_3^m &= a_{3m}x_m
  \end{aligned}
\end{equation}
$$
If there are two free indices in an equation, then it should be the shorthand for 9 equations, for example:
$$
\begin{equation}
  T_{ij} = A_{im}A_{jm}
\end{equation}
$$
If there are three free indices in an equation, then it should be shorthand for 27 equations, and so on.

### The Kronecker Delta

The equation for Kronecker Delta is:
$$
\begin{equation}
  \delta_{ij} = \begin{cases}
                  1, & \text{if } i = j \\
                  0, & \text{otherwise}
                \end{cases}
\end{equation}
$$

### The Permutation Symbol

The permutation symbol is denoted by $ɛ_{ijk}$ and is defined by:
$$
\begin{equation}
  \varepsilon_{ijk} = \begin{cases}
  +1 & \text{if } (i,j,k) \text{ is an even permutation of } (1,2,3) \\
  -1 & \text{if } (i,j,k) \text{ is an odd permutation of } (1,2,3) \\
  0 & \text{otherwise}
  \end{cases}
\end{equation}
$$

### Indicial Notation Manipulations

1. **Substitution**
Say we have $a_i = U_{im}b_{m}$ and $b_i = V_{im}c_m$, we can substitute $b_m$ and get $a_i = U_{im}V_{mn}c_n$. This equation have two sets of dummy indices thus there are two summations. This euqation has one free index thus it represents three equations. <br>
2. **Multiplication**
If $p=a_m b_m$ and $q = c_m d_m$, thus $pq = a_m b_m c_n d_n$. It is important that dummy index should not appear more than twice in a term.
3. **Factoring**
$T_{ij} n_j - λ δ_{ij} n_j = 0$ can be factored as $(T_{ij} - λ δ_{ij}) n_j = 0$
4. **Contraction**
The operation of identifying two indices is called contraction. For example, $T_{ii}$ is the contraction of $T_{ij}$


## Conclusion

Part A of Chapter 2 covers the most basic yet very important definitions for tensors. We have learned summation notation, dummy index, free index, Kronecker Delta, Permutation symbol, and some indicial notation manipulations. 
