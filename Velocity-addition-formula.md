# Practice and principle

Einstein used his second postulate, the constancy of the speed of light *in vacuo* across reference frames, to derive the Lorentz transformation. This postulate states and necessitates the following:

$x$ $=$ $ct$

$\rightarrow \frac{\partial x}{\partial t} = c$

and

$x' = ct'$

$\rightarrow \frac{\partial x'}{\partial t'} = c$.

However, for pretty much all bodies described by $x$ in experiment and application, *e.g.*, an electron, the body's velocity $\frac{\partial x}{\partial t}$ is measured or presumed below the speed of light *in vacuo* constant: $\frac{\partial x}{\partial t} < c$. These use cases cannot be valid at the same time as $x$ $=$ $ct$ is necessitated by Einstein's second postulate, since $x = ct \rightarrow \frac{\partial x}{\partial t} = c$.

The Fizeau experiment, for example, one of the main corroborations of the special theory of relativity, used the velocity-addition formula on a light beam's position through a tube of flowing water, describing the light beam's position in the respective reference frames of the tube and the contained flowing water medium, with $\frac{\partial x}{\partial t} \neq c$ measured, and $\frac{\partial x'}{\partial t'} \neq c$ assumed.

Such applications of Einstein's theory can't be valid at the same time as Einstein's second postulate. The object in motion must be defined to travel at exactly the speed of light: $\frac{\partial x}{\partial t} = \frac{\partial x'}{\partial t'} = c$ by implication of Einstein's second postulate. Einstein's second postulate is necessary to his derivation of the Lorentz transformation, and the latter is necessary to the derivation of the velocity-addition formula.

## Velocity-addition formula 

In the second postulate, Einstein defined $x$ and $x'$ as spatial coordinates in two reference frames $K$ and $K'$ respectively such that the body whose position is represented by these spatial coordinates is always measured as traveling at speed $c$, independent to reference frame. Namely, he described a beam of light, *in vacuo*, emitting from the intersecting origins of the reference frames. The referent body of $x$ and $x'$ must have speed $c$ in both reference frames. Popularly, this principle is known as the "constancy of light", but mathematically it's known as $x$ $=$ $ct$ and $x' = ct'$. This principle's direct implication ($\frac{\partial x}{\partial t} = \frac{\partial x'}{\partial t'} = c$), together with the velocity-addition formula and its ubiquitous usage, will make this point for me, that there is a huge, ubiquitous misuse and misunderstanding between the theory in practice and principle.

### Deriving the velocity-addition formula 

Assume the Lorentz transformation. We have:

$\partial x' = \frac{\partial x - v \partial t}{\sqrt{1 - \frac{v^2}{c^2}}}$

$\partial t' = \frac{\partial t - \frac{v \partial x}{c^2}}{\sqrt{1 - \frac{v^2}{c^2}}}$

$\frac{\partial x'}{\partial t'} = \frac{\frac{\partial x - v \partial t}{\sqrt{1 - \frac{v^2}{c^2}}}}{\frac{\partial t - \frac{v \partial x}{c^2}}{\sqrt{1 - \frac{v^2}{c^2}}}} = \frac{\partial x - v \partial t}{\partial t - \frac{v \partial x}{c^2}} = \frac{\frac{1}{\partial t}(\partial x - v \partial t)}{\frac{1}{\partial t}(\partial t - \frac{v \partial x}{c^2})} = \frac{\frac{\partial x}{\partial t} - v}{1 - \frac{v}{c^2}\frac{\partial x}{\partial t}}$.

### Utility of the velocity-addition formula 

This commonly used formula cannot in principle be usable in combination with Einstein's second postulate since the latter requires $\frac{\partial x}{\partial t}  = \frac{\partial x'}{\partial t'} = c$ always. Substituting as such the above gives us:

$$
\begin{align}
&\frac{\partial x'}{\partial t'} = \frac{\frac{\partial x}{\partial t} - v}{1 - \frac{v}{c^2}\frac{\partial x}{\partial t}} \\
&\rightarrow c = \frac{c - v}{1 - \frac{v}{c^2}c} \\
&\rightarrow c = \frac{c - v}{1 - \frac{v}{c}} \\
&\rightarrow c(1 - \frac{v}{c}) = c - v \\
&\rightarrow c - v = c - v \\
&\rightarrow 1 = 1, \\
\end{align}
$$

rendering the formula useless.

# Formally

## Definitions

### (1) Speed of light constant *in vacuo*, reference frame, and spacetime.

Let $c \coloneqq 299,792,458$ be the speed of light constant *in vacuo*.

Reference frame $K^{(i)}$ (for any $i \in \mathbb{N}$) is a coordinate system that is in motion relative to other reference frames  $K^{(j)}$ (for any $i \neq j \in \mathbb{N}$).

Any observer stationary in reference frame $K^{(i)}$ measures the corresponding time and space coordinates of body $\mathrm{B}$, as $t^{(i)}  \in \mathbb{R}$ and $x_{t^{(i)}}^{(i)} \in \mathbb{R}$ respectively.

Since multiple measurements may be taken, let $t_k^{(i)} \in \mathbb{R}$ represent each measured constant of the variable $t^{(i)}$, where $k \in \mathbb{N}$ represents the unique index across all reference frames for each taken measurement, as measured by an observer stationary in reference frame $K^{(i)}$. 

- Generating a unique index $k$ for each measurement is easy, without even knowing previous or concurrent indices. Just generate an arbitrarily long random hash with a pseudo-random number generator. The longer, the more probabilistically secure that the random hash is unique, up to arbitrarily negligible uncertainty. Therefore all of this is still physically tangible.

Denote $\Delta x_{t^{(i)}}^{(i)} \coloneqq x_{t_\ell^{(i)}}^{(i)} - x_{t_k^{(i)}}^{(i)}$ and $\Delta t^{(i)} \coloneqq t_\ell^{(i)} - t_k^{(i)}$ as spacetime displacements when $t_k^{(i)} < t_\ell^{(i)}$ (for any $k \neq \ell \in \mathbb{N}$).

$v^{(i, j)} \in \mathbb{R}$ is the velocity of any body (including observers) stationary in $K^{(j)}$ measured by any observer stationary in $K^{(i)}$.

### (2) Lorentz transformation.

$\mathcal{X}(X, T, V) \coloneqq \frac{X - VT}{\sqrt{1 - \frac{V^2}{c^2}}}$.

$\mathcal{T}(X, T, V) \coloneqq \frac{T - \frac{VX}{c^2}}{\sqrt{1 - \frac{V^2}{c^2}}}$.

### (3) Velocity-addition formula.

$\mathcal{V}(V, W) \coloneqq \frac{W - V}{1 - \frac{V}{c^2}W}$.

## Assumptions

### (1) Lorentz transformation.

$x_{t^{(j)}}^{(j)} = \mathcal{X}(x_{t^{(i)}}^{(i)}, t^{(i)}, v^{(i, j)})$.

$t^{(j)} = \mathcal{T}(x_{t^{(i)}}^{(i)}, t^{(i)}, v^{(i, j)})$.

The Lorentz transformation describes a transformation of the body $\mathrm{B}$'s corresponding space and time coordinates across reference frames in physical spacetime.

### (2) Uniform motion, and universally chronological pair.

The body $\mathrm{B}$ travels uniformly.

In other words, $\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}}$ is constant, or equivalently, $\frac{\partial^2 x_{t^{(i)}}^{(i)}}{\partial {t^{(i)}}^2} = 0$.

Allow $t_1^{(i)} < t_2^{(i)}$. 

- Note: This implicitly assumes that *at least* two of the body $\mathrm{B}$'s positions that happen chronologically in one reference frame $K^{(i)}$ can be transformed across all other (considered) reference frames $K^{(j)}$ in physical spacetime so as to happen in the same chronological order in all other (considered) reference frames $K^{(j)}$. 
- Any two index subscripts would work, without loss of generality. $1$ and $2$ are chosen for convenience.

Since average velocity is equal to displacement over time, a necessary consequence of constant $\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}}$ is:

$\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} = \frac{\Delta x_{t^{(i)}}^{(i)}}{\Delta t^{(i)}} = \frac{x_{t_2^{(i)}}^{(i)} - x_{t_1^{(i)}}^{(i)}}{t_2^{(i)} - t_1^{(i)}}$.

<!--since the average of a constant is the constant.-->

## Theorems

### (1) Velocity-addition formula.

$\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} = \mathcal{V}(v^{(i, j)}, \frac{\partial x_{t^{(j)}}^{(j)}}{\partial t^{(j)}})$.

The velocity-addition formula describes a transformation of the body $\mathrm{B}$'s velocity across reference frames in physical spacetime.

**Proof.**

$$
\begin{align}
\quad \quad \quad \quad \quad \text{ } \text{ } \text{ } \text{ } \text{ } \frac{\partial x_{t^{(j)}}^{(j)}}{\partial t^{(j)}} &= \frac{\Delta x_{t^{(j)}}^{(j)}}{\Delta t^{(j)}} \quad\quad \text{(Assumption 2)} \\
&= \frac{x_{t_2^{(j)}}^{(j)} - x_{t_1^{(j)}}^{(j)}}{t_2^{(j)} - t_1^{(j)}} \quad\quad \text{(Assumption 2)} \\
&= \frac{\mathcal{X}(x_{t_2^{(i)}}^{(i)}, t_2^{(i)}, v^{(i, j)}) - \mathcal{X}(x_{t_1^{(i)}}^{(i)}, t_1^{(i)}, v^{(i, j)})}{\mathcal{T}(x_{t_2^{(i)}}^{(i)}, t_2^{(i)}, v^{(i, j)}) - \mathcal{T}(x_{t_1^{(i)}}^{(i)}, t_1^{(i)}, v^{(i, j)})} \quad\quad \text{(Assumption 1)}\\
\end{align}
$$

$$
\begin{align}
\quad \quad \quad \text{ } \text{ } \text{ } \text{ } \text{ } &= \frac{\Bigg(\frac{x_{t_2^{(i)}}^{(i)} - v^{(i, j)} t_2^{(i)}}{\sqrt{1 - \frac{{v^{(i, j)}}^2}{c^2}}} - \frac{x_{t_1^{(i)}}^{(i)} - v^{(i, j)} t_1^{(i)}}{\sqrt{1 - \frac{{v^{(i, j)}}^2}{c^2}}}\Bigg)}{\Bigg(\frac{t_2^{(i)} - \frac{v^{(i, j)} x_{t_2^{(i)}}^{(i)}}{c^2}}{\sqrt{1 - \frac{{v^{(i, j)}}^2}{c^2}}} - \frac{t_1^{(i)} - \frac{v^{(i, j)} x_{t_1^{(i)}}^{(i)}}{c^2}}{\sqrt{1 - \frac{{v^{(i, j)}}^2}{c^2}}}\Bigg)} \quad\quad \text{(Definition 2)}\\
\end{align}
$$

$$
\begin{align}
\text{ } \text{ } \text{ } &= \frac{\Bigg(x_{t_2^{(i)}}^{(i)} - v^{(i, j)} t_2^{(i)} - (x_{t_1^{(i)}}^{(i)} - v^{(i, j)} t_1^{(i)})\Bigg)}{\Bigg(t_2^{(i)} - \frac{v^{(i, j)} x_{t_2^{(i)}}^{(i)}}{c^2} - (t_1^{(i)} - \frac{v^{(i, j)} x_{t_1^{(i)}}^{(i)}}{c^2})\Bigg)} \\
&= \frac{\Bigg((x_{t_2^{(i)}}^{(i)} - x_{t_1^{(i)}}^{(i)}) - v^{(i, j)}(t_2^{(i)} - t_1^{(i)})\Bigg)}{\Bigg((t_2^{(i)} - t_1^{(i)}) - \frac{v^{(i, j)} (x_{t_2^{(i)}}^{(i)} - x_{t_1^{(i)}}^{(i)})}{c^2}\Bigg)} \\
&= \frac{\Delta x_{t^{(i)}}^{(i)} - v^{(i, j)} \Delta t^{(i)}}{\Delta t^{(i)} - \frac{v^{(i, j)} \Delta x_{t^{(i)}}^{(i)}}{c^2}} \quad\quad \text{(Assumption 2)} \\
&= \frac{(\frac{1}{\Delta t^{(i)}})(\Delta x_{t^{(i)}}^{(i)} - v^{(i, j)} \Delta t^{(i)})}{(\frac{1}{\Delta t^{(i)}})(\Delta t^{(i)} - \frac{v^{(i, j)} \Delta x_{t^{(i)}}^{(i)}}{c^2})} \\
\end{align}
$$

$$
\begin{align}
\quad \quad \text{ } \text{ } &= \frac{\frac{\Delta x_{t^{(i)}}^{(i)}}{\Delta t^{(i)}} - v^{(i, j)}}{1 - \frac{v^{(i, j)}}{c^2} \frac{\Delta x_{t^{(i)}}^{(i)}}{\Delta t^{(i)}}} \\
&= \frac{\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} - v^{(i, j)}}{1 - \frac{v^{(i, j)}}{c^2} \frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}}} \quad\quad \text{(Assumption 2)}\\
&= \mathcal{V}(v^{(i, j)}, \frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}}). \quad\quad \text{(Definition 3)} \quad\quad\quad \square
\end{align}
$$

## Disproofs

### (1) Joint Einstein's second postulate and velocity-addition formula usefulness.

**Disproof.**

Einstein's second postulate, the constancy of the speed of light *in vacuo* across reference frames, states: $x_{t^{(i)}}^{(i)} = ct^{(i)} \text{ } \forall i$.

$$
\begin{align}
x_{t^{(i)}}^{(i)} = ct^{(i)} &\text{ and } x_{t^{(j)}}^{(j)} = ct^{(j)}  \quad\quad \text{(Einstein's second postulate)} \\
&\rightarrow \frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} = \frac{\partial x_{t^{(j)}}^{(j)}}{\partial t^{(j)}} = c \\
&\rightarrow c = \mathcal{V}(v^{(i, j)}, c),  \quad\quad \text{(Theorem 1)}
\end{align}
$$

rendering the velocity-addition formula useless. $\square$

### (2) Joint Einstein's second postulate and below-light-speed usefulness.

**Disproof.**

In the theories of special and general relativity, Einstein's second postulate states: $x_{t^{(i)}}^{(i)} = ct^{(i)} \text{ } \forall i$.

Assume body $\mathrm{B}$ below light speed: $\frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} < c$. We obtain: 

$$
\begin{align}
&x_{t^{(i)}}^{(i)} = ct^{(i)} \quad\quad \text{(Einstein's second postulate)} \\
&\rightarrow \frac{\partial x_{t^{(i)}}^{(i)}}{\partial t^{(i)}} = c\\ 
&\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ < c,  \quad\quad \text{(Below-light-speed assumption)}
\end{align}
$$

rendering the theories of special and general relativity unusable in this scenario. $\square$

# Conclusion

- Disproofs (1) and (2) mean that none of the experimental results of the velocity-addition formula (*e.g.* Fizeau experiment) can be attributed to Einstein's second postulate or used as evidence for Einstein's second postulate, and none of the experimental results of Einstein's theories of special and general relativity, that involve the body traveling at below light speed (*e.g.* any particles with mass), can be attributed to Einstein's second postulate, from which the theories are derived. 
- It also raises the fundamental question, pertaining either to consciousness or intelligence, of how physicists didn't notice any of this ($x$ $=$ $ct$), despite the core of the disproofs following immediately from elementary-level math. The answer to that will perhaps become clear with time.
