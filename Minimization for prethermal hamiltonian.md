# 1. Evaluating the cost function
Consider a time periodic unitary $P(t) = P(t+T)$, we introduce the transformed time-dependent Hamiltonian 
$$
\mathcal{H}(t) = P^{\dagger(t)}H(t)P(t)- iP^\dagger(t)\dot{P}(t).
$$
We introduce the cost function
$$
F[P] = \frac{1}{T}\int_0^T dt\, \mathrm{Tr}\left(\mathcal{H - }^2\right).
$$
To evaluate the cost function, we introduce the following algorithm.
- Consider discrete times $t_1\equiv 0 , t_1, \dots,t_{N-1}, t_N\equiv T$. 
- At each time $t_i$, parametrize $H(t_i)$ as an MPO.
- Parametrize $P(t_i) = P_e(t_i)P_o(t_i)$, in which both $P_e$ and $P_o$ are products of commuting two-local operations.
- Since $\dot{P}=\dot{P}_e P_o + P_e \dot{P}_o$, we have 
$$
-iP^\dagger \dot{P} = P_o^\dagger P_e^\dagger \dot{P}_e P_o
$$