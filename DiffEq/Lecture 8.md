## Review of Lecture 7

$y' + ky = k \cos \omega t$

$\tilde{y} + k \tilde{y} = k e^{iwt}$

$\tilde{y} = \frac{1}{1 + \frac{\omega}{k}} e^{i(\omega t - \phi)}$

$$\mathrm{Re}\left( \tilde{y} = \frac{1}{\sqrt{ 1 + \left( \frac{\omega}{k} \right)^2 }} \right)\cos({\omega t - \phi})$$


Now we use the Cartesian Form

$\tilde{y} = \frac{1}{ 1 + i (\frac{\omega}{k}) } e^{(i \omega )t}$

$= \frac{1 - i \left( \frac{\omega}{k} \right)}{1 + \left( \frac{\omega}{k} \right)^{2}} (\cos (\omega t) + i \sin (\omega t))$
$= \frac{1}{1 + \left( \frac{\omega}{k} \right)^{2}} (\left( \cos \omega t)) + (\frac{\omega}{k} \right) \sin \omega t)$

Identity: $a \cos \theta + b \sin \theta = C \cos(\theta - \phi)$

$\phi = \tan^{-1} \frac{b}{a}$

$C = \sqrt{ a^{2}+ b^{2} }$


$$= \frac{1}{1 + \left( \frac{\omega}{k} \right)^{2}} \left( \sqrt{ 1 + \left( \frac{\omega}{k} \right)^2 } \right)\cdot \cos(\theta - \phi)$$

From here we simplify!😀👍


$Proof$: 

- $a \cos \theta + b \sin \theta = C \cos(\theta - \phi)$

$<a , b> \cdot <\cos , \sin> =|a||b|\cos\left( \theta - \tan^{-1}\left( \frac{b}{a} \right) \right)$

$\phi = \tan^{-1}\left( \frac{b}{a} \right)$

$<a , b> \cdot <\cos , \sin> =|a||b|\cos\left( \theta - \phi) \right)$      $\square$



- Complexifying

$(a - bi) (\cos(\theta) + i \sin(\theta))$


Notice $\mathrm{Re}((a - bi) (\cos(\theta) + i \sin(\theta))$

$= \sqrt{ a^{2}+ b^{2} }  e^{- i \phi}\cdot e^{i \theta}$

$= \mathrm{Re} (\sqrt{ a^{2}+ b^{2} }  e^{- i \phi}\cdot e^{i \theta}) = \sqrt{ a^{2}+ b^{2} } (\cos (\theta - \phi))$             $\square$


### Basic Linear ODE



 


