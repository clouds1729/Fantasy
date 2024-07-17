
## 2.5
### Q3

$f(y)=y(y-1)(y-2).$ Below is a graph of $f(y)$ versus $y.$

![](https://img.simpletex.net/pdf/BzBdZgZi/fGhX9bnfLqmCO485uDVfU3aC4TYskzP2z.png)

The equilibrium points are found by solving $f(y)=0$ for $y.$
$$y(y-1)(y-2)=0$$
$$y=\{0,1,2\}$$
The open and closed circles represent unstable and stable equilibrium points, respectively. $y=0$
and $y=2$ are unstable while $y=1$ is stable.


![](https://img.simpletex.net/pdf/BzBdZgZi/fmnnIvgwVz84FEv5IRGxil4VGvUCYME4Q.png)

The arrows pointing left and right on the $y$-axis (phase line) mean that $y$ is decreasing and
increasing in time, respectively.


Some possible solution curves in the $ty$-plane for $t\geq0$ and $y\geq0$ are shown below. At every
point, they are tangent to the direction field vectors $\langle1,y(y-1)(y-2)\rangle.$

![](https://img.simpletex.net/pdf/BzBdZgZi/fwDohm4evt3nOCdIxEIOrI7gADVVbfYYh.png)


--------------------------------------------------------------------------

### Q22

$\mathbf{Solution}$

$\underline{\mathrm{Part~(a)}}$

$$\frac{dy}{dt}+\beta y=0$$
integrating factor $I.$
$$I=\exp\left(\int^t\beta\:ds\right)=e^{\beta t}$$
$$e^{\beta t}\frac{dy}{dt}+\beta e^{\beta t}y=0$$
$$\frac d{dt}(e^{\beta t}y)=0$$

$$e^{\beta t}y=A$$
$$y(t)=Ae^{-\beta t}$$
initial condition $y(0)=y_{0}$
$$y(0)=A=y_{0}\\y(t)=y_{0}e^{-\beta t}.$$


$\underline{\mathrm{Part~(b)}}$

$$\dfrac{dx}{dt}=-\alpha x(y_0e^{-\beta t})$$
$$\dfrac{dx}{x}=-\alpha y_0e^{-\beta t}\:dt$$
$$\begin{aligned}\ln|x|=\frac{\alpha}{\beta}y_0e^{-\beta t}+C\end{aligned}$$
$$\begin{aligned}|x|&=\exp\left(\frac{\alpha}{\beta}y_{0}e^{-\beta t}+C\right)\\&=e^C\exp\left(\frac{\alpha}{\beta}y_0e^{-\beta t}\right)\\\end{aligned}$$
$$x(t)=\pm e^C\exp\left(\frac{\alpha}{\beta}y_0e^{-\beta t}\right)$$$B$ =$\pm e^C.$
$$x(t)=B\exp\left(\frac{\alpha}{\beta}y_0e^{-\beta t}\right)$$
Initial condition $x(0)=x_0$ 
$$x(0)=B\exp\left(\frac{\alpha}{\beta}y_0\right)=x_0\quad\to\quad B=x_0\exp\left(-\frac{\alpha}{\beta}y_0\right)$$
The previous equation then becomes
$$x(t)=x_{0}\exp\left(-\frac{\alpha}{\beta}y_{0}\right)\exp\left(\frac{\alpha}{\beta}y_{0}e^{-\beta t}\right)\\=x_{0}\exp\left(-\frac{\alpha}{\beta}y_{0}+\frac{\alpha}{\beta}y_{0}e^{-\beta t}\right).$$
Thus,
$$x(t)=x_0\exp\left[-\dfrac{\alpha}{\beta}y_0(1-e^{-\beta t})\right]\quad\Rightarrow\quad\lim\limits_{t\to\infty}x(t)=x_0\exp\left[-\dfrac{\alpha}{\beta}y_0(1-0)\right]=x_0\exp\left(-\dfrac{\alpha}{\beta}y_0\right)$$


--------------------------------------------------------------------------

## 2.6

### Q1

The ODE is exact because
$$\frac\partial{\partial y}(2x+3)=\frac\partial{\partial x}(2y-2)=0.$$
That means there exists a potential function $\psi=\psi(x,y)$ such that

(1)
$$\frac{\partial\psi}{\partial x}=2x+3\\\frac{\partial\psi}{\partial y}=2y-2.$$
(2)

Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=x^2+3x+f(y)$$
Here $f$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=2y-2\quad\to\quad f(y)=y^2-2y.$$
As a result, a potential function is
$$\psi(x,y)=x^2+3x+y^2-2y.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.$$
(3)

Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}$$
$$\frac{d\psi}{dx}=0.$$
With it, equation (3) becomes

Integrate both sides with respect to $x.$
$$\psi(x,y)=C$$
Therefore,
$$x^2+3x+y^2-2y=C.$$

![](https://img.simpletex.net/pdf/BzBdZgZi/f1HoGYghbN1aaN3MnOpI9owH79bayPN52.png)


The general solution is a family of circles. This figure illustrates several of them. In red, orange, yellow, green, blue, and purple are $C=0,C=1,C=2,C=3,C=4$, and $C=5$, respectively.


--------------------------------------------------------------------------

### Q5

Multiply both sides by $bx+cy.$
$$(bx+cy)\frac{dy}{dx}=-(ax+by)$$
$$(ax+by)+(bx+cy)\frac{dy}{dx}=0$$
The ODE is exact because
$$\frac\partial{\partial y}(ax+by)=\frac\partial{\partial x}(bx+cy)=b.$$
That means there exists a potential function $\psi=\psi(x,y)$ such that
$$\frac{\partial\psi}{\partial x}=ax+by\\\frac{\partial\psi}{\partial y}=bx+cy.$$
Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=\frac{ax^2}2+bxy+f(y)$$
Here $f$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=bx+f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=cy\quad\to\quad f(y)=\frac{cy^2}{2}.$$
As a result, a potential function is
$$\psi(x,y)=\frac{ax^2}2+bxy+\frac{cy^2}2.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.$$
Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}$$
With it, equation (3) becomes
$$\frac{d\psi}{dx}=0.$$
Integrate both sides with respect to $x.$
$$\psi(x,y)=C$$
Therefore,
$$\frac{ax^2}2+bxy+\frac{cy^2}2=C.$$

--------------------------------------------------------------------------

### Q7

The ODE is exact because
$$\frac\partial{\partial y}\left(\frac yx+6x\right)=\frac\partial{\partial x}(\ln x-2)=\frac1x.$$
That means there exists a potential function $\psi=\psi(x,y)$ such that

(1)
$$\frac{\partial\psi}{\partial x}=\frac{y}{x}+6x\\\frac{\partial\psi}{\partial y}=\ln x-2.$$
(2)

Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=y\ln x+3x^2+f(y)$$
Here $f$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=\ln x+f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=-2\quad\to\quad f(y)=-2y.$$
As a result, a potential function is
$$\psi(x,y)=y\ln x+3x^2-2y.$$
Notice that by substituting equations (1) and (2), the ODE can be written as

(3)
$$\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.$$
Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}$$
$$\frac{d\psi}{dx}=0.$$
With it, equation (3) becomes

Integrate both sides with respect to $x.$
$$\psi(x,y)=C$$
Therefore,
$$y\ln x+3x^2-2y=C.$$


![](https://img.simpletex.net/pdf/BzBdZgAz/fMoTkMNHGuHivGeu513bGY6lalORTiacD.png)

This figure illustrates several solutions of the family. In red, orange, yellow, green, blue, and
${\mathrm{purple~are~}C=-10,C=-5,C=-1,C=1,C=5,\mathrm{~and~}C=10,\mathrm{~respectively}}$


--------------------------------------------------------------------------

### Q11

The ODE is exact only if
$$\frac\partial{\partial y}(xy^2+bx^2y)=2xy+bx^2=\frac\partial{\partial x}[(x+y)x^2]=3x^2+2xy,$$
that is, $b=3.$ That means there exists a potential function $\psi=\psi(x,y)$ such that

(1)
$$\frac{\partial\psi}{\partial x}=xy^2+3x^2y\\\frac{\partial\psi}{\partial y}=(x+y)x^2.$$
(2)

Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=\frac{x^2y^2}2+x^3y+f(y)$$
Here $f$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=x^2y+x^3+f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=0\quad\to\quad f(y)=0.$$
As a result, a potential function is
$$\psi(x,y)=\frac{x^2y^2}{2}+x^3y.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.$$
(3)

Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}$$
With it, equation (3) becomes
$$\frac{d\psi}{dx}=0.$$



Integrate both sides with respect to $x.$
$$\psi(x,y)=C$$
Therefore,
$$\frac{x^2y^2}2+x^3y=C.$$
![](https://img.simpletex.net/pdf/BzBdZgAz/fGPto3myThLU16Wt5Pg4fg4ut7pk7Yp4Z.png)


This figure illustrates several solutions of the family. In red, orange, yellow, green, blue, and
purple are $C=-10,C=-5,C=-1,C=1,C=5$, and $C=10$, respectively


### Q12

The ODE is exact only if
$$\frac{\partial}{\partial y}(ye^{2xy}+x)=e^{2xy}+2xye^{2xy}=\frac{\partial}{\partial x}(bxe^{2xy})=be^{2xy}+2bxye^{2xy},$$
that is, $b=1.$ That means there exists a potential function $\psi=\psi(x,y)$ such that

(1)
$$\begin{aligned}&\frac{\partial\psi}{\partial x}=ye^{2xy}+x\\&\frac{\partial\psi}{\partial y}=xe^{2xy}.\end{aligned}$$
(2)

Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=\frac{e^{2xy}}{2}+\frac{x^2}{2}+f(y)$$
Here $f$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=xe^{2xy}+f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=0\quad\to\quad f(y)=0.$$
As a result, a potential function is
$$\psi(x,y)=\frac{e^{2xy}}{2}+\frac{x^2}{2}.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.$$
(3)

Recall that the differential of $\psi(x,y)$ is defined as
$$\begin{aligned}d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.\end{aligned}$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\begin{aligned}\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}\end{aligned}$$
With it, equation (3) becomes
$$\frac{d\psi}{dx}=0.$$


Integrate both sides with respect to $x.$
$$\psi(x,y)=C$$
Therefore,
$$\frac{e^{2xy}}2+\frac{x^2}2=C.$$
![](https://img.simpletex.net/pdf/BzBdZgAz/f9To4YwN348IN4gQDy48HFYTAECl2GCFw.png)

This figure illustrates several solutions of the family. In red, orange, yellow, green, blue, and

purple are $C=1,C=5,C=10,C=15,C=20$, and $C=30$, respectively.


### Q18

The ODE is not exact at the moment because
$$\begin{aligned}\frac{\partial}{\partial y}(3x^2y+2xy+y^3)=3x^2+2x+3y^2\neq\frac{\partial}{\partial x}(x^2+y^2)=2x.\end{aligned}$$
To solve it, we seek an integrating factor $\mu=\mu(x,y)$ such that when both sides are multiplied by

it, the ODE becomes exact.
$$(3x^2y+2xy+y^3)\mu+(x^2+y^2)\mu y'=0$$
Since the ODE is exact now,
$$\frac\partial{\partial y}[(3x^2y+2xy+y^3)\mu]=\frac\partial{\partial x}[(x^2+y^2)\mu].$$
$$(3x^2+2x+3y^2)\mu+(3x^2y+2xy+y^3)\frac{\partial\mu}{\partial y}=2x\mu+(x^2+y^2)\frac{\partial\mu}{\partial x}$$
$$3(x^2+y^2)\mu+(3x^2y+2xy+y^3)\frac{\partial\mu}{\partial y}=(x^2+y^2)\frac{\partial\mu}{\partial x}$$
Assume that $\mu$ is only dependent on $x\colon\mu=\mu(x).$
$$3(x^2+y^2)\mu=(x^2+y^2)\frac{d\mu}{dx}$$
Solve for $\mu.$
$$\begin{aligned}\frac{d\mu}{dx}&=3\mu\\\frac{\frac{d\mu}{dx}}{\mu}&=3\\\frac{d}{dx}\ln\mu&=3\\\ln\mu&=3x\end{aligned}$$
$$\mu(x)=e^{3x}.$$
As a result, an integrating factor is

Multiply both sides of the original ODE by $e^3x.$
$$(3x^2e^{3x}y+2xe^{3x}y+e^{3x}y^3)+(x^2e^{3x}+e^{3x}y^2)y'=0$$

Because it's exact, there exists a potential function $\psi=\psi(x,y)$ that satisfies

(1)
$$\begin{aligned}&\frac{\partial\psi}{\partial x}=3x^2e^{3x}y+2xe^{3x}y+e^{3x}y^3\\&\frac{\partial\psi}{\partial y}=x^2e^{3x}+e^{3x}y^2.\end{aligned}$$
(2)

Integrate both sides of equation (2) partially with respect to $y$ to get $\psi.$
$$\psi(x,y)=x^2e^{3x}y+\frac{e^{3x}y^3}{3}+f(x)$$
Here $f(x)$ is an arbitrary function of $x.$ Differentiate both sides with respect to $x.$
$$\begin{aligned}\psi_x(x,y)=3x^2e^{3x}y+2xe^{3x}y+e^{3x}y^3+f'(x)\end{aligned}$$
Comparing this to equation (1),we see that
$$f'(x)=0\quad\to\quad f(x)=0.$$
As a result, a potential function is
$$\psi(x,y)=x^2e^{3x}y+\frac{e^{3x}y^3}{3}.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\begin{aligned}\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.\end{aligned}$$
(3)

Recall that the differential of $\psi(x,y)$ is defined as
$$\begin{aligned}d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.\end{aligned}$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\begin{aligned}\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}\end{aligned}$$
With it, equation (3) becomes
$$\frac{d\psi}{dx}=0.$$
$$\psi(x,y)=C$$
$$x^2e^{3x}y+\frac{e^{3x}y^3}{3}=C.$$


![](https://img.simpletex.net/pdf/BzBdZgAz/fhQevAMK5TE7V7nvkScufP24I0pDcucsd.png)


This figure illustrates several solutions of the family. In red, orange, yellow, green, blue, and

purple are $C=-30,C=-20,C=-10,C=10,C=20$, and $C=30$, respectively.
### Q21

This ODE is not exact at the moment because
$$\begin{aligned}\frac{\partial}{\partial y}(y)=1\neq\frac{\partial}{\partial x}(2xy-e^{-2y})=2y.\end{aligned}$$
To solve it, we seek an integrating factor $\mu=\mu(x,y)$ such that when both sides are multiplied by

it, the ODE becomes exact.
$$\mu y+\mu(2xy-e^{-2y})y'=0$$
Since the ODE is exact now,
$$\frac{\partial}{\partial y}(\mu y)=\frac{\partial}{\partial x}[\mu(2xy-e^{-2y})].$$
$$\dfrac{\partial\mu}{\partial y}y+\mu=\dfrac{\partial\mu}{\partial x}(2xy-e^{-2y})+\mu(2y)$$
Assume that $\mu$ is only dependent on $y\colon\mu=\mu(y).$
$$\dfrac{d\mu}{dy}y+\mu=\mu(2y)$$
$$\frac{d\mu}{dy}=\frac{2y-1}{y}\mu $$Hence, 
$$\dfrac{d\mu}{\mu}=\dfrac{2y-1}{y}\:dy$$
$$\begin{aligned}\ln\mu=2y-\ln y+C\end{aligned}$$
$$\mu=e^{2y}\left(\dfrac{1}{y}\right)e^C$$
Taking $e^C$ to be 1, an integrating factor is
$$\mu=\frac{e^{2y}}{y}.$$
Multiply both sides of the original ODE by $e^2y/y.$
$$e^{2y}+\left(2xe^{2y}-\dfrac{1}{y}\right)y'=0$$

Because it's exact, there exists a potential function $\psi=\psi(x,y)$ that satisfies

(1)
$$\begin{aligned}\frac{\partial\psi}{\partial x}&=e^{2y}\\\frac{\partial\psi}{\partial y}&=2xe^{2y}-\frac{1}{y}.\end{aligned}$$
(2)

Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$
$$\psi(x,y)=xe^{2y}+f(y)$$
Here $f(y)$ is an arbitrary function of $y.$ Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=2xe^{2y}+f'(y)$$
Comparing this to equation (2),we see that
$$f'(y)=-\dfrac{1}{y}\quad\to\quad f(y)=-\ln|y|.$$
As a result, a potential function is
$$\psi(x,y)=xe^{2y}-\ln|y|.$$
Notice that by substituting equations (1) and (2), the ODE can be written as
$$\begin{aligned}\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.\end{aligned}$$
(3)

Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}$$
With it, equation (3) becomes
$$\begin{aligned}\frac{d\psi}{dx}=0.\end{aligned}$$
Integrate both sides with respect to $x.$
$$\psi(x,y)=C_1$$
Therefore,
$$xe^{2y}-\ln|y|=C_1.$$


![](https://img.simpletex.net/pdf/BzBdZgAz/fgf1VSp1fNgSl2cRKhqDYlOZ13pAgs45L.png)


This figure illustrates several solutions of the family. In red, orange, yellow, green, blue, and
purple are $C_1=-10,C_1=-5,C_1=-1,C_1=1,C_1=5$, and $C_1=10$, respectively.
Notice also that $y=0$ is a solution.

### Q22


Multiply both sides of the ODE by $\mu(x,y).$
$$\left[\dfrac{3}{2x+y}+\dfrac{y}{x(2x+y)}\right]+\left[\dfrac{x}{y(2x+y)}+\dfrac{1}{2x+y}\right]y'=0$$
This ODE is exact because
$$\frac\partial{\partial y}\left[\frac3{2x+y}+\frac y{x(2x+y)}\right]=\frac\partial{\partial x}\left[\frac x{y(2x+y)}+\frac1{2x+y}\right]=-\frac1{(2x+y)^2}.$$
$$\frac{\partial\psi}{\partial x}=\frac{3}{2x+y}+\frac{y}{x(2x+y)}\\\frac{\partial\psi}{\partial y}=\frac{x}{y(2x+y)}+\frac{1}{2x+y}.$$
$$\int^x\left.\dfrac{\partial\psi}{\partial x}\right|_{x=s}ds=\int^x\dfrac{3}{2s+y}ds+\int^x\dfrac{y}{s(2s+y)}ds+f(y)$$
That means there exists a potential function $\psi=\psi(x,y)$ which satisfies Integrate both sides of equation (1) partially with respect to $x$ to get $\psi.$ Here $f(y)$ is an arbitrary function of $y.$
$$\begin{aligned}\psi(x,y)&=\int^x\frac3{2s+y}\:ds+\int^x\left(\frac1s+\frac{-2}{2s+y}\right)ds+f(y)\\&=\int^x\frac{ds}{2s+y}+\int^x\frac{ds}s+f(y)\end{aligned}$$
Use the substitution $u=2s+y$ and $du=2ds$ in the first integral.
$$\begin{aligned}\psi(x,y)&=\int^{2x+y}\frac{du/2}{u}+\int^{x}\frac{ds}{s}+f(y)\\&=\frac12\ln(2x+y)+\ln x+f(y)\end{aligned}$$
Differentiate both sides with respect to $y.$
$$\psi_y(x,y)=\frac{1}{2(2x+y)}+f'(y)$$
Comparing this to equation (2),we see that
$$\frac{1}{2(2x+y)}+f'(y)=\frac{x}{y(2x+y)}+\frac{1}{2x+y}\quad\to\quad f'(y)=\frac{x}{y(2x+y)}+\frac{1}{2(2x+y)}=\frac{2x+y}{2y(2x+y)}=\frac{1}{2y},$$


which means
$$f(y)=\frac{1}{2}\ln y.$$
As a result, a potential function is
$$\psi(x,y)=\frac{1}{2}\ln(2x+y)+\ln x+\frac{1}{2}\ln y.$$
Notice that by substituting equations (1) and (2), the ODE can be written as

(3)
$$\begin{aligned}\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}=0.\end{aligned}$$
Recall that the differential of $\psi(x,y)$ is defined as
$$d\psi=\frac{\partial\psi}{\partial x}\:dx+\frac{\partial\psi}{\partial y}\:dy.$$
Dividing both sides by $dx$, we obtain the fundamental relationship between the total derivative of

$\psi$ and its partial derivatives.
$$\begin{aligned}\frac{d\psi}{dx}=\frac{\partial\psi}{\partial x}+\frac{\partial\psi}{\partial y}\frac{dy}{dx}\end{aligned}$$
With it, equation (3) becomes
$$\frac{d\psi}{dx}=0.$$
Integrate both sides with respect to $x.$
$$\psi(x,y)=C_1$$
$$\dfrac{1}{2}\ln(2x+y)+\ln x+\dfrac{1}{2}\ln y=C_1$$
$$\begin{aligned}\ln(2x+y)+2\ln x+\ln y=2C_1\end{aligned}$$
$$\begin{aligned}\ln(2x+y)+\ln x^2+\ln y=2C_1\end{aligned}$$
$$\ln[(2x+y)(x^2)(y)]=2C_1$$
$$x^2y(2x+y)=e^{2C_1}$$
$$2x^3y+x^2y^2=e^{2C_1}$$
$$x^3y+\frac{1}{2}x^2y^2=\frac{1}{2}e^{2C_1}$$
Therefore, using a new constant $c$ for the right side,
$$x^3y+\dfrac{1}{2}x^2y^2=c,$$
which is the same answer obtained in Example 4 of the textbook.
## 2.7

### Q1


Attached

### Q7

![](https://img.simpletex.net/pdf/BzBdZgAz/fCwly1Ap20DSIMMI2gLrPKTw32UTtp7v6.png)

Solutions with initial conditions to the 'left' of the curve $t=0.1y^2$ seem to diverge. On the other hand, solutions to the 'right' of the curve seem to converge to zero. Also, $\phi(t)$ is an equilibrium solution.

### Q12


Attached 


##  3.1
### Q6


Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y^{\prime}=re^{rt}\quad\to\quad y^{\prime\prime}=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2e^{rt}-2(re^{rt})-2(e^{rt})=0$$
Divide both sides by $e^rt.$
$$r^2-2r-2=0$$
$$r=\frac{2\pm\sqrt{4+4(2)(1)}}2=\frac{2\pm\sqrt{12}}2=\frac{2\pm2\sqrt3}2=1\pm\sqrt3$$
$$r=\left\{1-\sqrt{3},1+\sqrt{3}\right\}$$
Two solutions to the ODE are $y=e^(1-\sqrt{3})t$ and $y=e^(1+\sqrt{3})t.$ Therefore, the general solution is
$$y(t)=C_1e^{(1-\sqrt{3})t}+C_2e^{(1+\sqrt{3})t},$$
a linear combination of the two.

### Q7

$$r^2e^{rt}+re^{rt}-2(e^{rt})=0$$
Divide both sides by $e^rt.$

Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y'=re^{rt}\quad\to\quad y''=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2+r-2=0$$
$$(r+2)(r-1)=0$$
$$r=\{-2,1\}$$
Two solutions to the ODE are $y=e^-2t$ and $y=e^t$, so the general solution is
$$y(t)=C_1e^{-2t}+C_2e^t,$$
a linear combination of the two. Differentiate it once with respect to $t.$
$$y'(t)=-2C_1e^{-2t}+C_2e^t$$
Apply the two initial conditions now to determine $C_1$ and $C_2.$
$$\begin{aligned}y(0)&=C_1+C_2=1\\y'(0)&=-2C_1+C_2=1\end{aligned}$$
Solving the system of equations yields $C_1=0$ and $C_2=1.$ Therefore,
$$y(t)=e^t.$$
This solution diverges to $\infty$ as $t\to\infty.$

### Q11

Divide both sides by $e^rt.$

Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y'=re^{rt}\quad\to\quad y''=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2e^{rt}+8(re^{rt})-9(e^{rt})=0$$
$$r^2+8r-9=0$$
$$(r+9)(r-1)=0$$
$$r=\{-9,1\}$$
Two solutions to the ODE are $y=e^-9t$ and $y=e^t$, so the general solution is
$$y(t)=C_1e^{-9t}+C_2e^t,$$
a linear combination of the two. Differentiate it once with respect to $t.$
$$y'(t)=-9C_1e^{-9t}+C_2e^t,$$
Apply the two initial conditions now to determine $C_1$ and $C_2.$
$$\begin{aligned}&y(1)=C_1e^{-9}+C_2e^1=1\\&y^{\prime}(1)=-9C_1e^{-9}+C_2e^1=0\end{aligned}$$
Solving the system of equations yields $C_1=e^9/10$ and $C_2=9/(10e).$ Therefore,
$$y(t)=\frac{e^9}{10}e^{-9t}+\frac{9}{10e}e^t.$$
Because the coefficient of $t$ in the second exponential function is positive, this solution diverges to
$\infty$ as $t\to\infty.$

### Q16


$$r^2e^{rt}-re^{rt}-2(e^{rt})=0$$
Divide both sides by $e^rt.$

Since this is a linear homogeneous constant-coefficient ODE, the solution is of the form $y=e^rt.$
$$y=e^{rt}\quad\to\quad y^{\prime}=re^{rt}\quad\to\quad y^{\prime\prime}=r^2e^{rt}$$
Substitute these expressions into the ODE.
$$r^2-r-2=0$$
$$(r-2)(r+1)=0$$
$$r=\{-1,2\}$$
Two solutions to the ODE are $y=e^-t$ and $y=e^2t$, so the general solution is
$$y(t)=C_1e^{-t}+C_2e^{2t},$$
a linear combination of the two. Differentiate it once with respect to $t.$
$$y'(t)=-C_1e^{-t}+2C_2e^{2t}$$
Apply the two initial conditions now to determine $C_1$ and $C_2.$
$$\begin{aligned}y(0)&=C_1+C_2=\alpha\\y'(0)&=-C_1+2C_2=2\end{aligned}$$
Solving the system of equations yields
$$C_{1}=\frac23(\alpha-1)\\C_{2}=\frac13(\alpha+2).$$
Therefore,
$$y(t)=\frac23(\alpha-1)e^{-t}+\frac13(\alpha+2)e^{2t}.$$
To prevent the solution from blowing up as $t\to\infty$, set $\alpha=-2.$