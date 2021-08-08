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

# Phonons 

Phonons are basically the normal modes in a set of coupled oscillators, 
here were take an example for 1-d chain of coupled oscillators.

$$\hat{H} = \sum_j \frac{p_j^2}{2} + \frac{1}{2} k (x_{j+1} - x_j)^2  $$

Hamiltonian of coupled oscillators can be decoupled by a fourier transform, 
the phonons are just the fourier basis.

$$\hat{x_k} = \frac{1}{\sqrt{N}} \sum_j x_j e^{-ikja}, \\ \hat{p}_k = \frac{1}{\sqrt{N}} \sum_j p_j e^{-ikja}$$

The Hamiltonian becomes, 
$$\hat{H} = \sum_k \frac{1}{2m}\hat{p}_k \hat{p}_{-k} + \frac{1}{2} m \omega_k^2 \hat{x}_k \hat{x}_{-k}, \\ = \sum_k \hbar \omega_k (\hat{a}_k \hat{a}^{\dagger}_{k} + \frac{1}{2}) \\ \omega_k = \sqrt{\frac{4k}{m}} \sin(\frac{ka}{2}) \text{ is the dispersion relation.}$$

This helps us write the field operators for position, '
$$\hat{x_j} = \frac{1}{\sqrt{N}} \sqrt{\frac{\hbar}{m}} \sum_k \frac{1}{\sqrt{2 \omega_k}} (\hat{a}_k e^{ikja} + \hat{a}^{\dagger}_k e^{-ikja})$$

This is like saying, when a point at $j$ is plucked, the field is a sum of plane waves of mode $k$. 

# Occupation number Representation 

Making Quantum mechanics relativistic requires us to discard finite particle physics, we switch to fock spaces where one can accomodate infinite particles. 


Another thing is the creation, annihlation operators have different properties based on what field you want. 

**Bosons** 

$\hat{a}_i^{\dagger}|n_1, n_2, n_3, \dots, n_i, \dots \rangle = \sqrt{n_i + 1} | n_1, n_2, n_3, \dots, n_i +1, \dots \rangle \\ \hat{a}_i |n_1, n_2, n_3, \dots, n_i, \dots \rangle = \sqrt{n_i} |n_1, n_2, n_3, \dots, n_i-1, \dots \rangle$ 

**Fermions**

$\hat{c}_i^{\dagger}|n_1, n_2, n_3, \dots, n_i, \dots \rangle = (-1)^{\sum n_i} \sqrt{n_i + 1} | n_1, n_2, n_3, \dots, n_i +1, \dots \rangle \\ \hat{c}_i |n_1, n_2, n_3, \dots, n_i, \dots \rangle = (-1)^{\sum n_i} \sqrt{n_i} |n_1, n_2, n_3, \dots, n_i-1, \dots \rangle$ 


Bosons follow canonical commutation relations, while fermions follow canonical anti-commutation relations. 
