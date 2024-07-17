### Section 3.3
#### Q17

Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $u=e^rt.$
$$u=e^{rt}\quad\to\quad u'=re^{rt}\quad\to\quad u''=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$5(r^2e^{rt})+2(re^{rt})+7(e^{rt})=0$$

$$5r^2+2r+7=0$$
$$r=\frac{-2\pm\sqrt{4-4(5)(7)}}{2(5)}=\frac{-2\pm\sqrt{-136}}{10}=\frac{-2\pm2i\sqrt{34}}{10}=-\frac15\pm i\frac{\sqrt{34}}5$$
$$r=\left\{-\frac15-i\frac{\sqrt{34}}5,-\frac15+i\frac{\sqrt{34}}5\right\}$$
Two solutions to the ODE are $u=e^(-1/5-i\sqrt{34}/5)t$ and $u=e^(-1/5+i\sqrt{34}/5)t$, so the general solution is a linear combination of the two.

$$\begin{aligned}u(t)&=C_1e^{-(1/5-i\sqrt{34}/5)}+C_2e^{-(1/5+i\sqrt{34}/5)t}\\&=C_1e^{-t/5-i\sqrt{34}/5}+C_2e^{-t/5+i\sqrt{34}/5}\\&=C_1e^{-t/5}e^{-i\sqrt{34}/5}+C_2e^{-t/5}e^{-i\sqrt{34}/5}\\&=C_1e^{-t/5}\left[\cos\left(-\frac{\sqrt{34}}{5}t\right)+i\sin\left(-\frac{\sqrt{34}}{5}t\right)\right]+C_2e^{-t/5}\left[\cos\left(\frac{\sqrt{34}}{5}t\right)+i\sin\left(\frac{\sqrt{34}}{5}t\right)\right]\\&=C_1e^{-t/5}\left[\cos\left(\frac{\sqrt{34}}{5}t\right)-i\sin\left(\frac{\sqrt{34}}{5}t\right)\right]+C_2e^{-t/5}\left[\cos\left(\frac{\sqrt{34}}{5}t\right)+i\sin\left(\frac{\sqrt{34}}{5}t\right)\right]\\&=C_1e^{-t/5}\cos\left(\frac{\sqrt{34}}{5}t\right)-iC_1e^{-t/5}\sin\left(\frac{\sqrt{34}}{5}t\right)+C_2e^{-t/5}\cos\left(\frac{\sqrt{34}}{5}t\right)+iC_2e^{-t/5}\sin\left(\frac{\sqrt{34}}{5}t\right)\\&=(C_1+C_2)e^{-t/5}\cos\left(\frac{\sqrt{34}}{5}t\right)+(-iC_1+iC_2)e^{-t/5}\sin\left(\frac{\sqrt{34}}{5}t\right)\end{aligned}$$
Using $C_3$ for $C_1+C_2$ and $C_4$ for $-iC_1+iC_2$, the real general solution is
$$u(t)=C_3e^{-t/5}\cos\left(\frac{\sqrt{34}}{5}t\right)+C_4e^{-t/5}\sin\left(\frac{\sqrt{34}}{5}t\right).$$

Take a derivative of it.
$$\begin{aligned}u'(t)&=-\frac{C_3}5e^{-t/5}\cos\left(\frac{\sqrt{34}}5t\right)-C_3\frac{\sqrt{34}}5e^{-t/5}\sin\left(\frac{\sqrt{34}}5t\right)\\&-\frac{C_4}5e^{-t/5}\sin\left(\frac{\sqrt{34}}5t\right)+C_4\frac{\sqrt{34}}5e^{-t/5}\cos\left(\frac{\sqrt{34}}5t\right)\end{aligned}$$
Apply the initial conditions now to determine $C_{3}$ and $C_{4}.$
$$\begin{aligned}u(0)&=C_3=2\\u'(0)&=-\frac{C_3}5+C_4\frac{\sqrt{34}}5=1\end{aligned}$$
Solving this system of equations yields $C_3=2$ and $C_4=7/\sqrt{34}.$ Therefore,
$$u(t)=2e^{-t/5}\cos\left(\frac{\sqrt{34}}{5}t\right)+\frac{7}{\sqrt{34}}e^{-t/5}\sin\left(\frac{\sqrt{34}}{5}t\right).$$

![](https://img.simpletex.net/pdf/BzBdZgAc/flR4QEuvIxFfpWqpzt7eVkbtOWW22stYA.png)


Based on the graph, the smallest time for which the amplitude is 0.1 or less is $t\approx14.5.$



#### Q18

$\underline{\text{Part }(\mathrm{a})}$


Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y'=re^{rt}\quad\to\quad y''=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2e^{rt}+2(re^{rt})+6(e^{rt})=0$$

$$r^2+2r+6=0$$
$$r=\frac{-2\pm\sqrt{4-4(1)(6)}}{2(1)}=\frac{-2\pm\sqrt{-20}}2=\frac{-2\pm2i\sqrt{5}}2=-1\pm i\sqrt{5}$$
$$r=\{-1-i\sqrt{5},-1+i\sqrt{5}\}$$
Two solutions to the ODE are $y=e^(-1-i\sqrt{5})t$ and $y=e^(-1+i\sqrt{5})t$, so the general solution is a

linear combination of the two.
$$\begin{aligned}y(t)&=C_1e^{(-1-i\sqrt{5})t}+C_2e^{(-1+i\sqrt{5})t}\\&=C_1e^{-t-i\sqrt{5}t}+C_2e^{-t+i\sqrt{5}t}\\&=C_1e^{-t}e^{-i\sqrt{5}t}+C_2e^{-t}e^{i\sqrt{5}t}\\&=C_1e^{-t}[\cos(-\sqrt{5}t)+i\sin(-\sqrt{5}t)]+C_2e^{-t}[\cos(\sqrt{5}t)+i\sin(\sqrt{5}t)]\\&=C_1e^{-t}[\cos(\sqrt{5}t)-i\sin(\sqrt{5}t)]+C_2e^{-t}[\cos(\sqrt{5}t)+i\sin(\sqrt{5}t)]\\&=C_1e^{-t}\cos(\sqrt{5}t)-iC_1e^{-t}\sin(\sqrt{5}t)+C_2e^{-t}\cos(\sqrt{5}t)+iC_2e^{-t}\sin(\sqrt{5}t)\\&=(C_1+C_2)e^{-t}\cos(\sqrt{5}t)+(-iC_1+iC_2)e^{-t}\sin(\sqrt{5}t)\end{aligned}$$
Using $C_{3}$ for $C_1+C_{2}$ and $C_4$ for $-iC_1+iC_{2}$, the real general solution is
$$y(t)=C_3e^{-t}\cos(\sqrt{5}t)+C_4e^{-t}\sin(\sqrt{5}t).$$
Take a derivative of it.
$$y'(t)=-C_3e^{-t}\cos(\sqrt{5}t)-\sqrt{5}C_3e^{-t}\sin(\sqrt{5}t)-C_4e^{-t}\sin(\sqrt{5}t)+\sqrt{5}C_4e^{-t}\cos(\sqrt{5}t)$$

Apply the initial conditions now to determine $C_{3}$ and $C_{4}.$
$$\begin{aligned}y(0)&=C_3=2\\y'(0)&=-C_3+\sqrt{5}C_4=\alpha\end{aligned}$$
Solving this system of equations yields $C_3=2$ and $C_4=(\alpha+2)/\sqrt{5}.$ Therefore
$$y(t)=2e^{-t}\cos(\sqrt{5}t)+\frac{\alpha+2}{\sqrt{5}}e^{-t}\sin(\sqrt{5}t).$$
$\underline{\text{Part }(\mathrm{b})}$

Set $y=0$ and $t=1$ in the result of part (a) and solve for $\alpha.$
$$0=2e^{-1}\cos\sqrt{5}+\frac{\alpha+2}{\sqrt{5}}e^{-1}\sin\sqrt{5}$$
$$\begin{aligned}\frac{\alpha+2}{\sqrt{5}}e^{-1}\sin\sqrt{5}=-2e^{-1}\cos\sqrt{5}\end{aligned}$$
$$(\alpha+2)\sin\sqrt{5}=-2\sqrt{5}\cos\sqrt{5}$$
$$\alpha+2=-2\sqrt5\frac{\cos\sqrt5}{\sin\sqrt5}$$
$$\begin{aligned}\alpha&=-2-2\sqrt{5}\frac{\cos\sqrt{5}}{\sin\sqrt{5}}\\&=-2\left(1+\sqrt{5}\frac{\cos\sqrt{5}}{\sin\sqrt{5}}\right)\\&=-2(1+\sqrt{5}\cot\sqrt{5})\\&\approx1.51.\end{aligned}$$
$\underline{\text{Part }(\mathrm{c})}$

Set $y=0$ in the result of part (a) and solve for $t.$
$$0=2e^{-t}\cos(\sqrt{5}t)+\frac{\alpha+2}{\sqrt{5}}e^{-t}\sin(\sqrt{5}t)$$
$$0=2\cos(\sqrt{5}t)+\dfrac{\alpha+2}{\sqrt{5}}\sin(\sqrt{5}t)$$
$$\begin{aligned}\frac{\alpha+2}{\sqrt{5}}\sin(\sqrt{5}t)=-2\cos(\sqrt{5}t)\end{aligned}$$
$$\tan(\sqrt{5}t)=-\frac{2\sqrt{5}}{\alpha+2}$$
$$\sqrt{5}t=\tan^{-1}\left(-\frac{2\sqrt{5}}{\alpha+2}\right)+n\pi $$
To obtain the smallest positive value of $t$,we choose $n=1.$
$$\sqrt{5}t=\tan^{-1}\left(-\dfrac{2\sqrt{5}}{\alpha+2}\right)+\pi $$
Therefore,
$$t_{\min}=\frac{1}{\sqrt{5}}\left(-\tan^{-1}\frac{2\sqrt{5}}{\alpha+2}+\pi\right).$$
$\underline{\text{Part }(\mathrm{d})}$

Take the limit of $t_\mathrm{min}$ as $\alpha\to\infty.$
$$\begin{aligned}\operatorname*{lim}_{\alpha\to\infty}t_{\mathrm{min}}&=\lim_{\alpha\to\infty}\frac{1}{\sqrt{5}}\left(-\tan^{-1}\frac{2\sqrt{5}}{\alpha+2}+\pi\right)\\&=\frac1{\sqrt{5}}(-\tan^{-1}0+\pi)\\&=\frac\pi{\sqrt{5}}\\&\approx1.40\end{aligned}$$


#### Q31


$$t^2y''+7ty'+10y=0$$
Since this is an Euler equation, the solution is of the form $y=t^r.$
$$y=t^r\quad\to\quad y'=rt^{r-1}\quad\to\quad y''=r(r-1)t^{r-2}$$
Substitute these expressions into the ODE.
$$t^2[r(r-1)t^{r-2}]+7t(rt^{r-1})+10t^r=0$$
$$r(r-1)t^r+7rt^r+10t^r=0$$

$$r(r-1)+7r+10=0$$
$$r^2+6r+10=0$$
$$r=\frac{-6\pm\sqrt{36-4(1)(10)}}2=\frac{-6\pm\sqrt{-4}}2=\frac{-6\pm2i}2=-3\pm i$$
$$r=\{-3-i,-3+i\}$$
$\begin{aligned}\text{Two solutions to the ODE are }y=t^{-3-i}\text{ and }y=t^{-3+i},\text{ so the general solution is a linear}\\\text{combination of the two ar}\\y(t)&=C_5t^{-3-i}+C_6t^{-3+i}\\&=C_5t^{-3}t^{-i}+C_6t^{-3}t^{-3}\\&=C_5t^{-3}e^{\ln t^{-i}}+C_6t^{-3}e^{\ln t^{i}}\\&=C_5t^{-3}e^{(-i)\ln t}+C_6t^{-3}e^{(i)\ln t}\\&=C_5t^{-3}[\cos(-\ln t)+i\sin(-\ln t)]+C_6t^{-3}[\cos(\ln t)+i\sin(\ln t)]\\&=C_5t^{-3}[\cos(\ln t)-i\sin(\ln t)]+C_6t^{-3}[\cos(\ln t)+i\sin(\ln t)]\\&=C_5t^{-3}[\cos(\ln t)-iC_5t^{-3}\sin(\ln(\ln t)+C_6t^{-3}\cos(\ln t)+iC_6t^{-3}\sin(\ln t)\\&=(C_5+C_6)t^{-3}\cos(\ln t)+(-iC_5+iC_6)t^{-3}\sin(\ln t)\\\text{Using }C_7\text{ for }C_5+C_6\text{ and }C_8\text{ for }-iC_5+iC_6\text{, the real general solution is}\\y(t)=C_7t^{-3}\cos(\ln t)+C_8t^{-3}\sin(\ln t).\end{aligned}$

#### Q 32
$$
\begin{aligned}
&\text{Eq.~(i)~is} \\
&\quad\begin{aligned}y'' + p(t)y' + q(t)y = 0.\end{aligned}&& \text{(i)} \\
&\text{Note:} \\
&\quad\begin{aligned}\frac{dy}{dt}\end{aligned} && = \frac{dy}{dx} \frac{dx}{dt} \\
&\quad\begin{aligned}\frac{d^2 y}{dt^2}\end{aligned} && = \frac{d}{dt}\left(\frac{dy}{dt}\right) \\
&\quad && = \frac{d}{dt}\left(\frac{dy}{dx}\frac{dx}{dt}\right) \\
&\quad && = \frac{d}{dt}\left(\frac{dy}{dx}\right)\frac{dx}{dt} + \frac{dy}{dx}\frac{d}{dt}\left(\frac{dx}{dt}\right) \\
&\quad && = \frac{dx}{dt}\frac{d}{dx}\left(\frac{dy}{dx}\right)\frac{dx}{dt} + \frac{dy}{dx}\frac{d^2 x}{dt^2} \\
&\quad && = \frac{d^2 y}{dx^2}\left(\frac{dx}{dt}\right)^2 + \frac{dy}{dx}\frac{d^2 x}{dt^2}. \\
&\text{Substitute these expressions for the derivatives into Eq.~(i):} \\
&\quad\begin{aligned}\left[\frac{d^2 y}{dx^2}\left(\frac{dx}{dt}\right)^2 + \frac{dy}{dx}\frac{d^2 x}{dt^2}\right] + p(t)\left(\frac{dy}{dx}\frac{dx}{dt}\right) + q(t)y = 0.\end{aligned}
\end{aligned}
$$


$$\begin{aligned}\left(\frac{dx}{dt}\right)^2\frac{d^2y}{dx^2}+\frac{d^2x}{dt^2}\frac{dy}{dx}+p(t)\frac{dx}{dt}\frac{dy}{dx}+q(t)y=0\end{aligned}$$
Therefore,
$$\left(\dfrac{dx}{dt}\right)^2\dfrac{d^2y}{dx^2}+\left(\dfrac{d^2x}{dt^2}+p(t)\dfrac{dx}{dt}\right)\dfrac{dy}{dx}+q(t)y=0.$$

In order for Eq. (iv) to have constant coefficients, the coefficients of $d^2y/dx^2$ and $y$ must be
proportional.
$$\begin{pmatrix}\dfrac{dx}{dt}\end{pmatrix}^2\propto q(t)$$
Introduce a proportionality constant $k$ to change this to an equation we can use
$$\left(\frac{dx}{dt}\right)^2=kq(t)$$
Take the square root of both sides.
$$\dfrac{dx}{dt}=\pm[kq(t)]^{1/2}$$
(1)

Differentiate both sides with respect to $t.$
$$\begin{aligned}\frac{d^{2}x}{dt^{2}}&=\pm\frac12[kq(t)]^{-1/2}kq^{\prime}(t)\\&=\pm\frac{kq^{\prime}(t)}{2[kq(t)]^{1/2}}\end{aligned}$$
Now substitute the previous three equations into Eq. (iv).
$$kq(t)\frac{d^2y}{dx^2}+\left(\pm\frac{kq'(t)}{2[kq(t)]^{1/2}}\pm p(t)[kq(t)]^{1/2}\right)\frac{dy}{dx}+q(t)y=0$$
$$kq(t)\frac{d^2y}{dx^2}\pm\left(\frac{kq'(t)+2p(t)[kq(t)]}{2[kq(t)]^{1/2}}\right)\frac{dy}{dx}+q(t)y=0$$
Divide both sides by $kq(t).$
$$\begin{aligned}\frac{d^2y}{dx^2}\pm\left(\frac{kq'(t)+2p(t)[kq(t)]}{2[kq(t)]^{3/2}}\right)\frac{dy}{dx}+\frac{1}{k}y=0\end{aligned}$$
Provided that the coefficient of $dy/dx$ is constant,
$$\pm\left(\frac{kq'(t)+2p(t)[kq(t)]}{2[kq(t)]^{3/2}}\right)=A,\quad\mathrm{or}\quad\frac{q'(t)+2p(t)q(t)}{[kq(t)]^{3/2}}=\pm\frac{2A}{k}=B$$
if we multiply both sides by $\pm2/k$, Eq. (i) can be transformed into a constant-coefficient ODE by

$x= u( t) .$ Integrating both sides of equation ( 1) with respect to $t$,we find what $x$ is exactly.
$$x(t)=\pm\int^t[kq(s)]^{1/2}\:ds$$
Note that for $[kq(s)]^{1/2}$ and $[kq(t)]^{3/2}$ to be real numbers, $k$ should be chosen to have the same sign as $q(t).$ For example, if $q(t)$ is positive, $k$ can be chosen to be 1 for convenience. Or if $q(t)$ is negative, $k$ can be chosen to be -1.

--------------------------------------------------------------------------
#### Q 35

$$
\begin{aligned}
&\text{Divide both sides by } t. \\
&y'' + \left( t - \frac{1}{t} \right) y' + t^2 y = 0 \\
&\text{To turn this ODE into one with constant coefficients, make the change of variables,} \\
&x = \int_{0}^{t} (s^2)^{1/2} \, ds = \int_{0}^{t} s \, ds = \frac{t^2}{2}. \\
&\text{Use the chain rule to write } y' \text{ and } y'' \text{ in terms of this new variable.} \\
&\frac{dy}{dt} = \frac{dy}{dx} \frac{dx}{dt} \\
&\frac{d^2 y}{dt^2} = \frac{d}{dt} \left( \frac{dy}{dt} \right) = \frac{d}{dt} \left( \frac{dy}{dx} \frac{dx}{dt} \right) = \frac{d}{dt} \left( \frac{dy}{dx} \right) \frac{dx}{dt} + \frac{dy}{dx} \frac{d}{dt} \left( \frac{dx}{dt} \right) \\
&= \frac{dx}{dt} \left( \frac{d}{dx} \left( \frac{dy}{dx} \right) \right) \frac{dx}{dt} + \frac{dy}{dx} \frac{d^2 x}{dt^2} = \frac{d^2 y}{dx^2} \left( \frac{dx}{dt} \right)^2 + \frac{dy}{dx} \frac{d^2 x}{dt^2}. \\
&\text{Substitute these expressions for the derivatives into the ODE.} \\
&\left( \frac{d^2 y}{dx^2} t^2 + \frac{dy}{dx} \right) + \left( t - \frac{1}{t} \right) \left( \frac{dy}{dx} t \right) + t^2 y = 0 \\
&\frac{d^2 y}{dx^2} t^2 + \frac{dy}{dx} + (t^2 - t) \frac{dy}{dx} + t^2 y = 0 \\
&\frac{d^2 y}{dx^2} t^2 + t^2 \frac{dy}{dx} + t^2 y = 0 \\
&\frac{d^2 y}{dx^2} + \frac{dy}{dx} + y = 0 \\
&\text{Divide both sides by } t^2. \\
&\frac{d^2 y}{dx^2} + \frac{dy}{dx} + y = 0 \\
&\text{Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form } y = e^{rx}. \\
&y = e^{rx} \implies \frac{dy}{dx} = re^{rx} \implies \frac{d^2 y}{dx^2} = r^2 e^{rx} \\
&\text{Substitute these expressions into the ODE.} \\
&r^2 e^{rx} + re^{rx} + e^{rx} = 0 \\
&\text{Divide both sides by } e^{rx}. \\
&r^2 + r + 1 = 0 \\
&r = \frac{-1 \pm \sqrt{1 - 4(1)(1)}}{2} = \frac{-1 \pm \sqrt{-3}}{2} = \frac{-1 \pm i \sqrt{3}}{2} = \frac{1}{2} \pm i \frac{\sqrt{3}}{2} \\
&r = \left\{ \frac{1}{2} - i \frac{\sqrt{3}}{2}, \frac{1}{2} + i \frac{\sqrt{3}}{2} \right\} \\
\end{aligned}
$$
$$

\begin{aligned}
&\text{Two solutions to the ODE are } y = e^{(-1/2 - i\sqrt{3}/2)x} \text{ and } y = e^{(-1/2 + i\sqrt{3}/2)x}, \text{ so the general solution is a linear combination of the two.} \\
&y(x) = C_1 e^{(-1/2 - i\sqrt{3}/2)x} + C_2 e^{(-1/2 + i\sqrt{3}/2)x} \\
&= C_1 e^{-x/2 - i\sqrt{3}x/2} + C_2 e^{-x/2 + i\sqrt{3}x/2} \\
&= C_1 e^{-x/2} e^{-i\sqrt{3}x/2} + C_2 e^{-x/2} e^{i\sqrt{3}x/2} \\
&= C_1 e^{-x/2} \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) + i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] + C_2 e^{-x/2} \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) - i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] \\
&= C_1 e^{-x/2} \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) + i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] + C_2 e^{-x/2} \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) - i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] \\
&= e^{-x/2} \left( C_1 \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) + i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] + C_2 \left[ \cos \left( \frac{\sqrt{3}}{2} x \right) - i \sin \left( \frac{\sqrt{3}}{2} x \right) \right] \right) \\
&= e^{-x/2} \left( \left( C_1 + C_2 \right) \cos \left( \frac{\sqrt{3}}{2} x \right) + i \left( C_1 - C_2 \right) \sin \left( \frac{\sqrt{3}}{2} x \right) \right) \\
&\text{Using } C_3 \text{ for } C_1 + C_2 \text{ and } C_4 \text{ for } i(C_1 - C_2), \text{ the real general solution is} \\
&y(x) = C_3 e^{-x/2} \cos \left( \frac{\sqrt{3}}{2} x \right) + C_4 e^{-x/2} \sin \left( \frac{\sqrt{3}}{2} x \right). \\
&\text{Therefore, since } x = t^2 / 2, \\
&y(t) = C_3 e^{-t^2/4} \cos \left( \frac{\sqrt{3}}{4} t^2 \right) + C_4 e^{-t^2/4} \sin \left( \frac{\sqrt{3}}{4} t^2 \right).
\end{aligned}
$$


### Section 3.4

#### Q 1

Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y'=re^{rt}\quad\to\quad y''=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2e^{rt}-2(re^{rt})+e^{rt}=0$$
Divide both sides by $e^rt.$
$$r^2-2r+1=0$$
$$(r-1)^2=0$$
$$r=\begin{Bmatrix}1\end{Bmatrix}$$
One solution to the ODE is $y=e^t.$ Because the ODE is homogeneous, any constant multiple of this is also a solution, that is, $y=ce^t.$ According to the method of reduction of order, the general solution is found by allowing $c$ to vary as a function of $t.$
$$y(t)=c(t)e^t$$
Substitute this expression for $y$ into the original ODE to determine $c(t).$
$$y''-2y'+y=0\quad\to\quad[c(t)e^t]''-2[c(t)e^t]'+[c(t)e^t]=0$$
Evaluate the derivatives using the product rule.
$$[c'(t)e^t+c(t)e^t]'-2[c'(t)e^t+c(t)e^t]+c(t)e^t=0$$
$$c''(t)e^t+c'(t)e^t+c'(t)e^t+c(t)e^t-2c'(t)e^t-2c(t)e^t+c(t)e^t=0$$
$$c''(t)e^t=0$$
Divide both sides by $e^t.$
$$c''(t)=0$$
Integrate both sides with respect to $t.$
$$c'(t)=C_1$$
Integrate both sides with respect to $t$ once more.
$$c(t)=C_1t+C_2$$
Therefore, the general solution is
$$y(t)=C_1te^t+C_2e^t.$$


#### Q 5


$$
\begin{aligned}
&\text{Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form } y = e^{rt}. \\
&y = e^{rt} \implies y' = re^{rt} \implies y'' = r^2 e^{rt} \\
&\text{Substitute these expressions into the ODE.} \\
&r^2 e^{rt} - 6r e^{rt} + 9 e^{rt} = 0 \\
&\text{Divide both sides by } e^{rt}. \\
&r^2 - 6r + 9 = 0 \\
&(r - 3)^2 = 0 \\
&r = 3 \\
&\text{One solution to the ODE is } y = e^{3t}. \\
&\text{Because the ODE is homogeneous, any constant multiple of this is also a solution, that is, } y = ce^{3t}. \\
&\text{According to the method of reduction of order, the general solution is found by allowing } c \text{ to vary as a function of } t. \\
&y(t) = c(t)e^{3t} \\
&\text{Substitute this expression for } y \text{ into the original ODE to determine } c(t). \\
&y'' - 6y' + 9y = 0 \implies [c(t)e^{3t}]'' - 6[c(t)e^{3t}]' + 9[c(t)e^{3t}] = 0 \\
&\text{Evaluate the derivatives using the product rule.} \\
&[c'(t)e^{3t} + 3c(t)e^{3t}]' - 6[c'(t)e^{3t} + 3c(t)e^{3t}] + 9[c(t)e^{3t}] = 0 \\
&[c''(t)e^{3t} + 6c'(t)e^{3t} + 9c(t)e^{3t}] - 6[c'(t)e^{3t} + 3c(t)e^{3t}] + 9[c(t)e^{3t}] = 0 \\
&c''(t)e^{3t} = 0 \\
&\text{Divide both sides by } e^{3t}. \\
&c''(t) = 0 \\
&\text{Integrate both sides with respect to } t. \\
&c'(t) = C_1 \\
&\text{Integrate both sides with respect to } t \text{ once more.} \\
&c(t) = C_1 t + C_2 \\
&\text{Therefore, the general solution is} \\
&y(t) = (C_1 t + C_2)e^{3t}.
\end{aligned}
$$



#### Q 7


$$
\begin{aligned}
&\text{Given differential equation:} \\
&16y'' + 24y' + 9y = 0 \\
&\text{Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form } y = e^{rt}. \\
&y = e^{rt} \implies y' = re^{rt} \implies y'' = r^2 e^{rt} \\
&\text{Substitute these expressions into the ODE:} \\
&16(r^2 e^{rt}) + 24(r e^{rt}) + 9(e^{rt}) = 0 \\
&\text{Divide both sides by } e^{rt}: \\
&16r^2 + 24r + 9 = 0 \\
&(4r + 3)^2 = 0 \\
&r = -\frac{3}{4} \\
&\text{One solution to the ODE is } y = e^{-3t/4}. \\
&\text{Because the ODE is homogeneous, any constant multiple of this is also a solution, that is, } y = ce^{-3t/4}. \\
&\text{According to the method of reduction of order, the general solution is found by allowing } c \text{ to vary as a function of } t: \\
&y(t) = c(t)e^{-3t/4} \\
&\text{Substitute this expression for } y \text{ into the original ODE to determine } c(t): \\
&16y'' + 24y' + 9y = 0 \implies 16[c(t)e^{-3t/4}]'' + 24[c(t)e^{-3t/4}]' + 9[c(t)e^{-3t/4}] = 0 \\
&\text{Evaluate the derivatives using the product rule:} \\
&16\left[ c''(t)e^{-3t/4} - \frac{3}{2}c'(t)e^{-3t/4} + \frac{9}{16}c(t)e^{-3t/4} \right] + 24\left[ c'(t)e^{-3t/4} - \frac{3}{4}c(t)e^{-3t/4} \right] + 9[c(t)e^{-3t/4}] = 0 \\
&16c''(t)e^{-3t/4} = 0 \\
&\text{Divide both sides by } 16e^{-3t/4}: \\
&c''(t) = 0 \\
&\text{Integrate both sides with respect to } t: \\
&c'(t) = C_1 \\
&\text{Integrate both sides with respect to } t \text{ once more:} \\
&c(t) = C_1 t + C_2 \\
&\text{Therefore, the general solution is:} \\
&y(t) = (C_1 t + C_2)e^{-3t/4}.
\end{aligned}
$$


#### Q 11

$$
\begin{aligned}
&\text{Given differential equation:} \\
&y'' + 4y' + 4y = 0 \\
&\text{Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form } y = e^{rt}. \\
&y = e^{rt} \implies y' = re^{rt} \implies y'' = r^2 e^{rt} \\
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} + 4r e^{rt} + 4 e^{rt} = 0 \\
&\text{Divide both sides by } e^{rt}: \\
&r^2 + 4r + 4 = 0 \\
&(r + 2)^2 = 0 \\
&r = -2 \\
&\text{One solution to the ODE is } y = e^{-2t}. \\
&\text{Because the ODE is homogeneous, any constant multiple of this is also a solution, that is, } y = ce^{-2t}. \\
&\text{According to the method of reduction of order, the general solution is found by allowing } c \text{ to vary as a function of } t: \\
&y(t) = c(t)e^{-2t} \\
&\text{Substitute this expression for } y \text{ into the original ODE to determine } c(t): \\
&y'' + 4y' + 4y = 0 \implies [c(t)e^{-2t}]'' + 4[c(t)e^{-2t}]' + 4[c(t)e^{-2t}] = 0 \\
&\text{Evaluate the derivatives using the product rule:} \\
&[c''(t)e^{-2t} - 4c'(t)e^{-2t} + 4c(t)e^{-2t}] + 4[c'(t)e^{-2t} - 2c(t)e^{-2t}] + 4[c(t)e^{-2t}] = 0 \\
&c''(t)e^{-2t} = 0 \\
&\text{Divide both sides by } e^{-2t}: \\
&c''(t) = 0 \\
&\text{Integrate both sides with respect to } t: \\
&c'(t) = C_1 \\
&\text{Integrate both sides with respect to } t \text{ once more:} \\
&c(t) = C_1 t + C_2 \\
&\text{Therefore, the general solution is:} \\
&y(t) = (C_1 t + C_2)e^{-2t}.
\end{aligned}
$$



$$y'(t)=C_1e^{-2t}-2C_1te^{-2t}-2C_2e^{-2t}$$
Apply the initial conditions now to determine $C_1$ and $C_2.$
$$\begin{aligned}y(-1)&=-C_1e^2+C_2e^2=2\\y'(-1)&=C_1e^2+2C_1e^2-2C_2e^2=1\end{aligned}$$
Solving this system of equations yields $C_1=5/e^2$ and $C_2=7/e^2.$ Therefore,
$$y(t)=\frac{5}{e^2}te^{-2t}+\frac{7}{e^2}e^{-2t}.$$
Take the limit of $y(t)$ as $t\to\infty.$
$$\begin{aligned}\lim_{t\to\infty}y(t)&=\lim_{t\to\infty}\left(\frac{5}{e^{2}}te^{-2t}+\frac{7}{e^{2}}e^{-2t}\right)\\&=\lim_{t\to\infty}\left(\frac{5}{e^{2}}t+\frac{7}{e^{2}}\right)e^{-2t}\\&=\lim_{t\to\infty}\frac{\frac{5}{e^{2}}t+\frac{7}{e^{2}}}{e^{2t}}\\&\overset{\infty}{\operatorname*{=}}\lim_{t\to\infty}\frac{\frac{5}{e^{2}}}{2e^{2t}}\\&=0\end{aligned}$$
Below is a plot of $y(t)$ versus $t.$

![[Pasted image 20240712150714.png]]

$$y(t)=\frac5{e^2}\:t\:e^{-2\:t}+\frac7{e^2}\:e^{-2\:t}$$

#### Q 12

$$
\begin{aligned}
&\text{Given differential equation:} \\
&y'' - y' + 0.25y = 0 \\[10pt]
&\text{Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form } y = e^{rt}. \\[10pt]
&y = e^{rt} \implies y' = re^{rt} \implies y'' = r^2 e^{rt} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} - r e^{rt} + 0.25 e^{rt} = 0 \\[10pt]
&\text{Divide both sides by } e^{rt}: \\
&r^2 - r + 0.25 = 0 \\[10pt]
&r = \frac{1 \pm \sqrt{1 - 4(0.25)}}{2} = \frac{1}{2} \\[10pt]
&\text{One solution to the ODE is } y = e^{t/2}. \\
&\text{Because the ODE is homogeneous, any constant multiple of this is also a solution, that is, } y = ce^{t/2}. \\[10pt]
&\text{According to the method of reduction of order, the general solution is found by allowing } c \text{ to vary as a function of } t: \\
&y(t) = c(t)e^{t/2} \\[10pt]
&\text{Substitute this expression for } y \text{ into the original ODE to determine } c(t): \\
&y'' - y' + 0.25y = 0 \implies [c(t)e^{t/2}]'' - [c(t)e^{t/2}]' + 0.25[c(t)e^{t/2}] = 0 \\[10pt]
&\text{Evaluate the derivatives using the product rule:} \\
&[c''(t)e^{t/2} + c'(t)\frac{1}{2}e^{t/2} + c'(t)\frac{1}{2}e^{t/2} + c(t)\frac{1}{4}e^{t/2}] - [c'(t)e^{t/2} + c(t)\frac{1}{2}e^{t/2}] + 0.25[c(t)e^{t/2}] = 0 \\
&c''(t)e^{t/2} = 0 \\[10pt]
&\text{Divide both sides by } e^{t/2}: \\
&c''(t) = 0 \\[10pt]
&\text{Integrate both sides with respect to } t: \\
&c'(t) = C_1 \\[10pt]

\end{aligned}
$$


$$c(t)=C_1t+C_2$$
$$y(t)=C_1te^{t/2}+C_2e^{t/2}.$$
Integrate both sides with respect to $t$ once more.
The general solution is then
Differentiate it with respect to $t.$
$$y'(t)=C_1e^{t/2}+\frac12C_1te^{t/2}+\frac12C_2e^{t/2}$$
Apply the initial conditions now to determine $C_1$ and $C_2.$
$$\begin{aligned}&y(0)=C_{2}=2\\&y'(0)=C_{1}+\frac{1}{2}C_{2}=b\end{aligned}$$
Solving this system of equations yields $C_1=b-1$ and $C_2=2.$ Therefore
$$\begin{aligned}y(t)&=(b-1)te^{t/2}+2e^{t/2}\\&=[(b-1)t+2]e^{t/2}.\end{aligned}$$
For $y(t)$ to always be positive, the quantity in square brackets must always be positive. More
specifically, the coefficient of $t$ must be positive. The value of $b$ that separates positive and
negative solutions is
$$b-1=0$$
$$b=1.$$



#### Q 18

$$
\begin{aligned}
&\text{Given differential equation:} \\
&t^2 y'' - 4t y' + 6y = 0, \quad t > 0; \quad y_1(t) = t^2 \\[10pt]
&\text{Since this ODE is homogeneous, any constant multiple of } y_1(t) \text{ is also a solution: } c y_1(t) = c t^2. \\
&\text{According to the method of reduction of order, the general solution is obtained by allowing } c \text{ to vary as a function of } t: \\
&y(t) = c(t)t^2 \\[10pt]
&\text{Substitute this formula for } y(t) \text{ into the ODE:} \\
&t^2 \left[ c(t)t^2 \right]'' - 4t \left[ c(t)t^2 \right]' + 6 \left[ c(t)t^2 \right] = 0 \\[10pt]
&\text{Evaluate the derivatives using the product rule:} \\
&t^2 \left[ c''(t)t^2 + 4c'(t)t + 2c(t) \right] - 4t \left[ c'(t)t^2 + 2c(t)t \right] + 6c(t)t^2 = 0 \\[10pt]
&t^2 \left[ c''(t)t^2 + 4c'(t)t + 2c(t) \right] - 4t \left[ c'(t)t^2 + 2c(t)t \right] + 6c(t)t^2 = 0 \\[10pt]
&t^4 c''(t) + 4t^3 c'(t) + 2t^2 c(t) - 4t^3 c'(t) - 8t^2 c(t) + 6t^2 c(t) = 0 \\[10pt]
&t^4 c''(t) = 0 \\[10pt]
&\text{Divide both sides by } t^4: \\
&c''(t) = 0 \\[10pt]
&\text{Integrate both sides with respect to } t: \\
&c'(t) = C_1 \\[10pt]
&\text{Integrate both sides with respect to } t \text{ once more:} \\
&c(t) = C_1 t + C_2 \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(t) = (C_1 t + C_2) t^2 \\[10pt]
&\text{The second solution is } y_2(t) = t^3.
\end{aligned}
$$


#### Q 21

$$
\begin{aligned}
&\text{Given differential equation:} \\
&xy'' - y' + 4x^3 y = 0, \quad x > 0; \quad y_1(x) = \sin x^2 \\[10pt]
&\text{Since this ODE is homogeneous, any constant multiple of } y_1(x) \text{ is also a solution: } c y_1(x) = c \sin x^2. \\
&\text{According to the method of reduction of order, the general solution is obtained by allowing } c \text{ to vary as a function of } x: \\
&y(x) = c(x) \sin x^2 \\[10pt]
&\text{Substitute this formula for } y(x) \text{ into the ODE:} \\
&x [c(x) \sin x^2]'' - [c(x) \sin x^2]' + 4x^3 [c(x) \sin x^2] = 0 \\[10pt]
&\text{Evaluate the derivatives using the product rule:} \\
&x \left[ c''(x) \sin x^2 + 2c'(x) \cos x^2 - c(x) \sin x^2 \right] - \left[ c'(x) \sin x^2 + 2c(x) \cos x^2 \right] + 4x^3 c(x) \sin x^2 = 0 \\[10pt]
&x \left[ c''(x) \sin x^2 + 2c'(x) \cos x^2 \right] - c'(x) \sin x^2 = 0 \\[10pt]
&x \sin x^2 c''(x) + 2x \cos x^2 c'(x) - c'(x) \sin x^2 = 0 \\[10pt]
&c''(x) \sin x^2 + 2c'(x) \cos x^2 - \frac{c'(x) \sin x^2}{x} = 0 \\[10pt]
&c''(x) \sin x^2 + \left( 2 \cos x^2 - \frac{\sin x^2}{x} \right) c'(x) = 0 \\[10pt]
&\text{Solve for } c''(x)/c'(x): \\
&\frac{c''(x)}{c'(x)} = - \left( 2 \frac{\cos x^2}{\sin x^2} - \frac{1}{x} \right) = - 2 \cot x^2 + \frac{1}{x} \\[10pt]
&\text{Integrate both sides:} \\
&\ln c'(x) = \int \left( -2 \cot x^2 + \frac{1}{x} \right) dx \\[10pt]
&\text{Make the substitution } u = \sin x^2, \quad du = 2x \cos x^2 dx: \\
&\ln c'(x) = \int \left( -2 \frac{du}{u} + \frac{1}{x} dx \right) = -2 \ln \left| \sin x^2 \right| + \ln x + C_1 \\[10pt]
&\ln c'(x) = \ln \left( x \sin^{-2} x^2 \right) + C_1 \\[10pt]
&c'(x) = C_2 \frac{x}{\sin^2 x^2} \\[10pt]
&\text{Integrate both sides again:} \\
&c(x) = \int \frac{x}{\sin^2 x^2} C_2 dx = C_3 \cot x^2 + C_4 \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(x) = C_3 \cot x^2 + C_4 \sin x^2.
\end{aligned}
$$


#### Q 25


$$
\begin{aligned}
&\text{Given differential equation:} \\
&t^2 y'' + 3t y' + y = 0, \quad t > 0; \quad y_1(t) = t^{-1} \\[10pt]
&\text{Divide both sides of the ODE by } t^2 \text{ to put it in the proper form:} \\
&y'' + \frac{3}{t} y' + \frac{1}{t^2} y = 0 \\[10pt]
&\text{Use the result of Problem 32 to determine a second solution:} \\
&y_2(t) = y_1(t) \int \frac{1}{[y_1(r)]^2} \exp \left( -\int \frac{3}{s} \, ds \right) dr \\[10pt]
&y_2(t) = t^{-1} \int \frac{1}{(r^{-1})^2} \exp \left( -\int \frac{3}{s} \, ds \right) dr \\[10pt]
&y_2(t) = t^{-1} \int r^2 \exp (-3 \ln r) \, dr \\[10pt]
&y_2(t) = t^{-1} \int r^2 r^{-3} \, dr \\[10pt]
&y_2(t) = t^{-1} \int dr \\[10pt]
&y_2(t) = t^{-1} \ln t \\[10pt]
&\text{Thus, the second solution is:} \\
&y_2(t) = t^{-1} \ln t.
\end{aligned}
$$


### Section 5.4


#### Q 1

$$
\begin{aligned}
&\text{Given differential equation:} \\
&x^2 y'' + 4xy' + 2y = 0 \\[10pt]
&\text{This is a homogeneous equidimensional (Euler) ODE, so the solution is of the form } y = x^r. \\[10pt]
&y = x^r \implies y' = rx^{r-1} \implies y'' = r(r-1)x^{r-2} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&x^2 r(r-1)x^{r-2} + 4x rx^{r-1} + 2x^r = 0 \\[10pt]
&r(r-1)x^r + 4r x^r + 2x^r = 0 \\[10pt]
&\text{Divide both sides by } x^r: \\
&r(r-1) + 4r + 2 = 0 \\[10pt]
&\text{Solve for } r: \\
&r^2 + 3r + 2 = 0 \\
&(r+2)(r+1) = 0 \\
&r = -2, -1 \\[10pt]
&\text{Two solutions to the ODE are } y = x^{-2} \text{ and } y = x^{-1}. \\
&\text{The general solution is a linear combination of these two:} \\
&y(x) = C_1 x^{-2} + C_2 x^{-1}.
\end{aligned}
$$


#### Q 3

$$
\begin{aligned}
&\text{Given differential equation:} \\
&x^2 y'' - 3xy' + 4y = 0 \\[10pt]
&\text{This is a homogeneous equidimensional (Euler) ODE, so the solution is of the form } y = x^r. \\[10pt]
&y = x^r \implies y' = rx^{r-1} \implies y'' = r(r-1)x^{r-2} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&x^2 r(r-1)x^{r-2} - 3xr x^{r-1} + 4x^r = 0 \\[10pt]
&x^r \left[ r(r-1) - 3r + 4 \right] = 0 \\[10pt]
&\text{Divide both sides by } x^r: \\
&r(r-1) - 3r + 4 = 0 \\
&r^2 - 4r + 4 = 0 \\
&(r-2)^2 = 0 \\
&r = 2 \\[10pt]
&\text{The general solution can be obtained by using the method of reduction of order: Plug in } y(x) = c(x)x^2 \text{ into the ODE:} \\
&x^2 [c(x)x^2]'' - 3x [c(x)x^2]' + 4 [c(x)x^2] = 0 \\[10pt]
&\text{Evaluate the derivatives:} \\
&x^2 [c''(x)x^2 + 2c'(x)x] - 3x [c'(x)x^2 + 2c(x)x] + 4c(x)x^2 = 0 \\[10pt]
&c''(x)x^4 + 2c'(x)x^3 - 3c'(x)x^3 - 6c(x)x^2 + 4c(x)x^2 = 0 \\
&c''(x)x^4 - c'(x)x^3 = 0 \\[10pt]
&\text{Solve this ODE for } c(x): \\
&c''(x) - \frac{c'(x)}{x} = 0 \\
&\text{Integrate both sides with respect to } x: \\
&\frac{d}{dx} [\ln c'(x)] = -\frac{1}{x} \\
&\ln c'(x) = -\ln x + C_1 \\
&c'(x) = e^{-\ln x + C_1} = \frac{e^{C_1}}{x} \\[10pt]
&\text{Integrate again:} \\
&c(x) = e^{C_1} \ln x + C_2 \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(x) = c(x)x^2 = (e^{C_1} \ln x + C_2)x^2 \\
&y(x) = C_3 x^2 \ln x + C_2 x^2.
\end{aligned}
$$



#### Q 9


$$
\begin{aligned}
&\text{Given differential equation:} \\
&2x^2 y'' + xy' - 3y = 0, \quad y(1) = 1, \quad y'(1) = 4 \\[10pt]
&\text{This is a homogeneous equidimensional (Euler) ODE, so the solution is of the form } y = x^r. \\[10pt]
&y = x^r \implies y' = rx^{r-1} \implies y'' = r(r-1)x^{r-2} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&2x^2 r(r-1)x^{r-2} + xr x^{r-1} - 3x^r = 0 \\
&2r(r-1)x^r + rx^r - 3x^r = 0 \\
&x^r [2r(r-1) + r - 3] = 0 \\[10pt]
&\text{Divide both sides by } x^r: \\
&2r^2 - r - 3 = 0 \\
&(2r-3)(r+1) = 0 \\
&r = \frac{3}{2}, -1 \\[10pt]
&\text{Two solutions to the ODE are } y = x^{-1} \text{ and } y = x^{3/2}. \\
&\text{The general solution is a linear combination of these two:} \\
&y(x) = C_1 x^{-1} + C_2 x^{3/2} \\[10pt]
&\text{Differentiate with respect to } x: \\
&y'(x) = -C_1 x^{-2} + \frac{3}{2} C_2 x^{1/2} \\[10pt]
&\text{Apply the initial conditions to determine } C_1 \text{ and } C_2: \\
&y(1) = 1 \implies C_1 + C_2 = 1 \\
&y'(1) = 4 \implies -C_1 + \frac{3}{2} C_2 = 4 \\[10pt]
&\text{Solve this system of equations:} \\
&C_1 = -1, \quad C_2 = 2 \\[10pt]
&\text{Thus, the solution is:} \\
&y(x) = -x^{-1} + 2x^{3/2} \\[10pt]
&\text{As } x \to 0: \\
&\lim_{x \to 0} y(x) = \lim_{x \to 0} \left( -x^{-1} + 2x^{3/2} \right) = -\infty
\end{aligned}
$$




![[Pasted image 20240712154322.png]]



### Section 3.5

#### Q 5

$$
\begin{aligned}
&\text{Given differential equation:} \\
&y'' + 2y' = 3 + 4 \sin 2t \\[10pt]
&\text{The general solution can be expressed as the sum of the complementary solution } y_c(t) \text{ and the particular solution } y_p(t): \\
&y(t) = y_c(t) + y_p(t) \\[10pt]
&\text{The complementary solution satisfies the associated homogeneous equation:} \\
&y_c'' + 2y_c' = 0 \\[10pt]
&\text{This is a homogeneous ODE with constant coefficients, so the solution is of the form } y_c = e^{rt}: \\
&y_c = e^{rt} \implies y_c' = re^{rt} \implies y_c'' = r^2 e^{rt} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} + 2r e^{rt} = 0 \\[10pt]
&\text{Divide both sides by } e^{rt}: \\
&r(r + 2) = 0 \\
&r = 0, -2 \\[10pt]
&\text{Two solutions to the homogeneous equation are } y_c = e^{-2t} \text{ and } y_c = e^{0t} = 1. \\
&\text{By the principle of superposition, the general solution is a linear combination of these two:} \\
&y_c(t) = C_1 e^{-2t} + C_2 \\[10pt]
&\text{The particular solution satisfies:} \\
&y_p'' + 2y_p' = 3 + 4 \sin 2t \\[10pt]
&\text{The inhomogeneous term has both a constant and a sine function. The trial solution is:} \\
&y_p(t) = At + B \cos 2t + C \sin 2t \\[10pt]
&\text{Substitute this into the ODE to determine } A, B, \text{ and } C: \\
&(At + B \cos 2t + C \sin 2t)'' + 2(At + B \cos 2t + C \sin 2t)' = 3 + 4 \sin 2t \\[10pt]
&-4B \cos 2t - 4C \sin 2t + 2A + 2B(-2 \sin 2t) + 2C(2 \cos 2t) = 3 + 4 \sin 2t \\[10pt]
&-4B \cos 2t - 4C \sin 2t + 2A - 4B \sin 2t + 4C \cos 2t = 3 + 4 \sin 2t \\[10pt]
&\text{Group like terms and solve the system of equations:} \\
&2A = 3 \\
&-4B + 4C = 0 \\
&-4B - 4C = 4 \\[10pt]
&\text{Solving this system yields:} \\
&A = \frac{3}{2}, \quad B = -\frac{1}{2}, \quad C = -\frac{1}{2} \\[10pt]
&\text{Thus, the particular solution is:} \\
&y_p(t) = \frac{3}{2}t - \frac{1}{2} \cos 2t - \frac{1}{2} \sin 2t \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(t) = C_1 e^{-2t} + C_2 + \frac{3}{2}t - \frac{1}{2} \cos 2t - \frac{1}{2} \sin 2t
\end{aligned}
$$

#### Q 8


$$
\begin{aligned}
&\text{Given differential equation:} \\
&u'' + \omega_0^2 u = \cos \omega t, \quad \omega^2 \neq \omega_0^2 \\[10pt]
&\text{The general solution can be expressed as the sum of the complementary solution } u_c(t) \text{ and the particular solution } u_p(t): \\
&u(t) = u_c(t) + u_p(t) \\[10pt]
&\text{The complementary solution satisfies the homogeneous equation:} \\
&u_c'' + \omega_0^2 u_c = 0 \\[10pt]
&\text{This is a homogeneous ODE with constant coefficients, so the solution is of the form } u_c = e^{rt}: \\
&u_c = e^{rt} \implies u_c' = re^{rt} \implies u_c'' = r^2 e^{rt} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} + \omega_0^2 e^{rt} = 0 \\[10pt]
&\text{Divide both sides by } e^{rt}: \\
&r^2 + \omega_0^2 = 0 \\
&r = \pm i \omega_0 \\[10pt]
&\text{The complementary solution is:} \\
&u_c(t) = C_1 e^{-i \omega_0 t} + C_2 e^{i \omega_0 t} \\[10pt]
&\text{Using Euler's formula, the general solution can be written as:} \\
&u_c(t) = C_3 \cos \omega_0 t + C_4 \sin \omega_0 t \\[10pt]
&\text{The particular solution satisfies:} \\
&u_p'' + \omega_0^2 u_p = \cos \omega t \\[10pt]
&\text{Since only even derivatives are present, the trial solution will be } u_p(t) = A \cos \omega t. \\[10pt]
&\text{Substitute this into the ODE to determine } A: \\
&-A \omega^2 \cos \omega t + A \omega_0^2 \cos \omega t = \cos \omega t \\[10pt]
&(-A \omega^2 + A \omega_0^2) \cos \omega t = \cos \omega t \\[10pt]
&\text{For this equation to be true, } A \text{ must satisfy:} \\
&-A \omega^2 + A \omega_0^2 = 1 \\
&A (\omega_0^2 - \omega^2) = 1 \\
&A = \frac{1}{\omega_0^2 - \omega^2} \\[10pt]
&\text{Thus, the particular solution is:} \\
&u_p(t) = \frac{1}{\omega_0^2 - \omega^2} \cos \omega t \\[10pt]
&\text{Therefore, the general solution is:} \\
&u(t) = C_3 \cos \omega_0 t + C_4 \sin \omega_0 t + \frac{1}{\omega_0^2 - \omega^2} \cos \omega t.
\end{aligned}
$$


#### Q 16


$$
\begin{aligned}
&\text{Given differential equation:} \\
&y'' + 3y' = 2t^4 + t^2 e^{-3t} + \sin 3t \\[10pt]
&\text{The general solution can be expressed as the sum of the complementary solution } y_c(t) \text{ and the particular solution } y_p(t): \\
&y(t) = y_c(t) + y_p(t) \\[10pt]
&\text{The complementary solution satisfies the homogeneous equation:} \\
&y_c'' + 3y_c' = 0 \\[10pt]
&\text{This is a homogeneous ODE with constant coefficients, so the solution is of the form } y_c = e^{rt}: \\
&y_c = e^{rt} \implies y_c' = re^{rt} \implies y_c'' = r^2 e^{rt} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} + 3r e^{rt} = 0 \\[10pt]
&\text{Divide both sides by } e^{rt}: \\
&r(r + 3) = 0 \\
&r = 0, -3 \\[10pt]
&\text{The complementary solution is:} \\
&y_c(t) = C_1 e^{-3t} + C_2 \\[10pt]
&\text{The particular solution satisfies:} \\
&y_p'' + 3y_p' = 2t^4 + t^2 e^{-3t} + \sin 3t \\[10pt]
&\text{The trial solution is:} \\
&y_p(t) = t(A + Bt + Ct^2 + Dt^3 + Et^4) + t(F + Gt + Ht^2)e^{-3t} + (I \cos 3t + J \sin 3t) \\[10pt]
&\text{Substitute this into the ODE to determine } A, B, C, D, E, F, G, H, I, \text{ and } J: \\
&y_p'' + 3y_p' = 2t^4 + t^2 e^{-3t} + \sin 3t \\[10pt]
&\text{Simplifying, we get:} \\
&(3A + 2B) + (6B + 6C)t + (9C + 12D)t^2 + (12D + 20E)t^3 + (15E)t^4 \\
&+ (-3F + 2G)e^{-3t} + (-6G + 6H)te^{-3t} + (-9H)t^2 e^{-3t} + (-9I \sin 3t + 9J \cos 3t) \\[10pt]
&\text{For this equation to be true, the coefficients must satisfy the system:} \\
&3A + 2B = 0 \\
&6B + 6C = 0 \\
&9C + 12D = 0 \\
&12D + 20E = 0 \\
&15E = 2 \\
&-3F + 2G = 0 \\
&-6G + 6H = 0 \\
&-9H = 1 \\
&-9I = 1 \\
&-9J = 1 \\[10pt]
&\text{Solving this system, we find:} \\
&A = \frac{16}{81}, \; B = -\frac{8}{27}, \; C = \frac{8}{27}, \; D = -\frac{2}{9}, \; E = \frac{2}{15} \\
&F = -\frac{2}{27}, \; G = -\frac{1}{9}, \; H = -\frac{1}{9}, \; I = -\frac{1}{9}, \; J = -\frac{1}{9} \\[10pt]
&\text{Thus, the particular solution is:} \\
&y_p(t) = t \left( \frac{16}{81} - \frac{8}{27}t + \frac{8}{27}t^2 - \frac{2}{9}t^3 + \frac{2}{15}t^4 \right) \\
&\quad + t \left( -\frac{2}{27} - \frac{1}{9}t - \frac{1}{9}t^2 \right)e^{-3t} - \frac{1}{9} \cos 3t - \frac{1}{9} \sin 3t \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(t) = C_1 e^{-3t} + C_2 + t \left( \frac{16}{81} - \frac{8}{27}t + \frac{8}{27}t^2 - \frac{2}{9}t^3 + \frac{2}{15}t^4 \right) \\
&\quad + t \left( -\frac{2}{27} - \frac{1}{9}t - \frac{1}{9}t^2 \right)e^{-3t} - \frac{1}{9} \cos 3t - \frac{1}{9} \sin 3t.
\end{aligned}
$$


#### Q 17


$$
\begin{aligned}
&\text{Given differential equation:} \\
&y'' - 5y' + 6y = e^t \cos 2t + e^{2t} (3t + 4) \sin t \\[10pt]
&\text{The general solution can be expressed as the sum of the complementary solution } y_c(t) \text{ and the particular solution } y_p(t): \\
&y(t) = y_c(t) + y_p(t) \\[10pt]
&\text{The complementary solution satisfies the homogeneous equation:} \\
&y_c'' - 5y_c' + 6y_c = 0 \\[10pt]
&\text{This is a homogeneous ODE with constant coefficients, so the solution is of the form } y_c = e^{rt}: \\
&y_c = e^{rt} \implies y_c' = re^{rt} \implies y_c'' = r^2 e^{rt} \\[10pt]
&\text{Substitute these expressions into the ODE:} \\
&r^2 e^{rt} - 5r e^{rt} + 6 e^{rt} = 0 \\[10pt]
&\text{Divide both sides by } e^{rt}: \\
&r^2 - 5r + 6 = 0 \\
&(r - 2)(r - 3) = 0 \\
&r = 2, 3 \\[10pt]
&\text{The complementary solution is:} \\
&y_c(t) = C_1 e^{2t} + C_2 e^{3t} \\[10pt]
&\text{The particular solution satisfies:} \\
&y_p'' - 5y_p' + 6y_p = e^t \cos 2t + e^{2t} (3t + 4) \sin t \\[10pt]
&\text{The trial solution is:} \\
&y_p(t) = e^t (A \cos 2t + B \sin 2t) + e^{2t} (C + Dt)(E \cos t + F \sin t) \\[10pt]
&\text{Substitute this into the ODE to determine } A, B, C, D, E, \text{ and } F: \\
&y_p'' - 5y_p' + 6y_p = e^t \cos 2t + e^{2t} (3t + 4) \sin t \\[10pt]
&\text{Simplify the left side:} \\
&(-2A - 6B)e^t \cos 2t + (CE - 2DE - CF - DF)e^{2t} \sin t \\
&+ (DE - DF)e^{2t} \cos t + (-CE - DE - CF + 2DF)e^{2t} \cos t \\
&+ (-DE - DF)te^{2t} + (6A - 2B)e^t \sin 2t \\[10pt]
&\text{For this equation to be true, the coefficients must satisfy:} \\
&-2A - 6B = 1 \\
&CE - 2DE - CF - DF = 4 \\
&DE - DF = 3 \\
&-CE - DE - CF + 2DF = 0 \\
&-DE - DF = 0 \\
&6A - 2B = 0 \\[10pt]
&\text{Solving this system, we find:} \\
&A = -\frac{1}{20}, \; B = -\frac{3}{20}, \; CE = \frac{1}{2}, \; DE = \frac{3}{2}, \; CF = -5, \; DF = -\frac{3}{2} \\[10pt]
&\text{Thus, the particular solution is:} \\
&y_p(t) = e^t \left( -\frac{1}{20} \cos 2t - \frac{3}{20} \sin 2t \right) + e^{2t} \left( C + Dt \right) \left( E \cos t + F \sin t \right) \\[10pt]
&\text{Therefore, the general solution is:} \\
&y(t) = C_1 e^{2t} + C_2 e^{3t} - \frac{1}{20} e^t (\cos 2t + 3 \sin 2t) + \frac{1}{2} e^{2t} (\cos t - 10 \sin t) + \frac{3}{2} te^{2t} (\cos t - \sin t).
\end{aligned}
$$


