---
title: "QFT"
author: "Adwait"
header-includes:
    - \usepackage{amsmath}
    - \usepackage{mathtools}
output:
    pdf_document
---

# Quantum Field Theory

# Canonical Quantisation. 

For Quantising fields using second quantisation, we follow the algorithm.

**step 1:** 

Get the Lagrangian Density $\mathcal{L}$

**step 2:**

Get the momentum and Hamiltonian density 
$$\Pi^\nu = \frac{\partial \mathcal{L}}{\partial(\partial_\nu \phi)} \\ \mathcal{H} = \Pi^0 \partial_0 \phi - \mathcal{L}$$

**step 3:**

$$[\hat{\phi}(x^\nu), \hat{\Pi}^0(y^\nu)] = i \delta ^3(x^\nu - y^\nu)$$

**Step 4:**

Expand the field in plane waves and get other operators. 
Use Wick ordering to prevent infinities. 

# Free Scalar field:

**step I:** 

$$\mathcal{L} = \frac{1}{2}((\partial_\nu \phi)^2 - m^2 \phi^2)$$

**Step II:**

$$\Pi^\nu = \partial^\nu \phi$$
$$\mathcal{H} = \frac{1}{2}(\dot{\phi}^2 + (\nabla \phi)^2 + m^2 \phi^2)$$

**Step III:**

Do the above

**Step IV:**

$$\hat{\phi}(x^\nu) = \int \frac{d^4p}{(2 \pi)^4} (\hat{a}(k_\nu) e^{ik_\nu x^\nu}+\hat{a}^{\dagger}(k_\nu)e^{-ik_\nu x^\nu}) = \int \frac{d^3p}{(2 \pi)^3 \sqrt{2 E_p}} (\hat{a}_p e^{ip.x}+\hat{a}^{\dagger}_p e^{-ip.x})$$

Where $E_p = \sqrt{p^2 + m^2}$

$$\mathcal{H} = \hat{T}\mathcal{H} = \int d^3 p E_p \hat{a}_p^\dagger \hat{a}_p$$

# Complex Scalar Field. 

**Step I:**

$$\mathcal{L}=\partial^{\nu}\psi \partial_\nu \psi - m^2 \psi^\dagger \psi $$

**Step II:**

$$\Pi^0_\psi = \partial^0 \psi,\ \Pi^0_{\psi^\dagger} = \partial^0 \psi$$
$$\mathcal{H} = \partial_0\psi^\dagger \partial_0 \psi + \nabla \psi^\dagger.\nabla \psi + m^2 \psi^\dagger \psi$$

**Step III:**

$$[\psi, \Pi^0_\psi]=[\psi^\dagger, \Pi^0_{\psi^\dagger}] = i\delta^3(x-y)$$

**Step IV:**

$$\hat{\psi}(x) = \int \frac{d^3p}{(2 \pi)^{3/2} \sqrt{2 E_p}} (\hat a_p e^{-ip.x} + \hat b_p^\dagger e^{ip.x})$$
$$\hat{\psi}^\dagger(x) = \int \frac{d^3p}{(2 \pi)^{3/2} \sqrt{2 E_p}} (\hat a_p ^\dagger e^{ip.x} + \hat b_p e^{-ip.x})$$

Where $a$ is for matter, $b$ for anti-matter. 

There is a symmetry in a phase transition. 
$$\psi \rightarrow \psi e^{i\alpha}, \ \psi^\dagger \rightarrow \psi ^\dagger e^{-i\alpha} \text{ does not change the Klein-Gordon Equation.}$$

The conserved charge is, $Q = N_{\text{anti-matter}} - N_{matter}$ which is the difference between particles and anti-particles.
