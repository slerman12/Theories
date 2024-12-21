# Conclusive Disproof of Lorentz Transformation

&ensp;&ensp;&ensp; $\color{green}\mathrm{Sam \ Lerman}$

#

4 reference frames $K^{(1)}, K^{(2)}, K^{(3)}, K^{(4)}$.

$v^{(i, j)}$ is the velocity of any body stationary in reference frame $K^{(j)}$ measured by any observer stationary in reference frame $K^{(i)}$. All reference frames are moving collinearly in one dimension (the "x-axis") and stationary elsewhere.

A body at the spatial origin of reference frame $K^{(4)}$ crosses a relay station hoop stationary in reference frame $K^{(1)}$ at positions and times measured as $x^{(i)}, t^{(i)}$ respectively by a unique observer per reference frame $K^{(i)}$ stationary in that respective reference frame $K^{(i)}$ for $i \in 1, 2, 3$.

By definition of intersection, $x^{(4)} = 0$.

According to the Lorentz transformation:

$$
\begin{align}
x^{(4)} &= \mathcal{X}(\hat{x}^{(i)}, \hat{t}^{(i)}, v^{(i, 4)}) \\
t^{(4)} &= \mathcal{T}(\hat{x}^{(i)}, \hat{t}^{(i)}, v^{(i, 4)}) 
\end{align}
$$

for some $\hat{x}^{(i)}, \hat{t}^{(i)}$ in reference frame $K^{(i)}$. Due to relativity of simultaneity, $x^{(i)}$ is not necessarily $\hat{x}^{(i)}$ and $t^{(i)}$ is not necessarily $\hat{t}^{(i)}$, except when $i = 4$.

We then have

$$
\begin{align}
\mathcal{X}(\hat{x}^{(i)}, \hat{t}^{(i)}, v^{(i, 4)}) &= 0 \\
&\rightarrow \hat{t}^{(i)} = \frac{\hat{x}^{(i)}}{v^{(i, 4)}}, \quad\quad \text{(after some basic derivation via Lorentz transformation)}
\end{align}
$$

where Lorentz transformation is:

$$
\begin{align}
\mathcal{X}(X, T, V) &= \frac{X - VT}{\sqrt{1 - \frac{V^2}{c^2}}}. \\
\mathcal{T}(X, T, V) &= \frac{T - \frac{VX}{c^2}}{\sqrt{1 - \frac{V^2}{c^2}}}.
\end{align}
$$

Velocity addition formula:

$$
\begin{align}
\mathcal{V}(V, W) &= \frac{W - V}{1 - \frac{V}{c^2}W}. \\
\end{align}
$$

According to the velocity addition formula, directly derivable from the Lorentz transformation:

$$
\begin{align}
v^{(i, N)} = \mathcal{V}(v^{(i, j)}, v^{(j, N)})
\end{align}
$$

between reference frame triples $K^{(i)}, K^{(j)}, K^{(N)}$.

We therefore arrive at the following system of equations:

$$
\begin{align}
\mathcal{T}(\hat{x}^{(i)}, \hat{t}^{(i)}, v^{(i, 4)}) &= t^{(4)} \quad\quad \text{(from before)} \\
\rightarrow \mathcal{T}(\hat{x}^{(i)}, \hat{t}^{(i)}, \mathcal{V}(v^{(i, 1)}, v^{(1, 4)})) &= t^{(4)} \\
\rightarrow \mathcal{T}(\hat{x}^{(i)}, \frac{\hat{x}^{(i)}}{v^{(i, 4)}}, \mathcal{V}(v^{(i, 1)}, v^{(1, 4)})) &= t^{(4)} \quad\quad \text{(due to earlier deduction that $\hat{t}^{(i)} = \frac{\hat{x}^{(i)}}{v^{(i, 4)}}$)} \\
\rightarrow \mathcal{T}(\hat{x}^{(i)}, \frac{\hat{x}^{(i)}}{\mathcal{V}(v^{(i, 1)}, v^{(1, 4)})}, \mathcal{V}(v^{(i, 1)}, v^{(1, 4)})) &= t^{(4)}.
\end{align}
$$

Since $v^{(i, 1)}$ is known $\forall i$, subtracting this last equation $\forall i$ from each other (across all $i$) and setting them equal (since they're equal) gives us a solvable system of equations for $\hat{x}^{(i)} \ \forall i$.

$\rightarrow$ Then can solve for $\hat{t}^{(i)}$.

$\rightarrow$ Then can solve for $t^{(4)}$ (which equals $\hat{t}^{(4)}$) via Lorentz transformation from any one of the reference frames $K^{(1)}, K^{(2)}, K^{(3)}$.

$\rightarrow$ Do this for two reference frames and show that their required $t^{(4)}$, the time measured by the observer stationary in reference frame $K^{(4)}$, disagree. This is not allowed, since the prediction is of a specific measurement (which can be communicated for example via cellular communication between the reference frames). Conclusive disproof. &ensp; $\square$

$\rightarrow$ Can just plug in values numerically to show the contradiction.
