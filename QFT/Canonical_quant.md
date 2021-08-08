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