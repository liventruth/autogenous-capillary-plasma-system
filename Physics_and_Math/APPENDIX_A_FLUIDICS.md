Appendix A: Fluidics & Physics Validation

To validate the ACPS, engineering teams must replicate and verify the two core physical phenomena: Acoustophoresis and Hydrodynamic Cavitation.

1. Passive Acoustophoresis (Mud Separation)

The internal hopper uses corrugated metamaterial baffles. As water flows over these baffles, its kinetic energy generates an acoustic standing wave. This wave physically pushes suspended particles (mud) out of the flow stream.

The primary acoustic radiation force $F_R$ exerted on a suspended particle of volume $V_p$ in a standing wave is governed by:

$$F_R = -\left(\frac{\pi P_0^2 V_p \beta_f}{2 \lambda}\right) \phi \sin(2kx)$$

Where $\phi$ is the acoustic contrast factor, which determines whether the mud particles are pushed to the pressure nodes or anti-nodes:

$$\phi = \frac{5\rho_p - 2\rho_f}{2\rho_p + \rho_f} - \frac{\beta_p}{\beta_f}$$

In this equation:

$P_0$ is the acoustic pressure amplitude.

$V_p$ is the volume of the particle.

$\beta_f$ and $\beta_p$ are the compressibilities of the fluid and particle, respectively.

$\rho_f$ and $\rho_p$ are the densities of the fluid and particle, respectively.

$\lambda$ is the acoustic wavelength, $k$ is the wave number, and $x$ is the distance from the pressure node.

Engineering Bounty

We require fluid dynamicists to optimize the baffle geometry (pitch and depth) to maximize $F_R$ for a standard gravity-pour velocity of $0.5\text{ m/s}$, ensuring $\phi$ remains positive for standard silica-based muds.

2. Hydrodynamic Cavitation (Pathogen Rupture)

The autogenous accumulator discharges water through a Venturi nozzle, causing a massive localized pressure drop. This triggers the violent formation and collapse of micro-bubbles, generating physical shockwaves that shred extremophile cell walls.

Cavitation inception occurs when the dimensionless cavitation number $\sigma$ drops below $1.0$:

$$\sigma = \frac{P_{\text{downstream}} - P_v}{\frac{1}{2}\rho v^2}$$

In this equation:

$P_{\text{downstream}}$ is the static pressure downstream of the constriction.

$P_v$ is the vapor pressure of the liquid at operating temperature.

$\rho$ is the fluid density.

$v$ is the fluid velocity at the throat of the Venturi constriction.

Engineering Bounty

We require mechanical validation of the Venturi constriction ratio. The accumulator gas spring must generate sufficient upstream pressure to achieve a throat velocity $v$ that guarantees $\sigma < 0.8$ based on the vapor pressure $P_v$ of ambient water.
