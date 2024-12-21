> I leave my journals to my uncles. In them, is a conclusive disproof based on a system of equations. They are welcome to locate the portions dealing with that disproof, organize them, and publish. I haven't looked at any other such disproofs on the internet. I believe this one is original. But since those were ignored, the one I leave to my uncles might be too.
>
> The below is not a disproof, but contains motivating ideas.

# (Begin disproof)

More specific [here](https://github.com/animal-tree/Writing-stuff-2/blob/15b393df1213e8537faf657869ac4606a357f132/Formal%20theory/Lorentz-disproof.md).

## (time-clock version)

$$\hat{t} = T(x^{(i)}, t^{(i)}, v^{(i, N)})$$

$\forall i < N$ and $i, N \in \mathbb{N}$.

### Definitions

$\hat{t}$: The time in coordinate system $N$ that the positional origin of coordinate system $N$ intersects the position of the exact center of the relay station hoop.

$T$: The Lorentz transformation time equation: transforms the time in one coordinate system to that in another. The three components are (1) the position in the former coordinate system, (2) the time in the former coordinate system, and (3) the velocity of the latter coordinate system in the former coordinate system.

$v^{(i,j)}$: The velocity of coordinate system $j$ in coordinate system $i$.

$x^{(i)}$: The unknown position of the exact center of the relay station hoop in coordinate system $i$, at time $t^{(i)}$ in coordinate system $i$.

$t^{(i)}$: The unknown time in coordinate system $i$ that is transformed to $\hat{t}$ in coordinate system $N$ via the Lorentz transformation time equation.

### Postulate and/or physical measurement

**Absoluteness of time and location identity postulate:** The time relative to itself at which a body undergoes an intersection with any given location has one and only one value, and physically exists.

Therefore $\hat{t}$ physically exists, whether measured, measured accurately/inaccurately, or not measured.

Quantum physics considerations can be accounted for via the below mechanism of physical measurement, with perhaps some approximation error in the actual numerical measurement. One could debate whether or not the wave function truly collapsed "100%" in that case.

The body can also be constrained to be non-quantum.

**Alternatively, physical measurement:** A rocket ship, positioned at the origin of coordinate system $N$, crosses through the exact center of the relay station hoop, where the inner edges of the relay station hoop shoot photons (or electrons) inward. $\hat{t}$ can at least approximately be measured by detecting the incoming rays on a sensor of a light clock aboard that causes the light clock to stop counting, thereby yielding a measurement, or of a second light clock aboard that causes the second light clock to start counting, thereby allowing for the calculation of a measurement via subtraction. Either way, this act of measuring collapses the wave function, arguably accounting for any quantum physics considerations in the earlier postulate. 

> **In case of debate:**
>
> If not, well, this is not that hard to answer. The existing theories around the Lorentz transformation don't account for wave-functions and coherence/decoherence either.
>
> That being said, sufficient measurement accuracy can be obtained via this mechanism, by using it twice as follows: measure once via this mechanism at the initial position, perhaps incurring some measurement delay and approximation error; and then measure again via an identical mechanism at the relay station hoop. One starts at the beginning; one starts at the end; subtract the two to get the total time spanned, each accounting for the other's measurement delay and approximation error, assuming negligible randomness.
> - Since the below disproof considers motion only in the x-axis, an argument could be made that the two light clocks being adjacent rather than fixed in the same position violates this collinearity; however, the two hoops (the initiating one at the start and the relay station hoop at the end) can account for this by respectively shooting photons (or electrons) from adjacent halves of the inner edge. And if this is too disruptive, then allow there to be one such additional measuring device on each side of the first (so three light clocks in total), and average the two to get the positional average of the middle one.
> - The experiment can also be reproduced twice with the respective start and end halves flipped, then averaged across both experiment runs.
>
> If that is still yet unconvincing, consider the physical coordinate systems of Einstein: physical measuring rods and clocks. Somehow, a spacetime origin has to be defined for such a coordinate system to exist, yes? In order to do that, a mechanism is already implicitly assumed that synchronizes the two. Whatever that mechanism is, let that mechanism be this mechanism. Alternatively, let this mechanism be that mechanism, provided here for the future use of theoreticians.
>
> In any case, $\hat{t}$ measurably exists up to some extremely small precision error, and that measurement, once having collapsed the wave function, should not by any known law negate the reality of $\hat{t}$'s existence, as being in a coherent quantum state and existing, though perhaps uncertain in the highest absolute precision to the microscopes and branding irons of measurement (which, frankly, is always the case).

### Formal contradiction

Assume the Lorentz transformation equations hold between coordinate systems.

$$x' = X(x, t, v) = \frac{x - vt}{\sqrt{1 - \frac{{v}^2}{c^2}}}$$

$$t' = T(x, t, v) = \frac{t - \frac{vx}{c^2}}{\sqrt{1 - \frac{{v}^2}{c^2}}}$$

$\forall i,j \in \mathbb{N}$.

(Appending to **Definitions** <br>$X$: The Lorentz transformation position equation: transforms the position in one coordinate system to that in another. The three components are (1) the position in the former coordinate system, (2) the time in the former coordinate system, and (3) the velocity of the latter coordinate system in the former coordinate system).

Let $N = 3$.

Let coordinate system 1 and the relay station hoop be stationary relative to one another. All coordinate systems are inertial, meaning their velocities stay the same. Therefore, we have $x^{(1)}$ as a constant and it is known.

Let $x^{(1)} = 1$.

Let the relative velocities of each coordinate system be $0$ in the $y$ and $z$-axes. That is, let velocity be collinear across the coordinate systems along the $x$-axis and stationary elsewhere.

(Appending to **Definitions** <br>$\text{Relay station hoop}$: Just a hoop whose exact center is located at position 1 in coordinate system 1 and is stationary relative to coordinate system 1, orthogonal to the x-axes of coordinate systems $1, 2$, and $3$).

Since none of the coordinate systems are assumed to be simultaneous in time and they are each inertial, neither relativity of simultaneity nor acceleration enter the picture, these being the usual resolutions to special/general relativity and Lorentz transformation paradoxes.

(Next step: system of equations, and derivation of formal contradiction)

I can immediately derive $t^{(1)}$, then transform between coordinate systems using the velocity-addition formula (also directly derivable from the Lorentz transformation equations).

The flaw in this disproof, is perhaps that the Lorentz transformation's mapping of $t^{(1)}$ to $t' = T(x^{(1)}, t^{(1)}, v^{(1,2)})$ might still be non-simultaneous with the actual $t^{(2)}$ that corresponds with $\hat{t}$. Yeah, $x', t'$ in the Lorentz transformation definition don't correspond to $x^{(j)}, t^{(j)}$ in the original definitions. There's perhaps no way to obtain those from $x^{(1)}, t^{(1)}$. However, $x^{(1)}, t^{(1)}$ can be obtained, so this nevertheless does synchronize time across coordinate systems, namely between coordinate systems 1 and 3.

And if I assume isotropy and relativity, a whole disproof can be constructed from just that (noting, I already knew that, but had this postulate-free one in mind that I thought maybe I could do... and/or a position-based postulate-free version...).

---

For a coordinate system to have a velocity, it must have a position and a time.

Therefore these coordinate systems have defined positions and times.

Therefore they are not exactly coordinate systems but bodies with perspectives.

A reference frame should be thought of as an observer with a coordinate system sticking out of his/her head and that coordinate system zero-centered on the observer's eyeballs.

This almost sounds like my journal descriptions, but not quite.
