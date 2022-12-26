# Graphical-Lasso
 Matlab implementation of the graphical Lasso model for estimating sparse inverse covariance matrix (a.k.a. precision matrix)

minimize    tr( Theta * S ) - logdet( Theta )  + ρ * || Theta ||_1

over all positive-definite and symmetric matrices Theta. S is an estimate of the covariance matrix (usually sample covariance matrix) and ρ is a regularization parameter.

I/O:
Input: sample covariance matrix S, penalty parameter ρ.
Output: the estimated precision matrix and the regularized covariance matrix.

References:
[1] Fu (1998) Penalized regression: the bridge versus the lasso. J. Comput. Graph. Stats.
[2] Friedman, et al. (2007) Sparse inverse covariance estimation with the graphical Lasso. Biostatistics.
