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
Let F1 and F2 be symmetric matrices, g1 and g2 be vectors and h1 and h2 be real numbers. Assume that there is some x0 such that the strict inequality ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/fd0ff7103761124c95d8e2a1ec19fbd773599f4b) holds. Then the implication

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/92f6a24cb68cf7417dbf1a7117a342160d104ea4)
holds if and only if there exists some nonnegative number λ such that
![](https://wikimedia.org/api/rest_v1/media/math/render/svg/e7efec5d5b2d3382738518b7ab263798eabe63c6)
is positive semi-definite.

#### Schur Complement

#### Ellipsoid

#### Outer Ellipsoid / Inner Ellipsoid




