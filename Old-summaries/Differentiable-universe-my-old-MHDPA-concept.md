> This an old summary that is outdated to my current theory.

# Differentiable universe

### Elementary particles

Particle $i \in 0, ..., N$ is defined by position $x^{(i)}$, velocity $v^{(i)}$, spin $\varsigma^{(i)}$, token $\tau^{(i)}$, $\in \mathbb{R}^d$ for number spatial dimensions $d \in \mathbb{N}$. As well as measurement (collision/interaction) score $k^{(i)} \in \mathbb{R}$.

$p^{(i)} = (x^{(i)}, v^{(i)}, \varsigma^{(i)}, \tau^{(i)}, k^{(i)})$.

$\tau$ belongs to one of $M$ quantized learnable elementary particle tokens.

### Differentiable physics

The following equations differentiably simulate a 1-time-step transition capable of differentiating effects 1 collision in $d+1$ spacetime beyond present moment.

$v^{(i)}_{t+1} = \text{MLP}_2(v^{(i)}_t + \text{MLP}_1(\sum\limits_j \frac{1}{\lVert x^{(i)} - x^{(j)} \rVert} \text{Linear}(v^{(j)}_t:\varsigma^{(j)}_t:\tau^{(j)}_t)))$.

$x_{t+1}^{(i)} = x_t^{(i)} + v_{t+1}^{(i)}$.

where $:$ represents concatenation.

This operation is identical to single-head dot-product attention with inverse Euclidean distance substituting the key-query dot-product attention.

### Sparsely localized collisions

To make the collisions more sparsely localized, we can use re-parameterization to only aggregate the immediately-proximal particles:

$$
\Gamma_t^{(i,j)} = \begin{dcases}
        1 & \lVert x_t^{(i)} - x_t^{(j)} \rVert \leq \epsilon \\
        0 & \text{else} \\
\end{dcases}
$$

$\hat{v_{t+1}}^{(i)} = \text{MLP}_2(v^{(i)}_t : \text{MLP}_1(\sum\limits_j \Gamma_t^{(i,j)} \frac{1}{\lVert x^{(i)} - x^{(j)} \rVert} \text{Linear}(v^{(j)}_t:s^{(j)}_t:\tau^{(j)}_t)))$.

$v_{t+1}^{(i)} \leftarrow v_{t+1}^{(i)} + \varphi(\hat{v_{t+1}}^{(i)} - v_{t+1}^{(i)})$

within some collision distance region $\epsilon \in \mathbb{R}$. 

$\varphi$ is the re-parameterization stop-grad operator.

Note: More precisely, the inner sum should be re-parameterized before the application of the first MLP layer. Some of these layers can be LayerNorm'd as well as per Transformer-convention.

### Supervised learning of density region and trajectory simulation

Given a subset of particles $L \subseteq 0, ..., N$ (e.g. all particles of a given elementary particle token), we can optimize their trajectory along a centroid path $\ell_0, ..., \ell_{T-1} \in \mathbb{R}^d$ for some number time steps $T \in \mathbb{N}$ with the following supervision objective:

$\max\limits_{\forall i \in L} \mathcal{N}(x_t^{(i)}, 1)(\ell_t)$

where $\mathcal{N}$ is the Normal distribution.

### Variational velocity

We can overcome the local-optima limitations of instantaneous derivatives with variational inference, capable of simulating via randomness non-local trajectories beyond just the immediate collision horizon:

$\mathrm{v} \sim \mathcal{N}(v_{t+1}^{(i)}, 1)$.

$v_{t+1}^{(i)} \leftarrow v_{t+1}^{(i)} + \varphi(\mathrm{v} - v_{t+1}^{(i)})$.

### Wave-particle duality

We can extend this to many branching wave-like particle simulations capable of simulating non-local longer-term trajectories over the course of many collisions, far beyond the reach of ordinary gradient-based optimization, via wave-particle duality, using "measurement score" $k^{(i)}$ to control the scattering and collapsing of particles into waves and measured points via iterative creation and truncation.

This is a proposed simplified model for wave-particle duality, compatible with the observations of the double-slit experiments that shall be theorized herein to govern optimization mechanisms of the actual universe's mechanics. This theory of a universe-optimizer-God will be called "the Theory of Naturalistic Intelligence". Our empirical finding is that wave-particle duality, as defined and proposed, is conducive to optimization.[^1]

To start, we will index particles with a second set of particles per the original defined:

$p^{(i,j)} = (x^{(i,j)}, v^{(i,j)}, \varsigma^{(i,j)}, \tau^{(i,j)}, k^{(i,j)})$.

At each time step, $x^{(i)}$ will be sampled categorically w.r.t. $k^{(i,j)}$ as a multinomial distribution via softmax'ing over the $j\text{th}$ dimension, initialized as $k^{(i,j)}_0 = 1$ and updated with each time increment according to the following entangling rule:

$k^{(i,j)}_{t+1} = k^{(i,j)}_t + \sum\limits_b \Gamma_t^{(a,b)} \frac{1}{\lVert x^{(a)} - x^{(b)} \rVert}$

Furthermore, multiple velocities will be sampled:

$\mathrm{v_\mathit{\omega}} \sim \mathcal{N}(v_{t+1}^{(i)}, 1)$,

where $\omega \in 0, ..., H-1$ indexes the $H \in \mathbb{N}$ "heads".

Then before the application of the first MLP layer, the top $K$ heads per particle $i$ will be selected and the rest truncated via the Gumbel-softmax trick w.r.t. $k^{(i,j)}_{t}$.

### Time quanta, non-locality, inertia, conservation laws, incrementalism

Additional inductive biases may be applied and the conduciveness of other universe phenomena to optimization may also be empirically evaluated.

### Differentiable gravity

It's too bad I didn't have time to elaborate on differentiable gravity.

To run this experiment, we may use a differentiable learned algorithm or a classical description.

Simply put, two randomly positioned "particles" in a batch of random initializations are optimized, within a swarm of surrounding dark matter, to converge to follow a defined trajectory in accord with the laws of physical gravity.

Next, we can describe electromagnetism, by picking a dense field of light particles and another dense field of light particles, both surrounded by dark particles and optimize for their convergence and divergence in position along the attractive and repulsive directions respectively.

The learned local interactions of the model can give us a classical description of quantum gravity. Meanwhile, a symbolic one can be imagined: dark particles of spin A having no effect on light particles; dark particles of spin B having an effect on light particles. Then, whose dark matter is of spin A and whose dark matter is of spin B depends on whether an interaction has occured with a light particle. If it has, it collides, bounces, and propogates as a wave spin B. With each collision between dark matter, that spin B can diminish according to an inverse square law. 

As for electromagnetism, this operation and interaction would likely require a simulation to explain, since it most likely depends on the orbit-like rotation and revolution pattern of particle systems, as they interact, in the same way, with dark matter.

We thus obtain through complex systems of potentially just two token IDs, quantum-defined, local properties of gravity and electromagnetism, and potentially more advanced "elementary" particles.

[^1]: Not yet. in progress..
