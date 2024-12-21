The "orbit" / "shell" / "energy-level" of an electron in an atom corresponds proportionally (or rather monotonically, positively increasing) with the radius of the electron's orbit away from the nucleus of the atom. Let's write that as

$$
\begin{align}
n \propto r, \quad\quad \text{(Relationship 1)}
\end{align}
$$

where $n \in \mathbb{N}$ is the energy-level, $r$ is the radius, and $\propto$ represents monotonic proportionality (monotonic meaning not necessarily linear, can be a curved monotonic proportionality, e.g. exponential, or can be linear).

According to de Broglie,

$$p = \frac{h}{\lambda}.$$

$h$ is Planck's constant.

Then:

$$\lambda = \frac{h}{p} = \frac{h}{mv},$$

since the momentum of fermions moving at non-relativistic speeds, such as electrons in atoms (which travel at less than $1$% the speed of light, according to Bohr), is $p$ $=$ $mv$, where $m$ is the mass and $v$ is the tangential velocity. 

This gives us:

$$
\begin{align}
v = \frac{h}{m\lambda}. \quad\quad \text{(First de Broglie velocity equation)}
\end{align}
$$

de Broglie also says:

$$2\pi r = \hat{n}\lambda,$$

that is, requiring the wavelength to fit into the circumference of each energy-level $\hat{n} \in \mathbb{N}$ times.

Standardly, the energy-level is assumed to be the same as the wavelength-count integer ($n$ $=$ $\hat{n}$ is standardly assumed). Sometimes $n = 2\hat{n}$ is standardly assumed (half-wavelength increments per energy-level, as atomic standing waves are often described, though somewhat contradictorily to the reasoning of de Broglie). However, when it comes to monotonic proportionality and the atomic radius proportions considered in this proof, there is no loss in generality choosing either, so let the assumed standard be $n = \hat{n}$.

We thus standardly have:

$$2\pi r = n\lambda.$$

Rewriting this equation for $\lambda$ and plugging it into the "First de Broglie velocity equation," you get:

$$v = \frac{hn}{m2\pi r}. \quad\quad \text{(Second de Broglie velocity equation)}$$

So now we have the following relationship:

$$
\begin{align}
v \propto \frac{n}{r}. \quad\quad \text{(Relationship 2)}
\end{align}
$$

Finally, according to Coulomb, the centripetal force of the orbit of the electron around the nucleus ($F_c$ $=$ $ma_c$, where $a_c$ is the centripetal acceleration) is:

$$
\begin{align}
ma_c = \frac{Kq_1q_2}{r^2}, \quad\quad \text{(Coulomb's law)}
\end{align}
$$

where $q_1, q_2$ are the charges of the electron and nucleus respectively, and $K$ is Coulomb's constant. 

Meanwhile, the centripetal acceleration of a circular orbit of tangential velocity $v$ and radius $r$ [is](https://www.britannica.com/science/centripetal-acceleration): 

$$a_c = \frac{v^2}{r}.$$

Plugging this into Coulomb's law, we get:

$$m\frac{v^2}{r} = \frac{Kq_1q_2}{r^2},$$

which gives us (by rearrangement):

$$
\begin{align}
\rightarrow v = \sqrt{\frac{Kq_1q_2}{mr}} \quad\quad \text{(Coulomb's velocity equation)}
\end{align}
$$

and subsequently a new relationship:

$$
\begin{align}
v \propto \frac{1}{r}. \quad\quad \text{(Relationship 3)}
\end{align}
$$

So we now have three necessary relationships, if all standard assumptions hold:

$$
\begin{align}
n &\propto r \quad\quad \text{(Relationship 1)} \\
v &\propto \frac{n}{r} \quad\quad \text{(Relationship 2)} \\
v &\propto \frac{1}{r} \quad\quad \text{(Relationship 3)}
\end{align}
$$

So $v$ has to decrease when $r$ increases, and $v$ has to increase when $\frac{n}{r}$ increases. In other words, velocity decreases with radius, and only *increases* with respect to the quotient of energy-level and radius. Meanwhile, energy-level increases with radius.

Since $n$ increments by integer values and $r$ is constrained by the size of an atom (in meters), $r$ has to increase much slower than $n$ [^2] since $n$ increases by 1 per energy-level and $r$ increases at much smaller fractions of 1 (in meters) per energy-level. (Call this "the reality of the radial size of an atom").

Is there a contradiction here?

When $r$ increases, $v$ must decrease (Relationship 3). Then $\frac{n}{r}$ decreases (Relationship 2). But Relationship 1 requires that $n$ increase when $r$ increases. So $\frac{n}{r}$ must be able to decrease even when $n$ and $r$ increase. How is that possible? Only if $n$ can increase slower than $r$.

Then $r$ can increase faster than $n$, which contradicts "the reality of the radial size of an atom."

That means something about the standard assumptions must be wrong. ($\square$ ?)

#

Here is a diagram of that logic:

$$
\begin{align}
\uparrow r &\implies \downarrow v \quad\quad \text{(Relationship 3)} \\
&\implies \downarrow \frac{n}{r} \quad\quad \text{(Relationship 2)} \\
&\implies (\downarrow \frac{n}{r}, \uparrow r, \uparrow n) \quad\quad \text{(Relationship 1)} \\
&\implies \text{($n$ must increase slower than $r$)} \\
&\implies \text{($r$ must increase faster than $n$)} \\
&\implies \text{(Contradiction to ``the reality of the radial size of an atom.")} \quad\quad\quad \square\text{ ?} \\
\end{align}
$$

But we can calculate the radius for each energy-level, and we do not have this contradiction, so how did the math bring us here?

Well, here is the derivation for radius $r$:

Setting equal "de Broglie's second velocity equation" to "Coulomb's velocity equation," we get:

$$
\begin{align}
\frac{hn}{m2\pi r} = \sqrt{\frac{Kq_1q_2}{mr}}.
\end{align}
$$

Then squaring both sides and dividing out shared terms:

$$
\begin{align}
\frac{h^2n^2}{m4\pi^2 r} = Kq_1q_2.
\end{align}
$$

Then solving for radius $r$:

$$
\begin{align}
r = \frac{h^2n^2}{m4\pi^2 Kq_1q_2}. \quad\quad \text{(Radius equation)}
\end{align}
$$

This equation has nothing to do with the answer, but it rounds out the equations.[^3] Answer is below:

#

So let's retrace our logic from before, hopefully with a clearer answer. When an electron jumps an energy level, its $n$ goes up by $1$. If its radius increases by a smaller proportion, then its $\frac{n}{r}$ goes up and that means, by Relationship 2, velocity $v$ goes up. So to recap, what just happened was, radius increased and velocity also increased. That's a contradiction, by Relationship 3. When radius increases, velocity should decrease, as derived directly from Coulomb's law. And that's an interesting point to note generally, that counterintuitively, velocity goes down with radius, or in other words, velocity goes down with energy-level[^4], or in yet even more counterintuitive words, kinetic energy goes down with energy-level.[^1]

But what the previous paragraph showed that's pertinent here is that the radius increasing by a smaller *proportion* than $n$ leads to a contradiction, and that's what we arrived to before, but with one mistake. 

Proportion is distinct from magnitude. So while "the reality of the radial size of an atom" definitely constrains the magnitude by which the radius $r$ can increase — it can't come anywhere near to that of $n$, which increases by 1 at each energy-level, and 1 meter  radius would be far bigger than the whole atom — it does not constrain the *proportion* increase to being smaller for radius $r$ than for energy-level $n$. So that was the mistake in the reasoning earlier, which wasn't even my original reasoning, as I remarked in earlier frustrated versions of writing this, and unfortunately distracted me from writing up my journal notes on a similar but different and somewhat larger-scope topic, as I also remarked in earlier frustrated versions of writing this — but then it's good that my mind however played those tricks on me because it's nice to have this formally written up and transcribed (the derivations I mean) since these derivations were in my journal as well, sans this exact confusion/fake-out-disproof.

So here is what the revised reasoning would look like:

$$
\begin{align}
\uparrow r &\implies \downarrow v \quad\quad \text{(Relationship 3)} \\
&\implies \downarrow \frac{n}{r} \quad\quad \text{(Relationship 2)} \\
&\implies (\downarrow \frac{n}{r}, \uparrow r, \uparrow n) \quad\quad \text{(Relationship 1)} \\
&\implies \text{($n$ must increase proportionally slower than $r$)} \\
&\implies \text{($r$ must increase proportionally faster than $n$)} \\
&\implies \text{(Not contradiction to ``the reality of the radial size of an atom.")} \quad\quad\quad \square \\
\end{align}
$$

[^2]: In magnitude, not necessarily proportion.

[^3]: The "Radius equation" definitely does agree with the logic that r must increase proportionally faster than n, specifically quadratically faster.

[^4]: One can derive this directly by plugging the "Radius equation" into Relationship 2, dividing out the shared n, and removing the coefficient constants (since those don't affect monotonicity). For reasons not specified here, the two charges q are both treated as positive, though if one of them was negative then the coefficient would affect monotonicity. That reason, summarized quickly, is that the centripetal acceleration already assumes the "negative" direction of the nuclear charge. 

[^1]: And it is like that for planetary orbits too due to the analogous derivation from Newton's law for gravitational acceleration as the one from Coulomb's law. However, the reason the "energy-level" is thought to go up (at least in the case of atomic orbits), despite kinetic energy going down, is because of the nuclear attraction having a formal increase of "potential energy" since that potential energy is conventionally negative and technically increases (goes towards 0) with greater radius (its magnitude decreases). That magnitude decrease turns out twice the kinetic energy decrease, so an energy-level "increase" is claimed, counterintuitively, despite all forces acting on the object being weaker and the velocity being slower. By this nomenclature, Pluto (or Neptune) has the highest energy-level of the planets, despite being the slowest and the least attracted to the sun.
