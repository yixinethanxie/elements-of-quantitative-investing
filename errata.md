page 29, equation 2.5, the right side on the first inequality should be $1/\left(2\sqrt{2\pi}\right)$
page 83, third equal sign, $E(\epsilon^2|x) + E\left[(\hat{y} - E(y|x))^2|x\right]$
page 86, exercise 4.2 part 2, min_i {\lambda_i}^2 \leq h^2? maybe? but rayleigh-ritz theorem??
page 91, (4.28) missed {v_i}^T $${u_i}^Tu_j = \frac{{v_i}^T(A^TAv_j)}{s_is_j} = \frac{{s_j}^2{v_i}^Tv_j}{s_is_j} = \frac{s_i}{s_j}{v_i}^Tv_j = \delta_{i,j}$$
page 95, 5.1.1, loss function should be: $$\bar{L} = 1/T\sum_{t=1}^TL(\tilde{\sigma}_t^2, \hat{\sigma}_t^2)$$
page 100, exercise 5.1, H=rr^T makes the loss function -infty
page 104, exponentially weighted covariance matrix: $$\hat{\Omega}_{r,t}=\frac{1-e^{-1/\tau}}{1-e^{-T/\tau}}\sum^T_{s=1}e^{-s/\tau}r_{t-s}r_{t-s}^T$$
page 107, the condition of equal wshould be $\Omega_r \propto \hat{\Omega}_r$
page 126, the lienar approximation of short-term idio update: $e^{\hat{x}_t/2} = \kappa_0 \sum^{\infty}_{s=0} e^{-s/\tau_0} \sqrt{\frac{\sum_i a_{i,t-s}(\epsilon_{i,t-s} / \hat{\sigma}_{i,t-s})^2}{\sum_i a_{i,t-s}}}$
page 138, at bottom, should we check the correlation across $\tilde{f}_t^{(1)},\dots,\tilde{f}_t^{(q)}$? Also, the covariance matrix should be $diag(cov(g_t), cov(\tilde{f}_t^{(1)}), \ldots, cov(\tilde{f}_t^{(q)}))$?
page 153, formula 7.16 - 7.19 seems to be off, 
    \begin{align}
        \hat{B} & = U_m(S_m - \hat{\sigma}I_m)^{1/2} \\
        \hat{\sigma}^2 & = \bar{\lambda}
        \hat{B} & = U_m \\
        \Sigma_f & = S_m - \bar{\lambda}I_m \\
        \Sigma_{\epsilon} & = \bar{\lambda}I_n 
    \end{align}
page 181, exercise 7.1, the only if direction "B and C must be full-rank with rank=m"??
page 181, exercise 7.2, not sure how to prove uniqueness and (7.10)'s constraint may not be binding
    (7.7) solves for the first eigenvector (largest eigenvalue) and (7.10) solves for the second eigenvector (second largest eigenvalue). It is possible that a covariance matrix has repeated eigenvalues, and infinitely many eigenvectors, so I don't know how to prove the solution (eigenvector) uniqueness. However, the constraint being binding indicates that the lagrangian multiplier $\lambda$ must be positive, which is also the eigenvalue. Again, since a covariance matrix must be PSD, there is at least one positive eigenvalue, so (7.7) must be binding, yet the second eigenvalue may be zero.
page 184, exercise 7.10, shouldn't the gradient be: \nabla_vf &= 2Xv - 2(v^TXv)v = 2(1 - vv^T)Xv ??