---
title: "QFT"
author: "Adwait"
header-includes:
    - \usepackage{amsmath}
    - \usepackage{mathtools}
output:
    pdf_document
---

# Quantum Field Theory. 

# Noether's theorem. 

For a field $\phi(x^{\nu})$, 
$$\phi(x^{\nu}) \rightarrow \phi(x^{\nu}+\lambda a^{\nu}) = \phi(x^{\nu}) + \lambda a^{\nu} \partial_{\nu} \phi(x^{\nu}) = \phi(x^{\nu}) + \lambda D \phi$$

For such a continuous transformation, will lead to a symmetry in the Langrangian.
$$\delta \cal{L} = \frac{\partial \mathcal{L}}{\partial \phi} + \frac{\partial \cal{L}}{\partial(\partial_{\nu} \phi)} \delta(\partial_{\nu} \phi)$$ 
With $\Pi^{\nu} = \frac{\partial \cal{L}}{\partial (\partial_{\nu} \phi)}$,
$$\delta \cal{L} = (\frac{\partial \cal{L}}{\partial \phi} - \partial_{\nu} \Pi^{\nu}) \delta \phi + \partial_{\nu}(\Pi^{\nu} \delta \phi) = \partial_{\nu}(\Pi^{\nu} \delta \phi)$$

With the transformation in the lagrangian being, 
$$ \partial \cal{L} = \partial_{\nu}(\Pi^{\nu}D \phi) \delta \lambda = D \phi \delta \lambda$$ 


$$ \text{Noether's theorem: } \partial_{\nu}(\Pi^{\nu}D\phi - W^{\nu}) = \partial_{\nu} J_N^{\nu} = 0  \\ \implies Q = \int dx J_N^0 \text{ is conserved.}$$

$$\text{where } \partial_{\nu}W^{\nu} = D \cal{L}$$

# Energy conservation

Energy conservation comes about when the Lagrangian is symmetric under time translation. 
Let's take a general translation in space-time. 

$$x^\nu \rightarrow x^\nu + \delta x^\nu \\ D \cal{L} = \partial(a^\nu \cal{L}) \implies W^\nu = a^\nu \cal{L}$$
$$J_N^\nu = \Pi^\nu D \phi - W^\nu = a^\nu(\Pi^\nu \partial_\nu \phi - \delta_\nu^\mu \cal{L}) = a^\nu T^{\mu\nu}$$

The conserved charge being, 
$$P^\alpha = \int d^3 x T^{0 \alpha}$$

