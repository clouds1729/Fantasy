  
### 10.5
#### 3

$u_{xx} + u_x + u_t = 0$ 

Assume $u(x,t) = X(x)T(t)$ 

$$ X''(x)T(t) + X'(x)T(t) + X(x)T'(t) = 0 $$ 

Divide by $X(x)T(t)$:

$$ \frac{X''(x)}{X(x)} + \frac{X'(x)}{X(x)} + \frac{T'(t)}{T(t)} = 0 $$ 

Set each side equal to $-\lambda$:

$$ X'' + X' + \lambda X = 0, \quad T' + \lambda T = 0 $$  


#### 4

$(p(x)u_x)_x - r(x)u_{tt} = 0$ 

Assume $u(x,t) = X(x)T(t)$ 

$$ (p(x)X'(x))'T(t) - r(x)X(x)T''(t) = 0 $$ 

Divide by $X(x)T(t)$:

$$ \frac{(p(x)X'(x))'}{X(x)} - \frac{r(x)T''(t)}{T(t)} = 0 $$ 

Set each side equal to $-\lambda$:

$$ (p(x)X')' + \lambda r(x) X = 0, \quad T'' + \lambda T = 0 $$


#### 7

 $100u_{xx} = u_t, \; u(0,t) = 0, \; u(1,t) = 0, \; u(x,0) = \sin(2\pi x) - \sin(5\pi x)$ 
 
 Assume $u(x,t) = X(x)T(t)$ 
 
 $$ 100X''(x)T(t) = X(x)T'(t) $$ 
 
 Divide by $X(x)T(t)$:

 $$ 100\frac{X''(x)}{X(x)} = \frac{T'(t)}{T(t)} $$ 

Set each side equal to $-\lambda$:

$$ 100X'' + \lambda X = 0, \quad T' + \lambda T = 0 $$ 

Solution:

$$ u(x,t) = e^{-400\pi^2 t} \sin(2\pi x) - e^{-2500\pi^2 t} \sin(5\pi x) $$


#### 11


 $u(x,0) = \left\{ \begin{array}{ll} 50, & 10 \leq x \leq 30 \\ 0, & \text{otherwise} \end{array} \right.$ 
 
 Assume $u(x,t) = \sum_{n=1}^{\infty} a_n e^{-n^2\pi^2 t/1600} \sin\left(\frac{n\pi x}{40}\right)$ 

Fourier coefficients:

$$ a_n = \frac{100}{\pi} \int_{10}^{30} 50 \sin\left(\frac{n\pi x}{40}\right) \, dx $$ 

Solve the integral and sum:

$$ u(x,t) = \frac{100}{\pi} \sum_{n=1}^{\infty} \left( \cos\left(\frac{n\pi}{4}\right) - \cos\left(\frac{3n\pi}{4}\right) \right) \frac{e^{-n^2\pi^2 t/1600}}{n} \sin\left(\frac{n\pi x}{40}\right) $$


#### 12

 $u(x,0) = x, \; 0 \leq x < 40$ 
 
 Assume $u(x,t) = \sum_{n=1}^{\infty} a_n e^{-n^2\pi^2 t/1600} \sin\left(\frac{n\pi x}{40}\right)$ 

Fourier coefficients:

$$ a_n = \frac{2}{40} \int_{0}^{40} x \sin\left(\frac{n\pi x}{40}\right) \, dx $$ 

$$ a_n = \frac{2}{40} \left[ \frac{-40^2}{n^2\pi^2} \left(\sin\left(\frac{n\pi x}{40}\right)\right) \right]_0^{40} + \frac{2}{40} \left[ \frac{40}{n\pi} \left(\cos\left(\frac{n\pi x}{40}\right)\right) \right]_0^{40} $$ 

$$ a_n = \frac{80}{n^2\pi^2} \left[(-1)^n - 1 \right] $$

Thus,

$$ u(x,t) = \frac{80}{\pi} \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n} e^{-n^2\pi^2 t/1600} \sin\left(\frac{n\pi x}{40}\right) $$



#### 21


$$ u(x,t) = \frac{200}{\pi} \sum_{n=1}^{\infty} \frac{1 - \cos(n\pi)}{n} e^{-n^2 \pi^2 \alpha^2 t / 400} \sin \left( \frac{n \pi x}{20} \right) $$

a. $\alpha^2_{\text{silver}} = 1.71 \times 10^{-2}$

$$ u(10,30) = 35.91^\circ C $$

b. $\alpha^2_{\text{aluminum}} = 8.418 \times 10^{-2}$

$$ u(10,30) = 67.23^\circ C $$

c. $\alpha^2_{\text{cast iron}} = 3.22 \times 10^{-3}$

$$ u(10,30) = 99.96^\circ C $$


#### 22


a. Using two terms:

$$ u(x,t) = \frac{200}{\pi} \left( \frac{1 - \cos(\pi)}{1} e^{-\pi^2 \alpha^2 t / 400} \sin \left( \frac{\pi x}{20} \right) + \frac{1 - \cos(3\pi)}{3} e^{-9 \pi^2 \alpha^2 t / 400} \sin \left( \frac{3 \pi x}{20} \right) \right) $$

Solve $u(10, \tau) = 1^\circ C$ for $\tau$:

$$ \tau_2 \approx 820 \text{ s} $$

b. Using three terms:

$$ u(x,t) = \frac{200}{\pi} \sum_{n=1,3,5}^{\infty} \frac{1 - \cos(n\pi)}{n} e^{-n^2 \pi^2 \alpha^2 t / 400} \sin \left( \frac{n \pi x}{20} \right) $$

Solve $u(10, \tau) = 1^\circ C$ for $\tau$:

$$ \tau_3 \approx 690 \text{ s} $$

c. Compare the times found in a and b with the time found using one term in Example 1:

One term in Example 1:

$$ \tau_1 = \frac{2500}{\pi^2} \ln \left( \frac{80}{\pi} \right) \approx 820 \text{ s} $$

Comparing $\tau_2$ and $\tau_3$ with $\tau_1$:

$$ \tau_2 \approx \tau_1 $$
$$ \tau_3 < \tau_1 $$


### 10.6:  
#### 1

$u(0,t) = 10, \; u(50,t) = 40$

Assume $u(x,t) = X(x)$

Boundary conditions:

$$ X(0) = 10, \quad X(50) = 40 $$

Linear interpolation:

$$ u(x,t) = 10 + \frac{3}{5} x $$


#### 2

$u(0,t) = 30, \; u(40,t) = -20$

Assume $u(x,t) = X(x)$

Boundary conditions:

$$ X(0) = 30, \quad X(40) = -20 $$

Linear interpolation:

$$ u(x,t) = 30 - \frac{5}{4} x $$


#### 8

$u(0,t) = T, \; u_x(L,t) = 0$

Assume $u(x,t) = X(x)$

Boundary conditions:

$$ X(0) = T, \quad X'(L) = 0 $$

Solution:

$$ u(x,t) = T(1 + x)/(1 + L) $$


#### 11

a. 
Assume $u(x,t) = X(x)T(t)$

Initial condition:

$$ u(x,0) = x(60 - x)/30 $$

Fourier series solution:

$$ u(x,t) = 30 - x + \sum_{n=1}^{\infty} c_n e^{-n^2 t/900} \sin\left(\frac{n \pi x}{30}\right) $$

Fourier coefficients:

$$ c_n = \frac{60}{n^3 \pi^3} \left( 2(1 - \cos(n\pi)) - n^2 \pi^2 (1 + \cos(n\pi)) \right) $$

b.

![[Pasted image 20240730215303.png]]


c. 

![[Pasted image 20240730215441.png]]

Initially, $u$ decreases due to the heat flow towards the colder end ($x=30$). As the rod approaches thermal equilibrium, the heat flow reduces, and the temperature increases before finally stabilizing.
#### 12

Consider a uniform rod of length $L$ with an initial temperature given by $u(x,0) = \sin(\pi x / L), \; 0 \le x \le L$. Assume that both ends of the bar are insulated.

a. Find $u(x,t)$

Assume $u(x,t) = X(x)T(t)$

Initial condition:

$$ u(x,0) = \sin(\pi x / L) $$

Fourier series solution:

$$ u(x,t) = \frac{2}{\pi} + \sum_{n=1}^{\infty} c_n e^{-n^2 \pi^2 \alpha^2 t / L^2} \cos\left(\frac{n \pi x}{L}\right) $$

Fourier coefficients:

$$ c_n = \begin{cases} 
0, & n \text{ odd} \\
-\frac{4}{(n^2 - 1) \pi}, & n \text{ even}
\end{cases} $$

b. Find the steady-state temperature as $t \to \infty$

$$ \lim_{t \to \infty} u(x,t) = \frac{2}{\pi} $$

c. 

![[Pasted image 20240730230141.png]]


d. 
Initially, the temperature distribution follows the sine function. Over time, the higher-order terms decay faster due to the exponential factor, leaving the lower-order terms to dominate, resulting in a smoother temperature profile until it reaches steady-state.

 
### 10.7:  
#### 4

$$ u(x,0) = T, \; u_x(0,t) = 0, \; u_x(L,t) = 0 $$

Assume $u(x,t) = X(x)T(t)$

Boundary conditions:

$$ X'(0) = 0, \quad X'(L) = 0 $$

Solution:

$$ u(x,t) = \frac{4}{\pi} \sum_{n=1}^{\infty} \frac{\sin\left(\frac{n\pi}{2}\right) \sin\left(\frac{n\pi x}{L}\right)}{n} \cos\left(\frac{n\pi at}{L}\right) $$


#### 8

$$ u(0,t) = T, \; u(L,t) = 0, \; u_x(0,t) = 0 $$

Assume $u(x,t) = X(x)T(t)$

Boundary conditions:

$$ X(0) = T, \quad X(L) = 0 $$

Solution:

$$ u(x,t) = \frac{4L}{a\pi^2} \sum_{n=1}^{\infty} \frac{\sin\left(\frac{n\pi}{2}\right) \sin\left(\frac{n\pi x}{L}\right)}{n^2} \sin\left(\frac{n\pi at}{L}\right) $$


#### 9

$$ 
u(x,0) = f(x) 
$$

Assume 
$$ 
u(x,t) = \sum_{n=1}^{\infty} C_n \sin\left(\frac{(2n-1)\pi x}{2L}\right) \cos\left(\frac{(2n-1)\pi at}{2L}\right) 
$$

Fourier coefficients:

$$ 
C_n = \frac{2}{L} \int_0^L f(x) \sin\left(\frac{(2n-1)\pi x}{2L}\right) dx 
$$

Solution:

$$ 
u(x,t) = \sum_{n=1}^{\infty} C_n \sin\left(\frac{(2n-1)\pi x}{2L}\right) \cos\left(\frac{(2n-1)\pi at}{2L}\right) 
$$


#### 10

$$
u(x,0) = f(x), \; f(x) = \begin{cases} 
0, & 0 \leq x \leq L/2 - 1 \\ 
1, & L/2 - 1 < x \leq L/2 + 1 \\ 
0, & L/2 + 1 < x \leq L 
\end{cases} 
$$

Assume 
$$ 
u(x,t) = \sum_{n=1}^{\infty} C_n \sin\left(\frac{(2n-1)\pi x}{2L}\right) \cos\left(\frac{(2n-1)\pi at}{2L}\right) 
$$

Fourier coefficients:

$$ 
C_n = \frac{8}{\pi} \sum_{n=1}^{\infty} \frac{1}{2n-1} \sin\left(\frac{(2n-1)\pi}{4}\right) \sin\left(\frac{(2n-1)\pi x}{2L}\right) 
$$

Solution:

$$ 
u(x,t) = \frac{8}{\pi} \sum_{n=1}^{\infty} \frac{1}{2n-1} \sin\left(\frac{(2n-1)\pi}{4}\right) \sin\left(\frac{(2n-1)\pi x}{2L}\right) \cos\left(\frac{(2n-1)\pi at}{2L}\right) 
$$

   
### 10.8:  
#### 2

Assume $u(x,y) = X(x)Y(y)$.

Boundary conditions:
$$
X(0) = 0, \quad X(a) = 0, \quad Y(0) = h(x), \quad Y(b) = 0
$$

Separation of variables:
$$
\frac{X''(x)}{X(x)} = -\frac{Y''(y)}{Y(y)} = \lambda
$$

Solve $X(x)$ and $Y(y)$:
$$
X'' + \lambda X = 0 \quad \Rightarrow \quad X(x) = \sin\left(\frac{n\pi x}{a}\right)
$$
$$
Y'' - \lambda Y = 0 \quad \Rightarrow \quad Y(y) = \sinh\left(\frac{n\pi y}{a}\right)
$$

General solution:
$$
u(x,y) = \sum_{n=1}^{\infty} c_n \sin\left(\frac{n\pi x}{a}\right) \sinh\left(\frac{n\pi (b-y)}{a}\right)
$$

Fourier coefficients:
$$
c_n = \frac{2}{a\sinh(n\pi b/a)} \int_0^a h(x) \sin\left(\frac{n\pi x}{a}\right) dx
$$


#### 8

Assume $u(x,y) = X(x)Y(y)$.

Boundary conditions:
$$
X(0) = 0, \quad X(a) = 0, \quad Y(0) = f(x)
$$

Separation of variables:
$$
\frac{X''(x)}{X(x)} = -\frac{Y''(y)}{Y(y)} = \lambda
$$

Solve $X(x)$ and $Y(y)$:
$$
X'' + \lambda X = 0 \quad \Rightarrow \quad X(x) = \sin\left(\frac{n\pi x}{a}\right)
$$
$$
Y'' - \lambda Y = 0 \quad \Rightarrow \quad Y(y) = e^{-n\pi y/a}
$$

General solution:
$$
u(x,y) = \sum_{n=1}^{\infty} c_n e^{-n\pi y/a} \sin\left(\frac{n\pi x}{a}\right)
$$

Fourier coefficients:
$$
c_n = \frac{2}{a} \int_0^a f(x) \sin\left(\frac{n\pi x}{a}\right) dx
$$

The smallest $y_0$ for which $u(x, y_0) = \frac{1}{2} f(x)$:
$$
y_0 = \frac{a}{\pi} \ln 2 \approx 6.6315
$$


#### 10

**a.** 

Solve Laplace's equation:
$$
\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0
$$

Assume $u(x,y) = X(x)Y(y)$.

Separation of variables:
$$
\frac{X''(x)}{X(x)} = -\frac{Y''(y)}{Y(y)} = \lambda = \left(\frac{n\pi}{b}\right)^2
$$

Solve $X(x)$ and $Y(y)$:
$$
X(x) = \cosh\left(\frac{n\pi x}{b}\right), \quad Y(y) = \cos\left(\frac{n\pi y}{b}\right)
$$

General solution:
$$
u_n(x,y) = c_n \cosh\left(\frac{n\pi x}{b}\right) \cos\left(\frac{n\pi y}{b}\right), \quad n = 1, 2, 3, \ldots
$$

**b. **

General solution:
$$
u(x,y) = c_0 + \sum_{n=1}^{\infty} c_n \cosh\left(\frac{n\pi x}{b}\right) \cos\left(\frac{n\pi y}{b}\right)
$$

Boundary condition:
$$
u_x(a,y) = \sum_{n=1}^{\infty} c_n \frac{n\pi}{b} \sinh\left(\frac{n\pi a}{b}\right) \cos\left(\frac{n\pi y}{b}\right) = f(y)
$$

Fourier coefficients:
$$
c_n = \frac{2}{n\pi \sinh(n\pi a/b)} \int_0^b f(y) \cos\left(\frac{n\pi y}{b}\right) dy
$$

Condition for solvability:
$$
\int_0^b f(y) dy = 0
$$

**c.**

Since $c_0$ remains arbitrary, the solution is determined up to this additive constant. This is a property of all Neumann problems. The final solution is:
$$
u(x,y) = c_0 + \sum_{n=1}^{\infty} c_n \cosh\left(\frac{n\pi x}{b}\right) \cos\left(\frac{n\pi y}{b}\right)
$$
