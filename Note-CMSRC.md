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

#### Schur Complement

#### Ellipsoid

#### Outer Ellipsoid / Inner Ellipsoid




