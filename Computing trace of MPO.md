# Krylov method
## 1. Lanczos algorithm
### 1.1. Original Lanczos algorithm
For a given matrix $A\in\mathbb{C}^{N\times N}$ and an initial vector $u\in\mathbb{C}^N$, one iteratively build up orthonormal basis $U_{K}= \{u_{1}, u_{2}, \dots, u_{K}\}\in\mathbb{C}^{N\times K}$ of the Krylov subspace $\mathcal{KR}_{K} = \mathrm{span}(u, Au, A^{2}u, \dots, A^{K-1}u)$. Then, the projection of $A$ on $\mathcal{KR}$ , denoted as $T_K$ can be used to approximate various properties of $A$. The algorithm builds up $U_K$ and $T_K$ simultaneously,  with
$$
U_{K}^{\dagger}A U_{K}= T_K.
$$
For every $v \in \mathcal{KR}_K$, we have 
$$
v = \sum_{i = 0}^{K-1}c_{i}(A^{i}u) =\left(\sum_{i=0}^{K-1}c_{i}A^{i}\right)u = p_v(A)u
$$with $p_v(A)$ being a polynomial in $A$ of degree $K-1$. For a given analytic function $f: \mathbb{C}^{N\times N} \to \mathbb{C}^{N\times N}$ it then follows that $\exists v_{a} \in \mathcal{KR}_{K}$ for which $p_{v_a}(A)$ corresponds to a power-series approximation around $0$ of degree $K-1$ of $f(A)$ .
### 1.2. Block Lanczos algorithm
Initially consider rather than a single vector $u$, one consider a block of column vectors $U\in\mathbb{C}^{N\times M}$ with $M\leq N$. We denote $\boldsymbol{U}_K \in \mathbb{C}^{N, KM}$ as the basis consisting of $K$ basis matrices $\{U_1, U_2, \dots, U_K\}$.
Define the the inner product  and the induced norm
$$
\braket{U_i, U_j}_F = \mathrm{Tr}(U_i^\dagger U_j), \quad \| U_i\|_F = \sqrt{\braket{U_i,U_i}} 
$$
we can construct block Lanczos algorithm to obtain 
$$
\boldsymbol{U}_K^\dagger A \boldsymbol{U}_K = T_K \otimes I_M.
$$
## 2. Connection to Gauss quadrature
For any vector $u$, we have
$$
u^\dagger f(A) u = u^\dagger V_A f(\Lambda_A) V_A^\dagger u = \sum_{i=1}^N f(\lambda_i) \mu_i^2 =\int_a^b f(\lambda) d\mu(\lambda),
$$
where $V_A\Lambda_A V_A^\dagger$ is the spectral decomposition of $A$, $\mu_i = e_i^TV_A^\dagger u$, and
$$
\mu (\lambda) = \begin{cases} 0 &\mathrm{if}\  \lambda < \lambda_1 =a \\
\sum_{i=1}^j\mu_i^2  & \mathrm{if}\ \lambda_j\leq\lambda<\lambda_{j+1}\\
 \sum_{i=1}^N\mu_i^2  & \mathrm{if}\ b=\lambda_N\leq\lambda\\
\end{cases}
$$



