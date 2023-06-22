# Sociology-of-Rats
In a population of interacting individuals, for instance **_rats_** in a cage, the mood of one individual can influence the others. Moreover, a collective behaviour can emerge if the interactions are sufficiently numerous, for instance if the density of the rats gets sufficiently large.

A simple model for studying this phenomenon considers a population of individuals (rats!) which can be either _calm_ or _nervous_.

The rats leave in a two-dimensional grid and each rat moves randomly from site to site.

At each time step a rat moves to a nearest-neighbour site, chosen randomly.
Two rats cannot occupy the same site, hence if no free site is available nearby, the rat does not move.

At each step the rat checks the state of the neighbouring rats in the neighbouring site: if they are all calm, the rat becomes calm. If any is nervous, the rat gets nervous as well. Moreover, with a small probability $p$, at each step a rat can become nervous spontaneously.

It can be proven that the fraction of nervous rats in the population undergoes a _phase transition_ driven by the density $\rho$ of rats in the lattice: below a certain _critical value_ $\rho_c$ the fraction of nervous rats is small (in fact it would be zero on an infinitely large lattice). Raising the density of rats above $\rho_c$, the fraction of nervous rats increases abruptly.
