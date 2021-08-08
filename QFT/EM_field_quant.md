# Quantum FIeld Thoery

# Digression : EM field Quantisation. 

The Hamiltonian for the EM field is,     
$$H = \frac{(p - qA/c)^2}{2m} + q \phi$$

For a free Electromagnetic field, 
$$H_{EM} = \frac{1}{8\pi} \int d^3r (E^2 + B^2) = \frac{1}{8\pi} \int d^3r ((-\frac{1}{c}\frac{dA}{dt})^2 + (\nabla \times A)^2)$$

Using Coloumb's gauge,    
$(\nabla^2 - \frac{1}{c^2}\frac{\partial^2}{\partial t^2})A = 0$

Plain wave expansion, 
$$A(r,t) = \sum_{k,\lambda} c_{k,\lambda} \hat{\epsilon}(k,\lambda) \frac{e^{i (k.r - \omega t)}}{\sqrt{V}} + c_{k,\lambda}^* \hat{\epsilon}(k,\lambda) \frac{e^{-i (k.r - \omega t)}}{\sqrt{V}}  $$

We can now derive other observables using this, 

$$E = \frac{1}{8 \pi c^2}\int d^3r \frac{\partial A}{\partial t}.\frac{\partial A}{\partial t} \\ \\ = \frac{1}{8 \pi} \int d^3r (\sum \frac{-i \omega}{c} c_{k,\lambda} \hat{\epsilon}(k,\lambda) \frac{e^{i(k.r - \omega t)}}{\sqrt{V}}).(\sum \frac{i \omega'}{c} c'_{k',\lambda'} \hat{\epsilon'}(k',\lambda') \frac{e^{-i(k'.r - \omega' t)}}{\sqrt{V}})  \\ $$

$$H = \frac{1}{2 \pi} \sum \frac{\omega^2}{c^2} c^*_{k,\lambda}c_{k,\lambda}  $$
We can redefine some coefficients,     
$q_{k,\lambda} = \frac{1}{\sqrt{4 \pi} c}(c_{k,\lambda} + c_{k,\lambda}^*) \\ p_{k,\lambda} = -\frac{1}{\sqrt{4 \pi} c}(c_{k,\lambda} - c_{k,\lambda}^*)$

And from this we get a Hamiltonian of the form, 
$$H = \sum_{k,\lambda} (\frac{p_{k \lambda}^2}{2} + \frac{1}{2} \omega^2 q_{k, \lambda}^2)$$
This is exactly a sum of an infinite number of decoupled harmonic oscillators, we turned the maxwell equations and it's coupled hamiltonian to get this new Hamiltonian in a diagonal basis. 

The free Radiation field can now be quantised by turning the coefficients into creation and annihlation operators, 
$$c_{k,\lambda} \rightarrow c \sqrt{\frac{2 \pi \hbar}{\omega}} \hat{a}_{k,\lambda} ,  \ \ c^*_{k,\lambda} \rightarrow c \sqrt{\frac{2 \pi \hbar}{\omega}} \hat{a}^{\dagger}_{k,\lambda}$$

and the vector potential is replaced by an operator, 
$$\hat{A} = \sum c \sqrt{\frac{2 \pi \hbar}{\omega}} (\hat{a}_{k,\lambda}\epsilon(k,\lambda) \frac{e^{i(k.r - \omega t)}}{\sqrt{V}} + \hat{a}^{\dagger}_{k,\lambda}\epsilon^*(k,\lambda) \frac{e^{-i(k.r - \omega t)}}{\sqrt{V}} ) $$

And this is the essence of Quantum field theory, just like in regualar Quantum Mechanics we turn physical observables into Hermitian operators, in Quantum field theory we turn fields into field operators which act on states to create and destroy excitations. 


