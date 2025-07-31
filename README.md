# Boltzmann-kinetic-theory

### Part 1: Evolving a random distribution to a Maxwell-Boltzmann distribution
The goal of the first part is to simulate a set of particles moving in 1D inside a harmonic potential, so $U(x) = \frac{1}{2}kx^2$
We start with random initial positions and velocities not at equilibrium, and evolve the system toward a Maxwell-Boltzmann distribution with the Runge-Kutta method.

### Part 2: The Langevin equation
In Part 1 we saw that the distributions for position and momentum were constantly shifting, but they were not truly in equilibrium. To make the system more realistic, we add friction and a noise term in the Langevin equation.

### Part 3: The 1D BGK Boltzmann model
Collisions between particles can be modelled with the Boltzmann equation. The BGK Bolztmann model simplifies the Boltzmann equation by relaxing the local distribution towards equilibrium.
The equation we are going to solve is: $\frac{\partial f}{\partial t} + \overrightarrow{v} \cdot \nabla_{\overrightarrow{x}} f + \frac{\overrightarrow{F}}{m} \cdot \nabla_{\overrightarrow{v}} f = -\nu (f - f_{eq})$.
