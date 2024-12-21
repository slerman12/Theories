# A Unified Wave Theory of Light and General Relativity

&ensp;&ensp;&ensp; $\color{green}\mathrm{Sam \ Lerman}$

#

$`N, M, L, n, m \in \mathbb{N}`$,

$`\sigma, f \in \mathbb{R}`$, 

$`\gamma_1, \gamma_2 \in [0, 1]`$,

$`\mathrm{h_x}^{(0,0,i,j)}, \mathrm{h_v}^{(0,0,i,j)} \in \mathbb{R}^3`$, 

$`\mathrm{h_\varphi}^{(0,0,i,j)} \in [0, 2\pi)`$,

$`\mathrm{h_K}^{(0,0,i,j)} = 0`$, 

$`\mathrm{h_t}^{(0,0,i,j)} = 0`$, 

$`\mathrm{p}^{(K, t-1, i)} \sim \mathbf{P}(\mathcal{W}^{(K, t-1, i)})`$ represents the $i\text{th}$ sampled particle,

$`\mathcal{W}^{(K, t-1, i)} = \langle h^{(K, t-1, i, j')} \bigm| \forall j' \in 1,2,..., M \rangle`$,

$`\mathrm{h}^{(K, t, i, j)} = \mathcal{S}_j^{(K, t, i)}`$,

$`\mathcal{S}^{(K, t, i)} = \langle b \sim \mathbf{P}(\mathcal{G}^{(K, t, i)}) \bigm| |\mathcal{S}^{(K,t,i)}| = M \rangle`$,

> [!NOTE]
> Sets, denoted by $\langle \rangle$, only contain unique elements. Also, GitHub's LaTeX doesn't support { } notation.

$`\mathcal{G}^{(K, t, i)} = \langle \hat{\mathrm{h}}^{(K,t,i,j',k')} \bigm| \forall j' \in 1, 2, ..., M, \forall k' \in 1,2, ..., L \rangle`$,

$`D(b) = \sum\limits_{q = 1}^{N+1} \mathrm{p_\omega}^{(b_\mathrm{K},b_\mathrm{t},q)}(b_\mathrm{x})`$,

$`\mathrm{p_\omega}^{(K,t-1,i)}(\cdot)`$ depends on $`\mathrm{p_x}^{(K,t-1,i)}`$ (inverse square laws and momentum, e.g., [the wavelets described here](https://github.com/animal-tree/Writing-stuff-2/blob/main/Theories/Bendy-Ball.md)),

$`\mathrm{\hat{h}_a}^{(K,t,i,j,k)} = - \nabla_{\mathrm{h_x}^{(K,t-1,i,j)}} D(\mathrm{h}^{(K,t-1,i,j)})`$,

> [!NOTE]
> Below are element-wise vector operations.

$`\mathrm{\hat{h}_\hat{v}}^{(K, t, i, j, k)} = \mathrm{h_v}^{(K, t-1, i, j)} + \mathrm{\hat{h}_a}^{(K, t,i,j,k)}`$,

$`\mathrm{\hat{h}_\mu}^{(K,t,i,j,k)} = \frac{\mathrm{\hat{h}_\hat{v}}}{\lVert \mathrm{\hat{h}_\hat{v}}^{(K,t,i,j,k)} \rVert}`$,

$`\mathrm{\hat{h}_d}^{(K,t,i,j,k)} \sim \mathbf{N}(\mathrm{\hat{h}_\mu}^{(K,t,i,j,k)}, \sigma)`$,

$`\mathbf{N}`$ is the Gaussian distribution,

$`\mathrm{\hat{h}_v}^{(K,t,i,j,k)} = \frac{\mathrm{\hat{h}_d}^{(K, t, i, j, k)} \lVert \mathrm{\hat{h}_\hat{v}}^{(K,t,i,j,k)} \rVert}{\lVert \mathrm{\hat{h}_d}^{(K,t,i,j,k)} \rVert}`$,

$`\mathrm{\hat{h}_x}^{(K,t,i,j,k)} = \mathrm{h_x}^{(K,t-1,i,j)} + \mathrm{\hat{h}_v}^{(K,t,i,j,k)}`$,

$`\mathrm{\hat{h}_K}^{(K,t,i,j,k)} = K`$, 

$`\mathrm{\hat{h}_t}^{(K,t,i,j,k)} = t`$, 

$`\mathrm{\hat{h}_\varphi}^{(K,t,i,j,k)} = \sin(ft)`$,

$`\mathrm{\hat{h}}_{\mathrm{p}^{(T)}}^{(K,t,i,j,k)} = \mathrm{h}_{\mathrm{p}^{(T)}}^{(K,t-1,i,j)}, \ \forall T \in 1, 2, ..., t - 1`$,

$`\mathrm{\hat{h}}_{\mathrm{p}^{(T)}}^{(K,t,i,j,k)} = \mathbf{N}(\mathrm{\hat{h}_d}^{(K,t,i,j,k)} \bigm| \mathrm{\hat{h}_\mu}^{(K,t,i,j,k)}, \sigma)\mathbf{B}(\mathrm{\hat{h}}^{(K,t,i,j,k)} \bigm| \mathcal{G}^{(K, t, i)})`$, when $T = t$,

> [!NOTE]
> In only the usage immediately above, $`\mathrm{\hat{h}}_{\mathrm{p}^{(t)}}^{(K,t,i,j,k)}`$ doesn't yet belong to the $`\mathrm{\hat{h}}^{(K,t,i,j,k)}`$ element of $`\mathcal{G}^{(K, t, i)}`$, since $`\mathrm{\hat{h}}_{\mathrm{p}^{(t)}}^{(K,t,i,j,k)}`$ isn't yet defined. All necessary elements of $`\mathrm{\hat{h}}^{(K,t,i,j,k)}`$ of $`\mathcal{G}^{(K, t, i)}`$ for this usage are defined.

$`\mathbf{B}(b \in H \bigm| H) = \frac{m^{(b_\mathrm{K}, b_\mathrm{t}, b_\mathrm{x})}}{\sum\limits_{g \in H} m^{(g_\mathrm{K}, g_\mathrm{t}, g_\mathrm{x})}}`$,

$`m^{(K,t,x)} = \lVert \sum\limits_{k'=1}^{L+1} \sum\limits_{j'=1}^{M+1} \sum\limits_{i'=1}^{N+1} \sum\limits_{T=0}^{\mathrm{min}(n, t)} \gamma_1^T s(x, \mathrm{\hat{h}}^{(K,t - T,i',j',k')}) \rVert`$ sums over vectors in $`[-1, 1]^2`$, then norms,

$`s(x,b) = \max(0, -f \mathrm{d}(x, b_\mathrm{x}) + 1)\langle \cos^{-1}(b_\varphi), \sin^{-1}(b_\varphi) \rangle`$ multiplies a scalar, by a vector in $`[-1, 1]^2`$,

$`\mathrm{d}(x_1, x_2)`$ is the distance between any two points $x_1, x_2$ (for example, Euclidean distance: $`\mathrm{d}(x_1, x_2) = \lVert x_1 - x_2 \rVert`$),

$`\mathbf{P}(b \in H \bigm| H) = \frac{\sum\limits_{T=0}^{\min(m, t)} \gamma_2^T b_{\mathbb{p}^{(b_\mathrm{t} - T)}}}{\sum\limits_{g \in H} \sum\limits_{T=0}^{\min(m, t)} \gamma_2^T g_{\mathbb{p}^{(b_\mathrm{t} - T)}}}`$,

$`\forall K \in \mathbb{Z}`$ with the reference frame transformations added, $`K`$ $`=`$ $`0`$ in the meantime,

$`\forall i \in 1, 2, ..., N`$, 

$`\forall j \in 1, 2, ..., M`$, 

$`\forall k \in 1,2, ..., L`$, 

and $`\forall t \in \mathbb{N}`$.

