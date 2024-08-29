## Complex Numbers

### Some Useful Identities and Definitions

- Polar Form($\alpha$) of $a + bi$ is $re^{i \theta}$ , such that $\tan \theta = \frac{b}{a}$ and $r = \sqrt{ a^{2}+ b^{2} }$. $r$ is called the modulus, abbreviated as $abs(\alpha)$. $\theta$ is called the $argument$, sometimes abbreviated by $arg(\alpha)$.

- $$a + b_{i} = r\cos \theta + i \sin \theta = r(\cos \theta + i\sin \theta)$$

- $$e^{i \theta} = \cos \theta + i \sin \theta$$
This is the definition of $e^{i \theta}$ made by *Euler*.

Why is this definition useful?🤔

- It satisfies the law of exponents
- It satisfies $\frac{dy}{dt} = ay$ and $y(0) = 1$. In fact, it is the only function that satisfies this differential equation.

Verify: 

$e^{i \theta_{1}} \cdot e^{i \theta_{2}} = e^{i(\theta_{1} + \theta_{2})}$


*Proof*: $e^{i \theta_{j}} = \cos \theta_{j} + i\sin \theta_{j}$

Thus, 
$e^{i \theta_{1}} \cdot e^{i \theta_{2}} = (\cos \theta_{1} + i\sin \theta_{2})(\cos \theta_{1} + i\sin \theta_{2})$
$= \cos(\theta_{1} + \theta_{2}) + i\sin(\theta_{1} + \theta_{2})$

$= e^{i(\theta_{1} + \theta_{2})}$


✋**Pause**: $\theta$ is real but the output from $e^{i \theta}$ is a complex value. So $e^{i\theta}$ is a *complex valued function* of a *real variable*.

Generally: Such a function can be defined as $u(t) + iv(t)$

$$D(u + iv) = Du + iDv(t)$$

$\frac{d}{d\theta} e^{i \theta} = i e^{i \theta}$

*Proof*: $\frac{d}{dt} e^{it} = \frac{d}{dt} (\cos t + i\sin t)$

$= -\sin t + i \cos t$
$= i(\cos t + \sin t) = ie^{it}$

 For $t = 0$,

$e^{i\cdot 0} = \cos(0) + i\sin(0) = 1$

Note: There's an argument that you can't just multiply the exponents(i.e. $i \cdot 0 = 0$) to simplify the calculation. Although I have no clue as to why?💀

--------------------------------------------------------------------------
### Advantage of Polar Form

- It's good for multiplication!
	Because you just multiply the moduli and use the exponential law on the arguments.

*Intuition*: Geometrically, the result of multiplying two complex numbers is the product of the moduli and the sum of the arguments. 👍


Example: 
- $\int e^{-x} \cos x dx$

Remember the hectic integration by parts way of doing this? Well you don't have to use that anymore??😬

$= e^{-x} \cos x$  is the **real** part of $e^{-x + ix} = \mathrm{Re}(e^{(-1 + i)x})$

This procedure is called **complexifying**(🥴) the integral.

$= \int e^{(-1 + i)x} dx = \frac{e^{(-1 + i)x}}{-1 + i}$

But we just want the real part of this integral.

$\frac{e^{(-1 + i)x}}{-1 + i} =  \frac{1}{-1 + i} e^{-x}(\cos x + i\sin x)$

$= \frac{-1 -i}{2} e^{-x}(\cos x + i\sin x)$

Now, we pick out the real parts of this.

$\mathrm{Re}(\frac{-1 -i}{2} e^{-x}(\cos x + i\sin x))$

$= \frac{e^{-x}}{2}(-\cos x + \sin x)$

and we're done!


--------------------------------------------------------------------------

### Extraction of Complex Roots


*PROBLEM*: We want to find the $nth$ root of 1: $n\sqrt{1}$

In the real domain there are mostly two answers depending on whether $n$ is even or odd.

In the complex domain there are n answers. To find the $nth$ root in this domain, consider the unit circle. 

$\alpha = \frac{2 \pi}{n}$ , $r=1$ and $\zeta = e^{i \cdot \frac{2\pi}{n} }$

Geometrically, $\zeta$ is the $nth$ root of 1. To verify, you can raise it to the $nth$ exponent. Hence $\zeta^{5}= e^{i \cdot 2\pi}$. But $2\pi = 0$ so $\zeta^{5}=1$


