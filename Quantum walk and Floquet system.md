## 1. Boundary modes in quantum walk with AZ symmetries 
- To consider the boundary modes, we decompose the $d$ dimensional quantum walk with gapped bulk as
$$
U(\boldsymbol{k})  = U_{bulk}(\boldsymbol{k})\oplus U_{boundary}(\boldsymbol{k_\parallel}),
$$
where $U_{bulk}(\boldsymbol{k})$ determines the gapped bulk spectrum and we can define effective bulk hamiltonian $H_{bulk}(\boldsymbol{k})$ as $U_{bulk} = \exp(-iH_{bulk})$.
- The boundary modes can come from two sources. 
	1) It can come from a topologically nontrivial $U_{bulk}(\boldsymbol{k})=\prod_j U_{bulk}^{(j)}(\boldsymbol{k})$, whose classification is the same as the one for Floquet topological phases in $d$ dimension.  
	2) It can come from the nontrivial winding of $U_{boundary}(\boldsymbol{k}_\parallel)$.The classification of it can be obtained by doing ther hermitian map 
$$
  H_U = \begin{cases}
   \begin{pmatrix}
  0 & U_{boundary}\\
  U_{boundary}^\dagger & 0  
  \end{pmatrix}, & \mathrm{nonchiral}\ U_{boundary} \\ \\
\\
\Gamma U_{boundary}, & \mathrm{chiral}\  U_{boundary}.
  \end{cases}
$$
Here $H_U(\boldsymbol{k}_\parallel)$ is a gapless Hamiltonian of a $(d-1)$ dimension, and can be regarded as the boundary of a $d$ dimensional Hamiltonian in the symmetry class shifted by 1 from the symmetry class of $U_{boundary}$. Hence, the classfication of $U_{boundary}$  in $(d-1)$ dimension is the same as the classification of hermitian matrices in $d$ dimension, in the same symmetry class. This gives the same classification as obtained in 1) at a gap.

## 2. Boundary modes in quantum walk with additional crystalline symmetries 
- When considering crystalline symmetries, we have to first ask whether the boundary respect the crystalline symmetries (or is compatible with the crystalThe boundary modes can come from two sources. line symmetries). 
- To classify the boundary modes, we can still decompose the $d$ dimensional quantum walk with gapped bulk as before, with a gapped bulk and gapless edge.  The boundary modes can come from two sources. 
	1) It can originate from a topologically nontrivial bulk.  We can call these boundary modes **intrinsic**. When the boundary modes are invariant under the crystalline symmetry operation, the classification is given by the K group $K(s,t) \equiv K^{(0)}$. Here $(s,t)$ denotes the Shiozaki class, where $s$ labels the AZ symmetry and $t$ labels the crystalline symmetry.  If the boundary modes is not invariant under crystalline symmetry opertation, then the boundary modes irrespective boundary orientation is given by $\mathcal{K}'=K/K'$ , where $K'$ is the pure crystalline  subgroups that correspond to the gapless modes on symmetry invariant boundaries. 
	 2) It can also originate from $U_{boundary}$. If the boundary respect the crystalline symmetry in Shiozaki class (s,t), then $H_U$ also has the crystalline symmetry (in Ken-Shiozaki class (s-1,t)), in dimension $d-1$. The classification of $H_U$ is thus the same as the classification of hermitian matrices in $(s,t)$ class in $d$ dimension, namely given by $K(s,t)$.   If the boundary does not respect the crystalline symmetry, then with the hermitian map we obtain a hermitian matrix $H_U$ in $(d-1)$ dimension in a shifted AZ symmetry class. Which mean the classification of $U_{boundary}$ is the same as the crystalline ten-fold classification in $d$ dimension, namely $K_{TF}(s))$.
	  3) Actually the groups obtained from 1) and 2) are the same! See the appendix.  
### 2.1. Appendix: Higher-order bulk boundary correspondence
- Bulk K group series: 
$$
K^{(d)}\subseteq \dots \subseteq K''\subseteq K'\subseteq K
$$
- For example, $K$ is the usual bulk classification K group. $K^{(n)}$ is a subgroup excluding topological phases of order $n$ or lower.  $K'$  classifies pure crystalline phases.
- Boundary K group, $\mathcal{K}'$ classifies gapless codimension-1 boundary modes irrespecive of boundary orientation, as long as the boundary is compatible with symmetry. $\mathcal{K}^{(n)}$  intrinsic codimension-n modes. 


