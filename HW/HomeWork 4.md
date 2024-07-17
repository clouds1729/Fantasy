
## Section 3.6
### Q3
$$y_p(t)=C_1(t)te^{t/2}+C_2(t)e^{t/2}$$
$\underline{\text{Method of Variation of Parameters}}$
Substitute this into the original ODE to determine $C_1(t)$ and $C_2(t).$
$$4[C_1(t)te^{t/2}+C_2(t)e^{t/2}]'''-4[C_1(t)te^{t/2}+C_2(t)e^{t/2}]'+[C_1(t)te^{t/2}+C_2(t)e^{t/2}]=16e^{t/2}$$
Evaluate the derivatives.
$$\begin{aligned}&[C_{1}^{\prime}(t)te^{-t}+C_{1}(t)e^{-t}-C_{1}(t)te^{-t}+C_{2}^{\prime}(t)e^{-t}-C_{2}(t)e^{-t}]^{\prime}\\&+2[C_{1}^{\prime}(t)te^{-t}+C_{1}(t)e^{-t}-C_{1}(t)te^{-t}+C_{2}^{\prime}(t)e^{-t}-C_{2}(t)e^{-t}]+[C_{1}(t)te^{-t}+C_{2}(t)e^{-t}]=3e^{-t}\end{aligned}$$
$$[C_{1}^{\prime\prime}(t)te^{-t}+C_{1}^{\prime}(t)e^{-t}-C_{1}^{\prime}(t)te^{-t}+C_{1}^{\prime}(t)e^{-t}-C_{1}(t)e^{-t}-C_{1}(t)te^{-t}-C_{1}(t)e^{-t}+C_{1}(t)te^{-t}\\+C_{2}^{\prime\prime}(t)e^{-t}-C_{2}^{\prime}(t)e^{-t}-C_{2}^{\prime}(t)e^{-t}+C_{2}(t)e^{-t}]\\+2[C_{1}^{\prime}(t)te^{-t}+C_{1}(t)e^{-t}-C_{1}(t)te^{-t}+C_{2}^{\prime}(t)e^{-t}-C_{2}(t)e^{-t}]+[C_{1}(t)te^{-t}+C_{2}(t)e^{-t}]=3e^{-t}$$
Simplify the left side.
$$C_{1}^{\prime\prime}(t)te^{-t}+C_{1}^{\prime}(t)e^{-t}-C_{1}^{\prime}(t)te^{-t}+C_{1}^{\prime}(t)e^{-t}-C_{1}^{\prime}(t)te^{-t}-C_{1}(t)e^{-t}+C_{1}(t)te^{-t}\\+C_{2}^{\prime\prime}(t)e^{-t}-C_{2}^{\prime}(t)e^{-t}-C_{2}^{\prime}(t)e^{-t}+C_{2}(t)e^{-t}\\+2C_{1}^{\prime}(t)te^{-t}+2C_{1}(t)e^{-t}-2C_{1}(t)te^{-t}+2C_{2}^{\prime}(t)e^{-t}-2C_{2}(t)e^{-t}+C_{1}(t)te^{-t}+C_{2}(t)e^{-t}=3e^{-t}$$
$$C_1''(t)te^{-t}+C_1'(t)e^{-t}-C_1'(t)te^{-t}+C_2''(t)e^{-t}=3e^{-t}$$
Multiply both sides by $e^{t}.$
$$C_1''(t)t+C_1'(t)-C_1'(t)t+C_2''(t)=3$$
If we set
$$C_1''(t)t+C_1'(t)-C_1'(t)t=0,$$
(2)
then the previous equation reduces to
$$C_2''(t)=3$$
(3)
The aim now is to solve this system of equations. Solve equation (2) first for $C_1(t).$ Divide both
sides of it by $t.$
$$C_1''(t)+\left(\dfrac{1}{t}-1\right)C_1'(t)=0$$

Use an integrating factor $I_{1}$ to solve it.
$$I_1=\exp\left[\int^t\left(\dfrac{1}{s}-1\right)ds\right]=e^{\ln t-t}=te^{-t}$$
Multiply both sides of the previous equation by $I_{1}.$
$$te^{-t}C_1''(t)+e^{-t}(1-t)C_1'(t)=0$$
The left side can be written as $d/dt[I_1C_1^{\prime}(t)]$ by the product rule.
$$\frac{d}{dt}[te^{-t}C_1'(t)]=0$$
Integrate both sides with respect to $t$, setting the integration constant to zero
$$te^{-t}C_1'(t)=0$$
Divide both sides by $te^-t.$
$$C_1'(t)=0$$
Integrate both sides with respect to $t$ once more, setting the integration constant to zero.
$$C_1(t)=0$$
Now solve equation (3) for $C_2(t).$ Integrate both sides of it with respect to $t$,setting the
integration constant to zero.
$$C_2'(t)=3t$$
Integrate both sides of it with respect to $t$ once more, setting the integration constant to zero.
$$C_2(t)=\dfrac{3}{2}t^2$$
Consequently, the particular solution is
$$\begin{aligned}y_p(t)&=C_1(t)te^{-t}+C_2(t)e^{-t}\\&=\frac{3}{2}t^2e^{-t}.\end{aligned}$$
Therefore,
$$\begin{aligned}y(t)&=y_c(t)+y_p(t)\\&=C_1te^{-t}+C_2e^{-t}+\frac{3}{2}t^2e^{-t}.\end{aligned}$$


$\underline{\text{Method of Undetermined Coefficients}}$

The particular solution satisfies
$$y_p''+2y_p'+y_p=3e^{-t}$$
Since the inhomogeneous term is an exponential function, we would use $y_p(t)=Ae^{-t}$ for the trial solution. However, since $e^-t$ satisfies equation (1), an extra factor of $t$ is needed. Actually, since $te^{-t}$ also satisfies equation (1), one more factor of $t$ is needed. Use $y_p(t)=At^2e^-t$ for the trial solution. Substitute this into the ODE to determine $A.$
$$(At^2e^{-t})''+2(At^2e^{-t})'+(At^2e^{-t})=3e^{-t}$$
Evaluate the derivatives.
$$(2Ate^{-t}-At^2e^{-t})'+2(2Ate^{-t}-At^2e^{-t})+(At^2e^{-t})=3e^{-t}$$
$$(2Ae^{-t}-2Ate^{-t}-2Ate^{-t}+At^2e^{-t})+2(2Ate^{-t}-At^2e^{-t})+(At^2e^{-t})=3e^{-t}$$
$$2Ae^{-t}-2Ate^t-2Ate^t+At^2e^{-t}+4Ate^t-2At^2e^{-t}+At^2e^{-t}=3e^{-t}$$
$$2Ae^{-t}=3e^{-t}$$
For this equation to be true, $A$ must satisfy $2A=3$, which means $A=3/2.$ That means the

particular solution is
$$y_p(t)=\frac{3}{2}t^2e^{-t}.$$
Therefore,
$$\begin{aligned}y(t)&=y_c(t)+y_p(t)\\&=C_{1}te^{-t}+C_{2}e^{-t}+\frac{3}{2}t^{2}e^{-t}.\end{aligned}$$


### Q5

The general solution to the ODE $y'' + 9y = 9 \sec^2(3t)$ can be expressed as the sum of the complementary solution $y_c(t)$ and the particular solution $y_p(t)$:

$$ y(t) = y_c(t) + y_p(t) $$

### Complementary Solution
The complementary solution satisfies the homogeneous equation:

$$ y''_c + 9y_c = 0 $$

Assume $y_c = e^{rt}$. Then:

$$ r^2 e^{rt} + 9 e^{rt} = 0 $$

Dividing by $e^{rt}$:

$$ r^2 + 9 = 0 $$

$$ r = \pm 3i $$

Thus, the complementary solution is:

$$ y_c(t) = C_1 e^{-3it} + C_2 e^{3it} $$

Using Euler's formula:

$$ y_c(t) = C_3 \cos(3t) + C_4 \sin(3t) $$

### Particular Solution
By the method of variation of parameters, assume:

$$ y_p(t) = C_3(t) \cos(3t) + C_4(t) \sin(3t) $$

Substitute into the ODE:

$$ y''_p + 9y_p = 9 \sec^2(3t) $$

After differentiating and substituting, solve for $C_3(t)$ and $C_4(t)$:

$$ C_4(t) = 0 $$

$$ C''_3(t) - 6 \frac{\sin(3t)}{\cos(3t)} C'_3(t) = 9 \sec(3t) $$

Solve using integrating factors:

$$ I_2 = \exp \left( \int -6 \frac{\sin(3s)}{\cos(3s)} ds \right) = \cos^2(3t) $$

Multiply both sides by $I_2$:

$$ \frac{d}{dt} \left( \cos^2(3t) C'_3(t) \right) = 9 \sec(3t) $$

Integrate both sides:

$$ (\cos^2(3t) C'_3(t)) = 9 \int \sec(3t) dt $$

$$ C'_3(t) = 3 (\sec^2(3t)) \ln (\sec(3t) + \tan(3t)) $$

Integrate again:

$$ C_3(t) = \int 3 (\sec^2(3t)) \ln (\sec(3t) + \tan(3t)) ds $$

$$ C_3(t) = \frac{1}{2} \left( -\frac{\cos^2(3t) + 1 + 2 \sin(3t) + \sin^2(3t)}{1 + \sin(3t)} \ln (\sec(3t) + \tan(3t)) - \frac{\cos^2(3t) + 1 + 2 \sin(3t) + \sin^2(3t)}{1 + \sin(3t)} \right) $$

### General Solution
$$ y(t) = y_c(t) + y_p(t) $$

$$ y(t) = C_3 \cos(3t) + C_4 \sin(3t) + \frac{1}{2} \left( -\frac{\cos^2(3t) + 1 + 2 \sin(3t) + \sin^2(3t)}{1 + \sin(3t)} \ln (\sec(3t) + \tan(3t)) - \frac{\cos^2(3t) + 1 + 2 \sin(3t) + \sin^2(3t)}{1 + \sin(3t)} \right) $$



### Q8

### Complementary Solution
The complementary solution satisfies the homogeneous equation:

$$ y''_c - 2y'_c + y_c = 0 $$

Assume $y_c = e^{rt}$. Then:

$$ r^2 e^{rt} - 2r e^{rt} + e^{rt} = 0 $$

Dividing by $e^{rt}$:

$$ r^2 - 2r + 1 = 0 $$

$$ (r - 1)^2 = 0 $$

$$ r = 1 $$

Thus, the complementary solution is:

$$ y_c(t) = (C_1 t + C_2) e^t $$

### Particular Solution
By the method of variation of parameters, assume:

$$ y_p(t) = C_1(t) t e^t + C_2(t) e^t $$

Substitute into the ODE:

$$ y''_p - 2y'_p + y_p = \frac{e^t}{1 + t^2} $$

After differentiating and substituting, solve for $C_1(t)$ and $C_2(t)$:

$$ C_2(t) = 0 $$

$$ t C''_1(t) + 2 C'_1(t) = \frac{1}{t (1 + t^2)} $$

Solve using integrating factors:

$$ I_1 = \exp \left( \int \frac{2}{t} dt \right) = t^2 $$

Multiply both sides by $I_1$:

$$ t^2 C''_1(t) + 2t C'_1(t) = \frac{t}{1 + t^2} $$

The left side can be written as:

$$ \frac{d}{dt} [t^2 C'_1(t)] = \frac{t}{1 + t^2} $$

Integrate both sides:

$$ t^2 C'_1(t) = \frac{1}{2} \ln (1 + t^2) $$

Divide by $t^2$:

$$ C'_1(t) = \frac{\ln (1 + t^2)}{2t^2} $$

Integrate again:

$$ C_1(t) = \int \frac{\ln (1 + t^2)}{2t^2} dt $$

Simplify using integration by parts:

$$ C_1(t) = t^{-1} \tan^{-1} t - \ln \sqrt{1 + t^2} $$

### General Solution
$$ y(t) = y_c(t) + y_p(t) $$

$$ y(t) = (C_1 t + C_2) e^t + \left( t^{-1} \tan^{-1} t - \ln \sqrt{1 + t^2} \right) t e^t $$

Therefore,

$$ y(t) = (C_1 t + C_2) e^t + t e^t \tan^{-1} t - e^t \ln \sqrt{1 + t^2} $$



### Q 15

### Verifying $y_1(x) = x^{-1/2} \sin x$
$$ y_1'' = x^{-1/2} \left( -\frac{3}{4} x^{-2} \sin x - x^{-1} \cos x \right) $$
$$ y_1' = x^{-1/2} \left( \cos x - \frac{1}{2} x^{-1} \sin x \right) $$
$$ x^2 y_1'' + x y_1' + (x^2 - 0.25) y_1 = 0 $$
Verification holds as the sum is zero.

### Verifying $y_2(x) = x^{-1/2} \cos x$
$$ y_2'' = x^{-1/2} \left( -\frac{3}{4} x^{-2} \cos x + x^{-1} \sin x \right) $$
$$ y_2' = x^{-1/2} \left( -\sin x - \frac{1}{2} x^{-1} \cos x \right) $$
$$ x^2 y_2'' + x y_2' + (x^2 - 0.25) y_2 = 0 $$
Verification holds as the sum is zero.

### General Solution
Since the ODE is linear, the general solution can be expressed as:
$$ y(x) = y_c(x) + y_p(x) $$
$$ y_c(x) = C_1 x^{-1/2} \sin x + C_2 x^{-1/2} \cos x $$

### Particular Solution
Assume:
$$ y_p(x) = C_1(x) x^{-1/2} \sin x + C_2(x) x^{-1/2} \cos x $$
Substitute into the nonhomogeneous equation:
$$ x^2 y''_p + xy'_p + (x^2 - 0.25)y_p = 3x^{3/2} \sin x $$
Evaluate derivatives and simplify:
$$ (C_1' x^{-1/2} \sin x + C_2' x^{-1/2} \cos x) + x^{-1/2} \cos x (C_1' x^{-1/2} \sin x - \frac{1}{2} x^{-3/2} \cos x) + x^{-1/2} \sin x (C_2' x^{-1/2} \cos x + \frac{1}{2} x^{-3/2} \sin x) = 3x^{3/2} \sin x $$

Divide by $x^{3/2}$:
$$ (C_1' \sin x + C_2' \cos x) + x^{-1/2} \left( \cos x \frac{\sin x - \frac{1}{2} \cos x}{x^{1/2}} + \sin x \frac{\cos x + \frac{1}{2} \sin x}{x^{1/2}} \right) = 3 \sin x $$

Solve for $C_1(x)$ and $C_2(x)$ using integrating factors:
$$ C_2(x) = 0 $$
$$ C_1(x) = -\frac{3}{2} x \cot x $$

### Final Particular Solution
$$ y_p(x) = -\frac{3}{2} x^{-1/2} \cos x $$

### General Solution
$$ y(x) = y_c(x) + y_p(x) $$
$$ y(x) = C_1 x^{-1/2} \sin x + C_2 x^{-1/2} \cos x - \frac{3}{2} x^{-1/2} \cos x $$
$$ y(x) = x^{-1/2} \left( C_1 \sin x + \left( C_2 - \frac{3}{2} \right) \cos x \right) $$


## Section 6.1

### Q2


![](https://img.simpletex.net/pdf/BzBdZgAg/fCnohkAOAvC4HbDSWGvVccx5HPEwO0fuE.png)
	                                                       $t$

This function is neither continuous nor piecewise continuous because it becomes infinite at $t=1.$

### Q3\


![](https://img.simpletex.net/pdf/BzBdZgAg/fZA0gzPCW6Zclh1fPcRUQ3FqiClLgqYSu.png)

This function is continuous because the limit of the function at every value of $t$ is the same from the left as it is from the right. In other words, there are no points of discontinuity.

### Q5

Find the Laplace transform of cos $at.$
$$\begin{aligned}\mathcal{L}\{\cos at\}&=\int_0^\infty e^{-st}\cos at\:dt\\&=\int_0^\infty e^{-st}\frac{e^{iat}+e^{-iat}}2\:dt\\&=\frac12\int_0^\infty e^{-st}(e^{iat}+e^{-iat})\:dt\\&=\frac12\left(\int_0^\infty e^{iat-st}\:dt+\int_0^\infty e^{-iat-st}\:dt\right)\\&=\frac12\left[\int_0^\infty e^{(a-s)t}\:dt+\int_0^\infty e^{(-ia-s)t}\:dt\right]\\&=\frac12\left[\left.\frac1{ia-s}e^{(ia-s)t}\right|_0^\infty+\left.\frac1{-ia-s}e^{(-ia-s)t}\right|_0^\infty\right]\\&=\frac12\left[\frac1{ia-s}(-1)+\frac1{-ia-s}(-1)\right]\\&=\frac12\left(\frac1{s-ia}+\frac1{s+ia}\right)\\&=\frac12\left[\frac{s+ia+s-ia}{(s-ia)(s+ia)}\right]\\&=\frac12\left(\frac{2s}{s^2-i^2a^2}\right)\\&=\frac s{s^2+a^2}\end{aligned}$$
where $s > 0$.
### Q6

### $\operatorname{Solution}$


Find the Laplace transform of cosh $bt.$
$$\begin{aligned}\{\cosh bt\}&=\int_0^\infty e^{-st}\cosh bt\:dt\\&=\int_0^\infty e^{-st}\frac{e^{bt}+e^{-bt}}{2}\:dt\\&=\frac12\int_0^\infty e^{-st}(e^{bt}+e^{-bt})\:dt\\&=\frac12\left(\int_0^\infty e^{bt-st}\:dt+\int_0^\infty e^{-bt-st}\:dt\right)\\&=\frac12\left[\int_0^\infty e^{(b-s)t}\:dt+\int_0^\infty e^{(-b-s)t}\:dt\right]\\&=\frac12\left[\frac1{b-s}e^{(b-s)t}\right|_0^\infty+\left.\frac1{-b-s}e^{(-b-s)t}\right|_0^\infty\\&=\frac12\left[\frac1{b-s}(-1)+\frac1{-b-s}(-1)\right]\\&=\frac12\left(\frac1{s-b}+\frac1{s+b}\right)\\&=\frac12\left[(s+b+s-b)\right]\\&=\frac12\left(\frac{2s}{s^2-b^2}\right)\\&=\frac s{s^2-b^2}\end{aligned}$$
where $b-s<0$ and $-b-s<0$

### Q9

$$\begin{aligned}
&&\mathcal{L}\{\operatorname{cos}bt\}& =\int_0^\infty e^{-st}\cos bt dt \\
&&&=\int_0^\infty e^{-st}\frac{e^{ibt}+e^{-ibt}}{2} dt \\
&&&=\frac{1}{2}\int_{0}^{\infty}e^{-st}(e^{ibt}+e^{-ibt}) dt \\
&&&\begin{aligned}=\frac{1}{2}\left(\int_{0}^{\infty}e^{ibt-st} dt+\int_{0}^{\infty}e^{-ibt-st} dt\right)\end{aligned} \\
&&&=\frac{1}{2}\left[\int_{0}^{\infty}e^{(ib-s)t} dt+\int_{0}^{\infty}e^{(-ib-s)t} dt\right] \\
&&&=\frac{1}{2}\left[\left.\frac{1}{ib-s}e^{(ib-s)t}\right|_{0}^{\infty}+\left.\frac{1}{-ib-s}e^{(-ib-s)t}\right|_{0}^{\infty}\right] \\
&&&=\frac{1}{2}\left[\frac{1}{ib-s}(-1)+\frac{1}{-ib-s}(-1)\right] \\
&&&=\frac{1}{2}\left(\frac{1}{s-ib}+\frac{1}{s+ib}\right) \\
&&&=\frac{1}{2}\left[\frac{s+ib+s-ib}{(s-ib)(s+ib)}\right] \\
&&&=\frac{1}{2}\left(\frac{2s}{s^2-i^2b^2}\right) \\
&&&=\frac{s}{s^2+b^2} \\
\end{aligned}$$



### Q23

$\underline{\text{Part }(\mathrm{a})}$

Use integration by parts in the definition of the gamma function.
$$\begin{aligned}\Gamma(p+1)&=\int_0^\infty e^{-x}x^p\:dx\\&=\int_0^\infty\frac d{dx}(-e^{-x})x^p\:dx\\&=\left.(-e^{-x})x^p\right|_0^\infty-\int_0^\infty(-e^{-x})px^{p-1}\:dx\\&=p\int_0^\infty e^{-x}x^{p-1}\:dx\\&=p\Gamma(p)\end{aligned}$$
Note that l'Hôpital's rule can be applied Ceiling$(p)$ (that is, $p$ rounded up to the nearest integer)
times to show that the limit of $(-e^{-x})x^p$ as $x\to\infty$ is zero.

$\underline{\text{Part }(\mathrm{b})}$


Set $p=0$ to get $\Gamma(1)$ in the definition.
$$\begin{aligned}\Gamma(0+1)&=\int_0^\infty e^{-x}x^0\:dx\\\Gamma(1)&=\int_0^\infty e^{-x}\:dx\\&=\left.-e^{-x}\right|_0^\infty\\&=\lim_{x\to\infty}(-e^{-x})-(-e^0)\\&=0+1\\&=1\end{aligned}$$
$\textbf{Part ( c) }$

Set $p=n$ in the result of part (a) and use it over and over again until $\Gamma(1)$ is reached. Then use
the result of part (b).
$$\begin{aligned}\Gamma(n+1)&=n\Gamma(n)\\&=n[(n-1)\Gamma(n-1)]\\&=n(n-1)\Gamma(n-1)\\&=n(n-1)[(n-2)\Gamma(n-2)]\\&=n(n-1)(n-2)\Gamma(n-2)\\&=n(n-1)(n-2)[(n-3)\Gamma(n-3)]\\&=n(n-1)(n-2)(n-3)\Gamma(n-3)\\&\vdots\\&=n(n-1)(n-2)(n-3)\cdots(3)(2)(1)\Gamma(1)\\&=n(n-1)(n-2)(n-3)\cdots(3)(2)(1)(1)\\&=n(n-1)(n-2)(n-3)\cdots(3)(2)(1)\\&=n!\end{aligned}$$


$$\begin{aligned}
&\underline{\text{Part (d)}} \\
&\mathrm{Use~the~result~of~part~(a)~in}&& \mathrm{the~numerator~over~and~over~again~until~}\Gamma(p)\mathrm{~is~reached.} \\
&&&\frac{\Gamma(p+n)}{\Gamma(p)} =\frac{(p+n-1)\Gamma(p+n-1)}{\Gamma(p)} \\
&&&=\frac{(p+n-1)(p+n-2)\Gamma(p+n-2)}{\Gamma(p)} \\
&&&=\frac{(p+n-1)(p+n-2)\cdots(p+2)\Gamma(p+2)}{\Gamma(p)} \\
&&&=\frac{(p+n-1)(p+n-2)\cdots(p+2)(p+1)\Gamma(p+1)}{\Gamma(p)} \\
&&&=\frac{(p+n-1)(p+n-2)\cdots(p+2)(p+1)p\Gamma(p)}{\Gamma(p)} \\
&&&=(p+n-1)(p+n-2)\cdots(p+2)(p+1)p \\
&\mathrm{Find~}\Gamma\left(\frac{3}{2}\right). \\
&&&\frac{\Gamma\left(\frac{1}{2}+1\right)}{\Gamma\left(\frac{1}{2}\right)} =\left(\frac12+1-1\right) \\
&&&\frac{\Gamma\left(\frac{3}{2}\right)}{\sqrt{\pi}} =\frac12 \\
&&&\Gamma\left(\frac{3}{2}\right) =\frac{\sqrt{\pi}}2 \\
&\mathrm{Find~}\Gamma\left(\frac{11}{2}\right). \\
&\frac{\Gamma\left(\frac{1}{2}+5\right)}{\Gamma\left(\frac{1}{2}\right)}&& =\left(\frac{1}{2}+5-1\right)\left(\frac{1}{2}+4-1\right)\left(\frac{1}{2}+3-1\right)\left(\frac{1}{2}+2-1\right)\left(\frac{1}{2}+1-1\right) \\
&\frac{\Gamma\left(\frac{11}{2}\right)}{\sqrt{\pi}}&& =\left(\frac92\right)\left(\frac72\right)\left(\frac52\right)\left(\frac32\right)\left(\frac12\right) \\
&\Gamma\left(\frac{11}{2}\right)&& =\frac{945}{32}\sqrt{\pi} 
\end{aligned}$$

### Q24

$\underline{\text{Part (a)}}$

Start by using the definition of the Laplace transform.
$$\mathcal{L}\{t^p\}=\int_0^\infty e^{-st}t^p\:dt$$
For this integral to converge, it must be the case that $s>0.$ Make the substitution $x=st.$ Then

$dx= s$ $dt.$
$$\begin{aligned}\mathcal{L}\{t^{p}\}&=\int_0^\infty e^{-x}\left(\frac xs\right)^p\frac{dx}s\\&=\int_0^\infty e^{-x}\frac{x^p}{s^p}\:\frac{dx}s\\&=\frac1{s^{p+1}}\int_0^\infty e^{-x}x^p\:dx\\&=\frac1{s^{p+1}}\Gamma(p+1)\end{aligned}$$

$\underline{\mathrm{Part~(b)}}$

Suppose now that $p$ is a positive integer $n.$
$$\begin{aligned}\mathcal{L}\{t^n\}&=\frac1{s^{n+1}}\Gamma(n+1)\\&=\frac1{s^{n+1}}n\Gamma(n)\\&=\frac1{s^{n+1}}n(n-1)\Gamma(n-1)\\&=\frac1{s^{n+1}}n(n-1)(n-2)\Gamma(n-2)\\&=\frac1{s^{n+1}}n(n-1)(n-2)\cdots(3)(2)\Gamma(2)\\&=\frac1{s^{n+1}}n(n-1)(n-2)\cdots(3)(2)(1)\Gamma(1)\\&=\frac1{s^{n+1}}n(n-1)(n-2)\cdots(3)(2)(1)(1)\\&=\frac1{s^{n+1}}n(n-1)(n-2)\cdots(3)(2)(1)\\&=\frac1{s^{n+1}}n!\end{aligned}$$
$\underline{\text{Part }(\mathrm{c})}$

Plug in $p=-1/2$ in the result of part (a).
$$\begin{aligned}\mathcal{L}\{t^{-1/2}\}&=\frac1{s^{-\frac12+1}}\Gamma\left(-\frac12+1\right)\\&=\frac1{s^{1/2}}\Gamma\left(\frac12\right)\\&=\frac1{s^{1/2}}\sqrt{\pi}\\&=\sqrt{\frac\pi s}\end{aligned}$$
Alternatively, use the definition of the Laplace transform once again.
$$\mathcal{L}\{t^{-1/2}\}=\int_0^\infty e^{-st}t^{-1/2}\:dt$$


Make the substitution $x^{2}= st.$Then $2xdx= s$ $dt.$
$$\begin{aligned}\mathcal{L}\{t^{-1/2}\}&=\int_0^\infty e^{-x^2}\left(\frac{x^2}s\right)^{-1/2}\frac{2x\:dx}s\\&=\int_0^\infty e^{-x^2}\left(\frac s{x^2}\right)^{1/2}\frac{2x\:dx}s\\&=\int_0^\infty e^{-x^2}\left(\frac{s^{1/2}}x\right)\frac{2x\:dx}s\\&=\int_0^\infty e^{-x^2}\frac{2\:dx}{s^{1/2}}\\&=\frac2{\sqrt{s}}\int_0^\infty e^{-x^2}\:dx\\&=\frac2{\sqrt{s}}\frac{\sqrt{\pi}}2\\&=\sqrt{\frac\pi s}\end{aligned}$$
$\underline{\text{Part }(\mathrm{d})}$

Plug in $p=1/2$ in the result of part (a)
$$\begin{aligned}\mathcal{L}\{t^{1/2}\}&=\frac1{s^{\frac12+1}}\Gamma\left(\frac12+1\right)\\&=\frac1{s^{3/2}}\Gamma\left(\frac32\right)\\&=\frac1{s^{3/2}}\frac{\sqrt{\pi}}2\\&=\frac{\sqrt{\pi}}{2s^{3/2}}\end{aligned}$$
Alternatively, we can use the following property of the Laplace transform.
$$\mathcal{L}\{tf(t)\}=-\frac{d}{ds}F(s)$$
Doing so gives
$$\begin{aligned}\mathcal{L}\{t^{1/2}\}&=\mathcal{L}\{t\cdot t^{-1/2}\}\\&=-\frac d{ds}\mathcal{L}\{t^{-1/2}\}\\&=-\frac d{ds}\left(\sqrt{\frac\pi s}\right)\\&=-\left(-\frac{\sqrt{\pi}}{2s^{3/2}}\right)\\&=\frac{\sqrt{\pi}}{2s^{3/2}}.\end{aligned}$$




## Section 6.2

### Q3

Factor the denominator.
$$\begin{aligned}F(s)&=\frac2{s^2+3s-4}\\&=\frac2{(s+4)(s-1)}\\&=\frac{2/5}{s-1}-\frac{2/5}{s+4}\end{aligned}$$
Take the inverse Laplace transform now to get $f(t).$
$$f(t)=\frac25e^t-\frac25e^{-4t}$$
### Q8

Because the ODE is linear, the Laplace transform can be applied to solve it. Consequently, the first and second derivatives transform as follows.
$$\begin{aligned}\mathcal{L}\left\{\frac{dy}{dt}\right\}&=sY(s)-y(0)\\\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\}&=s^2Y(s)-sy(0)-y'(0)\end{aligned}$$
Apply the Laplace transform to both sides of the ODE.
$$\mathcal{L}\{y''-y'-6y\}=\mathcal{L}\{0\}$$
Use the fact that the transform is a linear operator.
$$\mathcal{L}\{y''\}-\mathcal{L}\{y'\}-6\mathcal{L}\{y\}=0$$
$$[s^2Y(s)-sy(0)-y'(0)]-[sY(s)-y(0)]-6Y(s)=0$$
Plug in the initial conditions, $y(0)=1$ and $y^\prime(0)=-1.$
$$[s^2Y(s)-s+1]-[sY(s)-1]-6Y(s)=0$$
As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for
$Y$, the transformed solution.
$$s^2Y(s)-sY(s)-6Y(s)-s+2=0$$
$$\begin{matrix}(s^2-s-6)Y(s)=s-2\end{matrix}$$
$$\begin{aligned}Y(s)&=\frac{s-2}{s^{2}-s-6}\\&=\frac{s-2}{(s-3)(s+2)}\\&=\frac{1/5}{s-3}+\frac{4/5}{s+2}\end{aligned}$$


### Q9

Because the ODE is linear, the Laplace transform can be applied to solve it. 
Consequently, the first and second derivatives transform as follows.
$$\begin{aligned}\mathcal{L}\left\{\frac{dy}{dt}\right\}&=sY(s)-y(0)\\\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\}&=s^2Y(s)-sy(0)-y'(0)\end{aligned}$$
Apply the Laplace transform to both sides of the ODE.
$$\mathcal{L}\{y''+3y'+2y\}=\mathcal{L}\{0\}$$
Use the fact that the transform is a linear operator.
$$\mathcal{L}\{y''\}+3\mathcal{L}\{y'\}+2\mathcal{L}\{y\}=0$$
$$[s^2Y(s)-sy(0)-y'(0)]+3[sY(s)-y(0)]+2Y(s)=0$$
Plug in the initial conditions, $y(0)=1$ and $y^\prime(0)=0.$
$$[s^2Y(s)-s]+3[sY(s)-1]+2Y(s)=0$$
As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for
$Y$, the transformed solution.
$$s^{2}Y(s)+3sY(s)+2Y(s)-s-3=0\\(s^{2}+3s+2)Y(s)=s+3$$
$$\begin{aligned}Y(s)&=\frac{s+3}{s^{2}+3s+2}\\&=\frac{s+3}{(s+2)(s+1)}\\&=\frac{-1}{s+2}+\frac{2}{s+1}\end{aligned}$$
Take the inverse Laplace transform of $Y(s)$ now to recover $y(t).$
$$\begin{aligned}y(t)&=\mathcal{L}^{-1}\{Y(s)\}\\&=\mathcal{L}^{-1}\left\{\frac{-1}{s+2}+\frac2{s+1}\right\}\\&=-\mathcal{L}^{-1}\left\{\frac1{s+2}\right\}+2\mathcal{L}^{-1}\left\{\frac1{s+1}\right\}\\&=-e^{-2t}+2e^{-t}\end{aligned}$$

![](https://img.simpletex.net/pdf/BzBdZgAg/fqwQmALbrXl1cbdyXrWVxaNhpLKK130zo.png)

### Q13


Because the ODE is linear, the Laplace transform can be applied to solve it. Consequently, the derivatives transform as follows.
$$\begin{aligned}&\mathcal{L}\left\{\frac{dy}{dt}\right\}=sY(s)-y(0)\\&\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\}=s^2Y(s)-sy(0)-y'(0)\\&\mathcal{L}\left\{\frac{d^3y}{dt^3}\right\}=s^3Y(s)-s^2y(0)-sy'(0)-y''(0)\\&\mathcal{L}\left\{\frac{d^4y}{dt^4}\right\}=s^4Y(s)-s^3y(0)-s^2y'(0)-sy''(0)-y'''(0)\end{aligned}$$
Apply the Laplace transform to both sides of the ODE.
$$\mathcal{L}\{y^{(4)}-4y''''+6y''-4y'+y\}=\mathcal{L}\{0\}$$
Use the fact that the transform is a linear operator.
$$\mathcal{L}\{y^{(4)}\}-4\mathcal{L}\{y^{\prime\prime\prime}\}+6\mathcal{L}\{y^{\prime\prime}\}-4\mathcal{L}\{y^{\prime}\}+\mathcal{L}\{y\}=0$$
$$\begin{aligned}[s^4Y(s)-s^3y(0)-s^2y'(0)-sy''(0)-y'''(0)]&-4[s^3Y(s)-s^2y(0)-sy'(0)-y''(0)]\\&+6[s^2Y(s)-sy(0)-y'(0)]-4[sY(s)-y(0)]+Y(s)=0\end{aligned}$$
Plug in the initial conditions, $y(0)=0,y^\prime(0)=1,y^{\prime\prime}(0)=0$, and $y^\prime\prime\prime(0)=1.$
$$[s^4Y(s)-s^2-1]-4[s^3Y(s)-s]+6[s^2Y(s)-1]-4[sY(s)]+Y(s)=0$$
As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for
$Y$, the transformed solution.
$$s^4Y(s)-4s^3Y(s)+6s^2Y(s)-4sY(s)+Y(s)-s^2-1+4s-6=0$$
$$(s^4-4s^3+6s^2-4s+1)Y(s)=s^2-4s+7$$
$$\begin{aligned}Y(s)&=\frac{s^2-4s+7}{s^4-4s^3+6s^2-4s+1}\\&=\frac{s^2-4s+7}{(s-1)^4}\\&=\frac1{(s-1)^2}-\frac2{(s-1)^3}+\frac4{(s-1)^4}\\&=\frac1{(s-1)^2}-\frac2{(s-1)^3}+\frac46\frac6{(s-1)^4}\end{aligned}$$
Take the inverse Laplace transform of $Y(s)$ now to recover $y(t).$
$$\begin{aligned}y(t)&=\mathcal{L}^{-1}\{Y(s)\}\\&=\mathcal{L}^{-1}\left\{\frac1{(s-1)^2}-\frac2{(s-1)^3}+\frac46\frac6{(s-1)^4}\right\}\\&=\mathcal{L}^{-1}\left\{\frac1{(s-1)^2}\right\}-\mathcal{L}^{-1}\left\{\frac2{(s-1)^3}\right\}+\frac46\mathcal{L}^{-1}\left\{\frac6{(s-1)^4}\right\}\\&=te^t-t^2e^t+\frac46t^3e^t\\&=\frac13te^t\left(3-3t+2t^2\right)\end{aligned}$$
![[Pasted image 20240716202307.png]]
### Q14


Because the ODE is linear, the Laplace transform can be applied to solve it. Consequently, the derivatives transform as follows.
$$\begin{aligned}&\mathcal{L}\left\{\frac{dy}{dt}\right\}=sY(s)-y(0)\\&\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\}=s^2Y(s)-sy(0)-y'(0)\\&\mathcal{L}\left\{\frac{d^3y}{dt^3}\right\}=s^3Y(s)-s^2y(0)-sy'(0)-y''(0)\\&\mathcal{L}\left\{\frac{d^4y}{dt^4}\right\}=s^4Y(s)-s^3y(0)-s^2y'(0)-sy''(0)-y''''(0)\end{aligned}$$
Apply the Laplace transform to both sides of the ODE.
$$\mathcal{L}\{y^{(4)}-y\}=\mathcal{L}\{0\}$$
Use the fact that the transform is a linear operator.
$$\mathcal{L}\{y^{(4)}\}-\mathcal{L}\{y\}=0$$
$$[s^{4}Y(s)-s^{3}y(0)-s^{2}y^{\prime}(0)-sy^{\prime\prime}(0)-y^{\prime\prime\prime}(0)]-Y(s)=0$$
Plug in the initial conditions, $y(0)=1,y^\prime(0)=0,y^{\prime\prime}(0)=1$, and $y^\prime\prime\prime(0)=0.$
$$[s^4Y(s)-s^3-s]-Y(s)=0$$
As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for

$Y$, the transformed solution.
$$s^{4}Y(s)-Y(s)-s^{3}-s=0\\(s^{4}-1)Y(s)=s^{3}+s$$
$$\begin{aligned}Y(s)&=\frac{s^3+s}{s^4-1}\\&=\frac{s(s^2+1)}{(s+1)(s-1)(s^2+1)}\\&=\frac s{(s+1)(s-1)}\\&=\frac{1/2}{s+1}+\frac{1/2}{s-1}\end{aligned}$$


Take the inverse Laplace transform of $Y(s)$ now to recover $y(t).$
$$\begin{aligned}y(t)&=\mathcal{L}^{-1}\{Y(s)\}\\&=\mathcal{L}^{-1}\left\{\frac{1/2}{s+1}+\frac{1/2}{s-1}\right\}\\&=\frac12\mathcal{L}^{-1}\left\{\frac1{s+1}\right\}+\frac12\mathcal{L}^{-1}\left\{\frac1{s-1}\right\}\\&=\frac12e^{-t}+\frac12e^t\\&=\frac{e^{-t}+e^t}2\\&=\cosh t\end{aligned}$$
![[Pasted image 20240716202555.png]]
### Q16

Because the ODE is linear, the Laplace transform can be applied to solve it. Consequently, the first and second derivatives transform as follows.
$$\begin{aligned}\mathcal{L}\left\{\frac{dy}{dt}\right\}&=sY(s)-y(0)\\\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\}&=s^2Y(s)-sy(0)-y'(0)\end{aligned}$$
Apply the Laplace transform to both sides of the ODE.
$$\mathcal{L}\{y''-2y'+2y\}=\mathcal{L}\{e^{-t}\}$$
Use the fact that the transform is a linear operator.
$$\mathcal{L}\{y''\}-2\mathcal{L}\{y'\}+2\mathcal{L}\{y\}=\mathcal{L}\{e^{-t}\}$$
$$[s^2Y(s)-sy(0)-y'(0)]-2[sY(s)-y(0)]+2Y(s)=\dfrac{1}{s+1}$$
Plug in the initial conditions, $y(0)=0$ and $y^\prime(0)=1.$
$$[s^2Y(s)-1]-2[sY(s)]+2Y(s)=\dfrac{1}{s+1}$$
As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for
$Y$, the transformed solution.
$$s^2Y(s)-2sY(s)+2Y(s)-1=\dfrac{1}{s+1}$$
$$\begin{aligned}(s^{2}-2s+2)Y(s)&=\frac{1}{s+1}+1\\&=\frac{s+2}{s+1}\end{aligned}$$
Divide both sides by $s^2-2s+2.$
$$Y(s)=\frac{s+2}{(s+1)(s^2-2s+2)}$$

Use partial fraction decomposition to write $Y(s)$ in terms of known transforms.
$$\begin{aligned}\frac{s+2}{(s+1)(s^2-2s+2)}=\frac{A}{s+1}+\frac{Bs+C}{s^2-2s+2}\end{aligned}$$
Multiply both sides by $(s+1)(s^2-2s+2).$
$$s+2=A(s^2-2s+2)+(Bs+C)(s+1)$$
Choose three random values for $s$ to get a system of equations for $A,B$,and $C.$
$$\begin{aligned}s&=0:&2&=2A+C\\s&=1:&3&=A+2B+2C\\s&=2:&4&=2A+6B+3C\end{aligned}$$
Solving this system yields
$$A=\frac{1}{5}\quad\mathrm{and}\quad B=-\frac{1}{5}\quad\mathrm{and}\quad C=\frac{8}{5},$$
so $Y(s)$ becomes
$$\begin{aligned}Y(s)&=\frac{\frac15}{s+1}+\frac{-\frac15s+\frac85}{s^2-2s+2}\\&=\frac15\frac1{s+1}-\frac15\frac{s-8}{s^2-2s+2}\\&=\frac15\frac1{s+1}-\frac15\frac{s-8}{s^2-2s+1+2-1}\\&=\frac15\frac1{s+1}-\frac15\frac{s-8}{(s-1)^2+1}\\&=\frac15\frac1{s+1}-\frac15\frac{s-1-8+1}{(s-1)^2+1}\\&=\frac15\frac1{s+1}-\frac15\frac{s-1-7}{(s-1)^2+1}\\&=\frac15\frac1{s+1}-\frac15\frac{s-1}{(s-1)^2+1}+\frac75\frac1{(s-1)^2+1}.\end{aligned}$$
Take the inverse Laplace transform of $Y(s)$ now to recover $y(t).$
$$\begin{aligned}y(t)&=\mathcal{L}^{-1}\{Y(s)\}\\&=\mathcal{L}^{-1}\left\{\frac15\frac1{s+1}-\frac15\frac{s-1}{(s-1)^2+1}+\frac75\frac1{(s-1)^2+1}\right\}\\&=\frac15\mathcal{L}^{-1}\left\{\frac1{s+1}\right\}-\frac15\mathcal{L}^{-1}\left\{\frac{s-1}{(s-1)^2+1}\right\}+\frac75\mathcal{L}^{-1}\left\{\frac1{(s-1)^2+1}\right\}\\&=\frac15e^{-t}-\frac15e^t\cos t+\frac75e^t\sin t\\&=\frac15[e^{-t}+e^t(7\sin t-\cos t)]\end{aligned}$$


![[Pasted image 20240716202811.png]]

## Section 6.3

### Q6

Write $f(t)$ in terms of the Heaviside function, $H(t)$, which is defined to be 1 if $t > 0$ and 0 if $t < 0$: $$ f(t) = 1[H(t) - H(t-1)] - 1[H(t-1) - H(t-2)] + 1[H(t-2) - H(t-3)] - 1[H(t-3) - H(t-4)] $$ Simplify: $$ f(t) = H(t) - 2H(t-1) + 2H(t-2) - 2H(t-3) + H(t-4) $$ Using unit step functions $u_c(t)$, we have: $$ f(t) = u_0(t) - 2u_1(t) + 2u_2(t) - 2u_3(t) + u_4(t) $$

![[Pasted image 20240716203044.png]]


### Q14

$$\begin{aligned}
&\text{Factor the denominator.} \\
&&&\begin{aligned}F(s)=\frac{1}{(s+2)(s-1)}e^{-2s}\end{aligned} \\
&\text{Partially decompose the fraction.} \\
&&&F(s)=\left(\frac{-\frac{1}{3}}{s+2}+\frac{\frac{1}{3}}{s-1}\right)e^{-2s} \\
&\begin{aligned}\text{Now take the inverse Laplace transform of }&F(s)\text{ to get }f(t).\end{aligned} \\
&&f(t)& =\mathcal{L}^{-1}\{F(s)\} \\
&&&=\mathcal{L}^{-1}\left\{\left(\frac{-\frac13}{s+2}+\frac{\frac13}{s-1}\right)e^{-2s}\right\} \\
&&&=\left[-\frac{1}{3}e^{-2(t-2)}+\frac{1}{3}e^{(t-2)}\right]H(t-2) \\
&&&=\frac{1}{3}\left[e^{t-2}-e^{-2(t-2)}\right]u_2(t)
\end{aligned}$$


### Q16

$$\begin{aligned}
&\text{Apply the two transforms,}&  \\
&&&\mathcal L\{t^{n}\}=\frac{n!}{s^{n+1}}\quad\mathrm{and}\quad\mathcal L\{f(t-c)H(t-c)\}=F(s)e^{-cs}, \\
&\text{together to solve this problem.} \\
&f(t&&& )=\mathcal{L}^{-1}\{F(s)\} \\
&&&&=\mathcal{L}^{-1}\left\{\frac{e^{-s}+e^{-2s}-e^{-3s}-e^{-4s}}s\right\} \\
&&&=\mathcal{L}^{-1}\begin{Bmatrix}1\\-e^{-s}\\s\end{Bmatrix}+\mathcal{L}^{-1}\begin{Bmatrix}1\\-e^{-2s}\\s\end{Bmatrix}-\mathcal{L}^{-1}\begin{Bmatrix}1\\-e^{-3s}\\s\end{Bmatrix}-\mathcal{L}^{-1}\begin{Bmatrix}1\\-e^{-4s}\\s\end{Bmatrix} \\
&&&=H(t-1)+H(t-2)-H(t-3)-H(t-4) \\
&&&=u_1(t)+u_2(t)-u_3(t)-u_4(t)
\end{aligned}$$

### Q17\

Part (a)

Suppose we use $f(ct)$ rather than $f(t)$.

$$
\mathcal{L}\{f(ct)\} = \int_0^{\infty} e^{-st} f(ct) \, dt.
$$

Make the substitution $x = ct$. Then $dx = c \, dt$.

$$
\mathcal{L}\{f(ct)\} = \int_0^{\infty} e^{-sx/c} f(x) \left( \frac{dx}{c} \right)
$$
$$
= \frac{1}{c} \int_0^{\infty} e^{-(s/c)x} f(x) \, dx
$$
$$
= \frac{1}{c} F \left( \frac{s}{c} \right)
$$


Part ( b) 

Suppose we use $(1/k)f(t/k)$ rather than $f(t).$
$$\mathcal{L}\left\{\dfrac{1}{k}f\left(\dfrac{t}{k}\right)\right\}=\int_0^\infty e^{-st}\dfrac{1}{k}f\left(\dfrac{t}{k}\right)dt$$
Make the substitution $x=t/k.$ Then $dx=dt/k.$
$$\begin{aligned}\mathcal{L}\left\{\frac{1}{k}f\left(\frac{t}{k}\right)\right\}&=\int_0^\infty e^{-s(kx)}\frac1kf(x)(k\:dx)\\&=\int_0^\infty e^{-(ks)x}f(x)\:dx\\&=F(ks)\end{aligned}$$
Therefore, taking the inverse Laplace transform of both sides,
$$\dfrac{1}{k}f\left(\dfrac{t}{k}\right)=\mathcal{L}^{-1}\{F(ks)\}.$$
$\underline{\text{Part }(\mathrm{c})}$

Suppose we use $(1/a)e^{-bt/a}f(t/a)$ rather than $f(t).$
$$\mathcal{L}\left\{\frac{1}{a}e^{-bt/a}f\left(\frac{t}{a}\right)\right\}=\int_0^\infty e^{-st}\frac{1}{a}e^{-bt/a}f\left(\frac{t}{a}\right)dt$$
Make the substitution $x=t/a.$ Then $dx=dt/a.$
$$\begin{aligned}\mathcal{L}\left\{\frac{1}{a}e^{-bt/a}f\left(\frac{t}{a}\right)\right\}&=\int_0^\infty e^{-s(ax)}\frac1ae^{-bx}f(x)(a\:dx)\\&=\int_0^\infty e^{-(as+b)x}f(x)\:dx\\&=F(as+b)\end{aligned}$$
Therefore, taking the inverse Laplace transform of both sides,
$$\begin{aligned}\frac{1}{a}e^{-bt/a}f\left(\frac{t}{a}\right)=\mathcal{L}^{-1}\{F(as+b)\}.\end{aligned}$$



### Q21
We split the integral accordingly:
$$
F(s) = \int_0^1 e^{-st} \cdot 1 \, dt + \int_1^\infty e^{-st} \cdot 0 \, dt
$$

Simplify:
$$
F(s) = \int_0^1 e^{-st} \, dt
$$

Evaluate the integral:
$$
F(s) = \left. -\frac{1}{s} e^{-st} \right|_0^1
$$

Substitute the limits:
$$
F(s) = -\frac{1}{s} e^{-s} + \frac{1}{s} e^0
$$
$$
F(s) = \frac{1}{s} - \frac{1}{s} e^{-s}
$$

Thus, the Laplace transform is:
$$
F(s) = \frac{1 - e^{-s}}{s}
$$


### Q22

$$
\begin{aligned}
\text{Of course, for this integral to converge, it's necessary that }s>0.\text{ Split up the integral over the} \\
\begin{aligned}\text{intervals that the given function is defined over.}\end{aligned} \\
F(s) \begin{aligned}=\int_0^1e^{-st}(1) dt+\int_1^2e^{-st}(0) dt+\int_2^3e^{-st}(1) dt+\int_3^\infty e^{-st}(0) dt\end{aligned} \\
\begin{aligned}=\int_{0}^{1}e^{-st} dt+\int_{2}^{3}e^{-st} dt\end{aligned} \\
=\left.-\frac1se^{-st}\right|_0^1\left.-\frac1se^{-st}\right|_2^3 \\
\begin{aligned}&=\frac1s-\frac1se^{-s}+\frac1se^{-2s}-\frac1se^{-3s}\end{aligned} \\
=\frac{1-e^{-s}+e^{-2s}-e^{-3s}}s
\end{aligned}
$$