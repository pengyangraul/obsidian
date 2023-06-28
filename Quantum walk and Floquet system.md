## Boundary modes in quantum walk with AZ symmetries 
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
  \end{pmatrix}, & \mathrm{nonchiral}\ U_{boundary} \\
\Gamma U_{boundary}, & \mathrm{chiral}\  U_{boundary}.
  \end{cases}
$$
			Here $H_U(\boldsymbol{k}_\parallel)$ is a gapless Hamiltonian of a $(d-1)$ dimension, and can be regarded as the boundary of a $d$ dimensional Hamiltonian in the symmetry class shifted by 1 from the symmetry class of $U_{boundary}$. Hence, the classfication of $U_{boundary}$  in $(d-1)$ dimension is the same as the classification of hermitian matrices in $d$ dimension, in the same symmetry class. This gives the same classification as obtained in 1) at a gap.
   
## Boundary modes in quantum walk with additional crystalline symmetries 


## Bulk and intrinsic boundary modes
- Bulk K group series: 
$$
K^{(d)}\subseteq \dots \subseteq K''\subseteq K'\subseteq K
$$
- For example, $K$ is the usual bulk classification K group. $K^{(n)}$ is a subgroup excluding topological phases of order $n$ or lower.  $K'$  classifies pure crystalline phases.
- Boundary K group, $\mathcal{K}'$ classifies gapless codimension-1 boundary modes irrespecive of boundary orientation, as long as the boundary is compatible with symmetry. $\mathcal{K}^{(n)}$  intrinsic codimension-n modes. 

