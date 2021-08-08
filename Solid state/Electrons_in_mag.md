



# Solid State

# Electrons in a Magnetic field (1)

For a Classical Electromagnetic field, with scalar and vector potentials $\phi$ and $A$. 

$E = -\nabla\phi - \frac{\partial A}{\partial t}$ , $B = \nabla \times A$.

The Lagrangian,    $L = \frac{1}{2} m \dot{x}^2 + q(\dot{x}.A - \phi)$

For, $E=0$ and  $B = B_z \hat{k}$,
$$(x(t), y(t)) = (R \sin(\omega_B(t-t_0)), R\cos(\omega_B(t-t_0)))$$ 
Using Lagrange's equation and the Legendre transformation, 
$$p = \frac{\partial L}{\partial \dot{x}} = m \dot{x} + qA \\ 
H = \frac{1}{2m}(p-qA)^2 + q\phi$$
With poisson brackets,  
$\{x_i, p_j\} = \delta_{ij}, \{x_i, x_j\}=\{p_i,p_j\} = 0$

Gauge: 
$\phi \rightarrow \phi - \frac{\partial \alpha}{\partial t}, A \rightarrow A + \nabla \alpha$

This leads to the Schrodinger's equation, 
$$i\hbar\frac{\partial \psi}{\partial t} = \frac{1}{2m} (-i\hbar\nabla - qA)^2 \psi + q\phi \psi$$
For the above case $(E =0, B = B_z \hat{k})$, 
$$H = \frac{1}{2m}(p_x^2 + (p_y-qBx)^2 + p_z^2) \\
\psi = e^{i(k_yy +k_zz)} X(x) \\
\hat{p_y}\psi = \hbar k_y \psi,  \\ \hat{p_z}\psi=\hbar k_z \psi$$

$$H = \frac{1}{2m}p_x^2 + \frac{m \omega_B^2}{2} (x-k_yl_B^2)^2$$
Where, $l_B = \sqrt{\frac{\hbar}{qB}}$

This is a harmonic oscillator, therefore the eigenvalues and eigenvectors are, 
$$E = \hbar \omega_B (n+\frac{1}{2}) + \frac{\hbar^2 k_z^2}{2m} \\ \psi_{n,k}(x,y,z) = e^{i(k_yy + k_zz)}H_n(x-k_yl_B^2)e^{-\frac{(x-k_yl_B^2)^2}{2l_B^2}}$$

These are **Landau levels**, 
There exists a large degeneracy because of dependence on $n$ and $k$. 
Say, we study a finite region on the $(x,y)$ plane., with side lengths $L_x$ & $L_y$. 
$$\psi(x,y+L_y,z) = \psi(x,y,z) \implies e^{ik_yL_y} = 1$$

and the total degeneracy,
As the $x$ direction has the whole harmonic oscillator thing, it does not have translation invariance under the gauge transform. 
So as $x = k_y l_B^2$ is where the exponent localises,   
for $0 \leq x \leq L_x \implies 0 \leq k_y \leq L_x/l_B^2$

Degeneracy for each level is, 
$\cal{N} = \frac{L_y}{2 \pi} \int_0^{L_x/l_B^2} dk = \frac{q B A}{2 \pi \hbar}$.
Where $\cal{A}$ is the area of the sample. 



<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/x-mathjax-config">
        MathJax.Hub.Config({ tex2jax: {inlineMath: [['$', '$']]}, messageStyle: "none" });
</script>
