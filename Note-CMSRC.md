Note
=====

## Intuition of this paper
To solve challenging registration problems by maximizing the number of corresponding semantic regions - such as windows, doors or balconies.

In this work, 

1. they approximated semantic regions by ellipsoids, and leverage their convexity to formulate the correspondence search efeectively 
as a constrained optimization problem that maximizes the number of matched regions 
(which is solved by <strong>globally optimal in a Branch-and-Bound fashion </strong>).

2. they derived suitable <strong>linear matrix inequality (LMI) constraints</strong> which describe ellipsoid-to-ellipsoid assignment conditions.

## Contribution
a global optimization framework for semantic region assignment.

## Related Works 

with only local features - SfM (structure from motion) feature points

#### For Consensus Optimization
stochasitic or local methods for Consensus Maximization - RANSAC. 
These methods cannot guarantee optimum and are slow or break down entirely for outliers.

The path pruning strategy used in this work - Branch and Bound (BnB) Strategy.

To speed up the BnB optimization, Mixed Integer Programming (MIP) / A*-search are used.


#### For Specialized Registration Methods
It's a more general framework to handle almost all of transformations.

A related work:: Polygon to Ellipsoid, some known semantic correspondences needed and do not use consensus optimization.


## Definitions

#### S-Procedure
Let F1 and F2 be symmetric matrices, g1 and g2 be vectors and h1 and h2 be real numbers. Assume that there is some x0 such that the strict inequality {\displaystyle x_{0}^{T}F_{1}x_{0}+2g_{1}^{T}x_{0}+h_{1}<0} x_0^T F_1 x_0 + 2g_1^T x_0 + h_1 < 0 holds. Then the implication

{\displaystyle x^{T}F_{1}x+2g_{1}^{T}x+h_{1}\leq 0\Longrightarrow x^{T}F_{2}x+2g_{2}^{T}x+h_{2}\leq 0} x^T F_1 x + 2g_1^T x + h_1 \le 0 \Longrightarrow x^T F_2 x + 2g_2^T x + h_2 \le 0
holds if and only if there exists some nonnegative number λ such that

{\displaystyle \lambda {\begin{bmatrix}F_{1}&g_{1}\\g_{1}^{T}&h_{1}\end{bmatrix}}-{\begin{bmatrix}F_{2}&g_{2}\\g_{2}^{T}&h_{2}\end{bmatrix}}}  \lambda \begin{bmatrix} F_1 & g_1 \\ g_1^T & h_1 \end{bmatrix} - \begin{bmatrix} F_2 & g_2 \\ g_2^T & h_2 \end{bmatrix}

#### Schur Complement

#### Ellipsoid

#### Outer Ellipsoid / Inner Ellipsoid




