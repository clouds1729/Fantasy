## Section 10.1

### 2

$$
\begin{align*}
\text{Given:} & \quad y'' + 2y = 0 \\
\text{Characteristic equation:} & \quad r^2 + 2 = 0 \implies r = \pm i\sqrt{2} \\
\text{General solution:} & \quad y(x) = c_1 \cos(\sqrt{2} x) + c_2 \sin(\sqrt{2} x) \\
\text{Using initial conditions:} & \quad y'(0) = 1 \text{ and } y'(\pi) = 0 \\
y(x) & = c_1 \cos(\sqrt{2} x) + c_2 \sin(\sqrt{2} x) \\
y'(x) & = -c_1 \sqrt{2} \sin(\sqrt{2} x) + c_2 \sqrt{2} \cos(\sqrt{2} x) \\
y'(0) & = c_2 \sqrt{2} = 1 \implies c_2 = \frac{1}{\sqrt{2}} \\
y'(\pi) & = -c_1 \sqrt{2} \sin(\sqrt{2} \pi) + c_2 \sqrt{2} \cos(\sqrt{2} \pi) \\
0 & = -c_1 \sqrt{2} \sin(\sqrt{2} \pi) + \frac{\sqrt{2}}{\sqrt{2}} \cos(\sqrt{2} \pi) \\
0 & = -c_1 \sin(\sqrt{2} \pi) + \cos(\sqrt{2} \pi) \\
c_1 \sin(\sqrt{2} \pi) & = \cos(\sqrt{2} \pi) \\
c_1 & = \cot(\sqrt{2} \pi) \\
\text{Solution:} & \quad y(x) = \cot(\sqrt{2} \pi) \cos(\sqrt{2} x) + \frac{1}{\sqrt{2}} \sin(\sqrt{2} x)
\end{align*}
$$


### 3


$$
\begin{align*}
\text{Given:} & \quad y'' + y = 0 \\
\text{Characteristic equation:} & \quad r^2 + 1 = 0 \implies r = \pm i \\
\text{General solution:} & \quad y(x) = c_1 \cos(x) + c_2 \sin(x) \\
\text{Using initial conditions:} & \quad y(0) = 0 \text{ and } y(L) = 0 \\
y(0) & = c_1 \cos(0) + c_2 \sin(0) = c_1 = 0 \implies y(x) = c_2 \sin(x) \\
y(L) & = c_2 \sin(L) = 0 \\
\text{For non-trivial solution:} & \quad \sin(L) = 0 \implies L = n\pi, \, n \in \mathbb{Z} \\
\text{Solution:} & \quad y(x) = c_2 \sin(x) \quad \text{if} \quad \sin(L) = 0 \\
\text{Trivial solution:} & \quad y(x) = 0 \quad \text{for all} \quad L
\end{align*}
$$


### 7

$$
\begin{align*}
\text{Given:} & \quad y'' + 4y = \cos(x), \quad y(0) = 0, \quad y(\pi) = 0 \\
\text{Complementary solution:} & \quad y_c(x) = c_1 \cos(2x) + c_2 \sin(2x) \\
\text{Particular solution:} & \quad y_p(x) = A \cos(x) \\
\text{Substitute } y_p \text{ into the differential equation:} & \\
y_p'' + 4y_p & = -A \cos(x) + 4A \cos(x) = 3A \cos(x) \\
& = \cos(x) \implies 3A = 1 \implies A = \frac{1}{3} \\
\text{General solution:} & \quad y(x) = y_c(x) + y_p(x) = c_1 \cos(2x) + c_2 \sin(2x) + \frac{1}{3} \cos(x) \\
\text{Applying boundary conditions:} & \\
y(0) = 0 & \implies c_1 + \frac{1}{3} = 0 \implies c_1 = -\frac{1}{3} \\
y(\pi) = 0 & \implies -\frac{1}{3} \cos(2\pi) + c_2 \sin(2\pi) + \frac{1}{3} \cos(\pi) \\
& = -\frac{1}{3} \cdot 1 + 0 + \frac{1}{3} \cdot (-1) = -\frac{1}{3} - \frac{1}{3} \neq 0 \\
\text{This yields a contradiction,} & \quad \text{hence there is no solution.}
\end{align*}
$$


### 14


$$
\begin{align*}
\text{Given:} & \quad y'' + \lambda y = 0, \quad y(0) = 0, \quad y'(\pi) = 0 \\
\text{Characteristic equation:} & \quad r^2 + \lambda = 0 \implies r = \pm i\sqrt{\lambda} \\
\text{General solution:} & \quad y(x) = c_1 \cos(\sqrt{\lambda} x) + c_2 \sin(\sqrt{\lambda} x) \\
\text{Applying boundary condition } y(0) = 0: & \quad y(0) = c_1 = 0 \implies y(x) = c_2 \sin(\sqrt{\lambda} x) \\
\text{Applying boundary condition } y'(\pi) = 0: & \\
y'(x) & = c_2 \sqrt{\lambda} \cos(\sqrt{\lambda} x) \\
y'(\pi) = 0 & \implies c_2 \sqrt{\lambda} \cos(\sqrt{\lambda} \pi) = 0 \\
\text{For non-trivial solution:} & \quad \cos(\sqrt{\lambda} \pi) = 0 \implies \sqrt{\lambda} \pi = \left(n - \frac{1}{2}\right) \pi \implies \sqrt{\lambda} = \frac{2n - 1}{2} \\
\text{Eigenvalues:} & \quad \lambda_n = \left(\frac{2n - 1}{2}\right)^2 \\
\text{Eigenfunctions:} & \quad y_n(x) = \sin\left(\frac{2n - 1}{2} x\right), \quad n = 1, 2, 3, \ldots
\end{align*}
$$

### 17

$$
\begin{align*}
\text{Given:} & \quad y'' + \lambda y = 0, \quad y'(0) = 0, \quad y(L) = 0 \\
\text{Characteristic equation:} & \quad r^2 + \lambda = 0 \implies r = \pm i\sqrt{\lambda} \\
\text{General solution:} & \quad y(x) = c_1 \cos(\sqrt{\lambda} x) + c_2 \sin(\sqrt{\lambda} x) \\
\text{Applying boundary condition } y'(0) = 0: & \quad y'(x) = -c_1 \sqrt{\lambda} \sin(\sqrt{\lambda} x) + c_2 \sqrt{\lambda} \cos(\sqrt{\lambda} x) \\
& \quad y'(0) = c_2 \sqrt{\lambda} = 0 \implies c_2 = 0 \\
\text{Therefore:} & \quad y(x) = c_1 \cos(\sqrt{\lambda} x) \\
\text{Applying boundary condition } y(L) = 0: & \quad y(L) = c_1 \cos(\sqrt{\lambda} L) = 0 \\
\text{For non-trivial solution:} & \quad \cos(\sqrt{\lambda} L) = 0 \implies \sqrt{\lambda} L = \left(n - \frac{1}{2}\right) \pi \implies \sqrt{\lambda} = \frac{(2n-1) \pi}{2L} \\
\text{Eigenvalues:} & \quad \lambda_n = \left(\frac{(2n-1) \pi}{2L}\right)^2 \\
\text{Eigenfunctions:} & \quad y_n(x) = \cos\left(\frac{(2n-1) \pi x}{2L}\right), \quad n = 1, 2, 3, \ldots
\end{align*}
$$

### 20

$$
\begin{align*}
\text{Given:} & \quad x^2 y'' - x y' + \lambda y = 0, \quad y(1) = 0, \quad y(L) = 0, \quad L > 1 \\
\text{Substitute } y(x) = x^r: & \quad x^2 (r(r-1)x^{r-2}) - x (r x^{r-1}) + \lambda x^r = 0 \\
& \quad r(r-1) - r + \lambda = 0 \implies r^2 - 2r + \lambda = 0 \\
\text{Roots:} & \quad r = 1 \pm \sqrt{1-\lambda} \\
\text{General solution:} & \quad y(x) = c_1 x^{1+\sqrt{1-\lambda}} + c_2 x^{1-\sqrt{1-\lambda}} \\
\text{Boundary condition } y(1) = 0: & \quad c_1 (1^{1+\sqrt{1-\lambda}}) + c_2 (1^{1-\sqrt{1-\lambda}}) = 0 \implies c_1 + c_2 = 0 \implies c_2 = -c_1 \\
\text{Simplified solution:} & \quad y(x) = c_1 (x^{1+\sqrt{1-\lambda}} - x^{1-\sqrt{1-\lambda}}) \\
\text{Boundary condition } y(L) = 0: & \quad c_1 (L^{1+\sqrt{1-\lambda}} - L^{1-\sqrt{1-\lambda}}) = 0 \\
\text{Non-trivial solution:} & \quad L^{1+\sqrt{1-\lambda}} = L^{1-\sqrt{1-\lambda}} \\
& \quad L^{2\sqrt{1-\lambda}} = 1 \implies 2\sqrt{1-\lambda} \ln L = n \pi \implies \sqrt{1-\lambda} = \frac{n \pi}{2 \ln L} \\
& \quad 1 - \lambda = \left(\frac{n \pi}{2 \ln L}\right)^2 \implies \lambda_n = 1 + \left(\frac{n \pi}{\ln L}\right)^2 \\
\text{Eigenfunctions:} & \quad y_n(x) = x \sin\left(\frac{n \pi \ln x}{\ln L}\right), \quad n = 1, 2, 3, \ldots
\end{align*}
$$


## Section 10.2

### 4
$$
\begin{align*} \text{Given:} & \quad f(x) = \sin\left( \frac{\pi x}{L} \right) \\ \text{To determine if } f(x) \text{ is periodic:} & \\ \text{A function } f(x) \text{ is periodic if } & \quad f(x + T) = f(x) \text{ for some } T > 0 \\ f(x + 2L) & = \sin\left( \frac{\pi (x + 2L)}{L} \right) \\ & = \sin\left( \frac{\pi x}{L} + 2\pi \right) \\ & = \sin\left( \frac{\pi x}{L} \right) \quad (\text{since } \sin(\theta + 2\pi) = \sin(\theta)) \\ \text{Therefore, } f(x) & \text{ is periodic with period } T = 2L. \end{align*}
$$

### 6


$$
\begin{align*}
\text{Given:} & \quad f(x) = x^2 \\
\text{To determine if } f(x) \text{ is periodic:} & \\
\text{A function } f(x) \text{ is periodic if } & \quad f(x + T) = f(x) \text{ for some } T > 0 \\
f(x + T) & = (x + T)^2 = x^2 + 2Tx + T^2 \\
f(x + T) & \neq f(x) \text{ unless } 2Tx + T^2 = 0 \text{ for all } x \\
\text{This condition is not possible,} & \quad \text{hence } f(x) \text{ is not periodic.}
\end{align*}
$$


### 8

$$
\begin{align*}
\text{Given:} & \quad f(x) = 
\begin{cases} 
(-1)^n, & 2n - 1 \leq x < 2n \\
1, & 2n \leq x < 2n + 1 
\end{cases}, \quad n = 0, \pm1, \pm2, \ldots \\
\text{To determine if } f(x) \text{ is periodic:} & \\
\text{We need to check if } f(x + T) = f(x) & \text{ for some period } T > 0 \\
\text{Let } T = 4: & \\
f(x + 4) & = 
\begin{cases} 
(-1)^n, & 2n - 1 \leq (x + 4) < 2n \\
1, & 2n \leq (x + 4) < 2n + 1 
\end{cases} \\
& = 
\begin{cases} 
(-1)^{n+2}, & 2(n+2) - 1 \leq x < 2(n+2) \\
1, & 2(n+2) \leq x < 2(n+2) + 1 
\end{cases} \\
& = 
\begin{cases} 
(-1)^n, & 2n - 1 \leq x < 2n \\
1, & 2n \leq x < 2n + 1 
\end{cases} \\
\text{Therefore, } f(x) & \text{ is periodic with period } T = 4.
\end{align*}
$$


### 9

$$
\begin{align*}
\text{Given:} & \quad f(x) = -x \text{ for } -L < x < L \\
\text{Given periodicity:} & \quad f(x + 2L) = f(x) \\
\text{To find } f(x) \text{ in the interval } L < x < 2L: & \\
\text{Since } f(x + 2L) = f(x), & \text{ consider } x \in L < x < 2L \\
f(x) = f(x - 2L) & \text{ in } -L < (x - 2L) < L \\
f(x) & = -(x - 2L) = 2L - x \text{ for } L < x < 2L \\
\text{To find } f(x) \text{ in the interval } -3L < x < -2L: & \\
\text{Since } f(x + 2L) = f(x), & \text{ consider } x \in -3L < x < -2L \\
f(x) = f(x + 2L) & \text{ in } -L < (x + 2L) < L \\
f(x) & = -(x + 2L) = -2L - x \text{ for } -3L < x < -2L \\
\text{Thus, the formulas are:} & \\
f(x) & = 2L - x \text{ in the interval } L < x < 2L \\
f(x) & = -2L - x \text{ in the interval } -3L < x < -2L
\end{align*}
$$


### 16

$$
\begin{align*} \text{Given:} & \quad f(x) = \begin{cases} x + 1, & -1 \leq x < 0 \\ 1 - x, & 0 \leq x < 1 \end{cases} \\ \text{Period:} & \quad T = 2 \\ \text{Fourier series:} & \\ a_0 & = \frac{1}{2} \int_{-1}^{1} f(x) \, dx = \frac{1}{2} \left( \int_{-1}^{0} (x + 1) \, dx + \int_{0}^{1} (1 - x) \, dx \right) = \frac{1}{2} \\ a_n & = 0 \quad (\text{since } f(x) \text{ is an odd function}) \\ b_n & = \frac{2}{2} \int_{-1}^{1} f(x) \sin(n \pi x) \, dx = 2 \int_{-1}^{0} (x + 1) \sin(n \pi x) \, dx + 2 \int_{0}^{1} (1 - x) \sin(n \pi x) \, dx \\ & = 2 \left[ \frac{-(x + 1) \cos(n \pi x)}{n \pi} \right]_{-1}^{0} + 2 \int_{-1}^{0} \frac{\cos(n \pi x)}{n \pi} \, dx + 2 \left[ \frac{(1 - x) \cos(n \pi x)}{n \pi} \right]_{0}^{1} - 2 \int_{0}^{1} \frac{\cos(n \pi x)}{n \pi} \, dx \\ & = \frac{4}{n \pi} \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{(2n-1)^2} \\ & = \frac{4}{\pi^2} \sum_{n=1}^{\infty} \frac{\cos((2n-1) \pi x)}{(2n-1)^2} \\ \text{Fourier series:} & \quad f(x) = \frac{1}{2} + \frac{4}{\pi^2} \sum_{n=1}^{\infty} \frac{\cos((2n-1) \pi x)}{(2n-1)^2} \end{align*}
$$


![[Pasted image 20240726174210.png]]

$$\text{Graph of $f(x)$ periodically extended for three periods.}$$
### 18


$$
\begin{align*}
\text{Given:} & \quad f(x) = 
\begin{cases} 
0, & -2 \leq x \leq -1 \\
x, & -1 < x < 1 \\
0, & 1 \leq x < 2 
\end{cases}, \quad f(x+4) = f(x) \\
\text{Period:} & \quad T = 4 \\
\text{Fourier series:} & \\
a_0 & = \frac{1}{4} \int_{-2}^{2} f(x) \, dx = \frac{1}{4} \left( \int_{-1}^{1} x \, dx \right) = \frac{1}{4} \left( \left[ \frac{x^2}{2} \right]_{-1}^{1} \right) = \frac{1}{4} \left( \frac{1}{2} - \frac{1}{2} \right) = 0 \\
a_n & = \frac{1}{2} \int_{-2}^{2} f(x) \cos\left( \frac{n \pi x}{2} \right) \, dx = \frac{1}{2} \left( \int_{-1}^{1} x \cos\left( \frac{n \pi x}{2} \right) \, dx \right) \\
& = \frac{1}{2} \left[ x \frac{2}{n \pi} \sin\left( \frac{n \pi x}{2} \right) \right]_{-1}^{1} - \frac{1}{2} \int_{-1}^{1} \frac{2}{n \pi} \sin\left( \frac{n \pi x}{2} \right) \, dx \\
& = \frac{2}{n \pi} \left( \left[ x \sin\left( \frac{n \pi x}{2} \right) \right]_{-1}^{1} - \int_{-1}^{1} \sin\left( \frac{n \pi x}{2} \right) \, dx \right) \\
& = \frac{2}{n \pi} \left( 0 - \int_{-1}^{1} \sin\left( \frac{n \pi x}{2} \right) \, dx \right) \\
& = \frac{2}{n \pi} \left( -\frac{4}{n \pi} \cos\left( \frac{n \pi x}{2} \right) \right)_{-1}^{1} = 0 \quad (\text{since integral of odd function over symmetric interval is zero}) \\
b_n & = \frac{1}{2} \int_{-2}^{2} f(x) \sin\left( \frac{n \pi x}{2} \right) \, dx = \frac{1}{2} \left( \int_{-1}^{1} x \sin\left( \frac{n \pi x}{2} \right) \, dx \right) \\
& = \frac{1}{2} \left[ -x \frac{2}{n \pi} \cos\left( \frac{n \pi x}{2} \right) \right]_{-1}^{1} + \frac{1}{2} \int_{-1}^{1} \frac{2}{n \pi} \cos\left( \frac{n \pi x}{2} \right) \, dx \\
& = \frac{2}{n \pi} \left( \left[ -x \cos\left( \frac{n \pi x}{2} \right) \right]_{-1}^{1} + \frac{4}{(n \pi)^2} \sin\left( \frac{n \pi x}{2} \right) \right) \\
& = \frac{2}{n \pi} \left( 0 + \frac{4}{(n \pi)^2} \right) = \frac{8}{(n \pi)^2} \\
\text{Fourier series:} & \quad f(x) = \sum_{n=1}^{\infty} \left( -\frac{2}{n \pi} \cos\left( \frac{n \pi}{2} \right) + \left( \frac{2}{n \pi} \right)^2 \sin\left( \frac{n \pi}{2} \right) \right) \sin\left( \frac{n \pi x}{2} \right)
\end{align*}
$$


![[Pasted image 20240726174608.png]]

$$
 \text{Graph of $f(x)$ periodically extended for three periods.}
$$
### 29


$$
\text{(a) Let } \mathbf{v_1}, \mathbf{v_2}, \mathbf{v_3} \text{ be a set of mutually orthogonal vectors in three dimensions, and let } \mathbf{u} \text{ be any three-dimensional vector. Show that:}
$$

$$
\mathbf{u} = a_1 \mathbf{v_1} + a_2 \mathbf{v_2} + a_3 \mathbf{v_3}
$$

$$
\text{where } a_i = \frac{\mathbf{u} \cdot \mathbf{v_i}}{\mathbf{v_i} \cdot \mathbf{v_i}}, \quad i = 1, 2, 3.
$$

$$
\text{This shows that } a_i \text{ can be interpreted as the projection of } \mathbf{u} \text{ in the direction of } \mathbf{v_i} \text{ divided by the length of } \mathbf{v_i}.
$$

$$
\text{(b) Define the inner product } (\mathbf{u}, \mathbf{v}) \text{ by}
$$

$$
(\mathbf{u}, \mathbf{v}) = \int_{-L}^{L} u(x) v(x) \, dx.
$$

$$
\text{Let } \phi_n(x) = \cos\left(\frac{n \pi x}{L}\right), \quad n = 0, 1, 2, \ldots; \quad \psi_n(x) = \sin\left(\frac{n \pi x}{L}\right), \quad n = 1, 2, \ldots.
$$

$$
\text{(c) Use equation (32) and the corresponding equation for } (\mathbf{f}, \psi_n), \text{ together with the orthogonality relations, to show that}
$$

$$
a_n = \frac{(\mathbf{f}, \phi_n)}{(\phi_n, \phi_n)}, \quad n = 0, 1, 2, \ldots; \quad b_n = \frac{(\mathbf{f}, \psi_n)}{(\psi_n, \psi_n)}, \quad n = 1, 2, \ldots.
$$

$$
\text{Equation (32) can be written in the form}
$$

$$
(f, \phi_n) = \frac{a_0}{2} (\phi_0, \phi_n) + \sum_{m=1}^{\infty} a_m (\phi_m, \phi_n) + \sum_{m=1}^{\infty} b_m (\psi_m, \phi_n).
$$

$$
\text{With the orthogonality relations, we get}
$$

$$
a_n = \frac{(f, \phi_n)}{(\phi_n, \phi_n)}, \quad n = 0, 1, 2, \ldots;
$$

$$
b_n = \frac{(f, \psi_n)}{(\psi_n, \psi_n)}, \quad n = 1, 2, \ldots.
$$


## Section 10.3


### 2

$$ \text{(a) Fourier series for the extended function:} $$ $$ a_0 = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \, dx = \frac{1}{\pi} \left( \int_{0}^{\pi} x \, dx \right) = \frac{1}{\pi} \left[ \frac{x^2}{2} \right]_0^{\pi} = \frac{\pi^2}{2\pi} = \frac{\pi}{2} $$ $$ a_n = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \cos(nx) \, dx = \frac{1}{\pi} \left( \int_{0}^{\pi} x \cos(nx) \, dx \right) $$ $$ a_n = \frac{1}{\pi} \left( \left[ \frac{x \sin(nx)}{n} \right]_0^{\pi} - \int_{0}^{\pi} \frac{\sin(nx)}{n} \, dx \right) = \frac{1}{\pi} \left( \frac{\pi \sin(n\pi)}{n} - \frac{1}{n^2} \left[ -\cos(nx) \right]_0^{\pi} \right) $$ $$ a_n = \frac{1}{\pi} \left( 0 + \frac{1}{n^2} \left( -\cos(n\pi) + 1 \right) \right) = \frac{1}{\pi} \left( \frac{1 - (-1)^n}{n^2} \right) = \begin{cases} 0, & \text{if } n \text{ is even} \\ \frac{2}{\pi n^2}, & \text{if } n \text{ is odd} \end{cases} $$ $$ b_n = \frac{1}{\pi} \int_{-\pi}^{\pi} f(x) \sin(nx) \, dx = \frac{1}{\pi} \left( \int_{0}^{\pi} x \sin(nx) \, dx \right) $$ $$ b_n = \frac{1}{\pi} \left( \left[ -\frac{x \cos(nx)}{n} \right]_0^{\pi} + \int_{0}^{\pi} \frac{\cos(nx)}{n} \, dx \right) = \frac{1}{\pi} \left( \frac{\pi \cos(n\pi)}{n} - \frac{1}{n^2} \left[ \sin(nx) \right]_0^{\pi} \right) $$ $$ b_n = \frac{1}{\pi} \left( \frac{\pi (-1)^n}{n} - \frac{1}{n^2} (0) \right) = \frac{(-1)^n}{n} $$ $$ \text{Fourier series:} \quad f(x) = \frac{\pi}{4} - \sum_{n=1}^{\infty} \left( \frac{2}{(2n-1)^2 \pi} \cos((2n-1)x) + \frac{(-1)^n}{n} \sin(nx) \right) $$

![[Pasted image 20240726175517.png]]

$$\text{Graph of $f(x)$ periodically extended for three periods.}$$
### 4

$$ a_0 = \frac{1}{2} \int_{-1}^{1} (1 - x^2) \, dx = \frac{1}{2} \left( \int_{-1}^{1} 1 \, dx - \int_{-1}^{1} x^2 \, dx \right) = \frac{1}{2} \left( 2 - \frac{2}{3} \right) = \frac{2}{3} $$ $$ a_n = \int_{-1}^{1} (1 - x^2) \cos(n \pi x) \, dx $$ $$ a_n = 2 \int_{0}^{1} (1 - x^2) \cos(n \pi x) \, dx $$ $$ \int_{0}^{1} x^2 \cos(n \pi x) \, dx = \left( \frac{x^2 \sin(n \pi x)}{n \pi} \right)_0^1 - \int_{0}^{1} \frac{2x \sin(n \pi x)}{n \pi} \, dx $$ $$ = \left( \frac{1 \cdot \sin(n \pi)}{n \pi} - 0 \right) - \left[ \frac{2}{n \pi} \int_{0}^{1} x \sin(n \pi x) \, dx \right] $$ $$ \int_{0}^{1} x \sin(n \pi x) \, dx = \left( -\frac{x \cos(n \pi x)}{n \pi} \right)_0^1 + \int_{0}^{1} \frac{\cos(n \pi x)}{n \pi} \, dx $$ $$ = \left( -\frac{1 \cdot \cos(n \pi)}{n \pi} - 0 \right) + \left( \frac{\sin(n \pi x)}{(n \pi)^2} \right)_0^1 $$ $$ = -\frac{\cos(n \pi)}{n \pi} + 0 $$ $$ \int_{0}^{1} (1 - x^2) \cos(n \pi x) \, dx = \int_{0}^{1} \cos(n \pi x) \, dx - \int_{0}^{1} x^2 \cos(n \pi x) \, dx $$ $$ \int_{0}^{1} \cos(n \pi x) \, dx = \left( \frac{\sin(n \pi x)}{n \pi} \right)_0^1 = 0 $$ $$ a_n = 2 \left( 0 - \left( \frac{(-1)^n - 1}{n^2 \pi^2} \right) \right) = \frac{4 (-1)^{n+1}}{n^2 \pi^2} $$ $$ b_n = \frac{2}{\pi} \int_{-1}^{1} (1 - x^2) \sin(n \pi x) \, dx = 0 $$ $$ \text{Fourier series:} \quad f(x) = \frac{2}{3} + \frac{4}{\pi^2} \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n^2} \cos(n \pi x) $$


![[Pasted image 20240726175825.png]]

$$\text{Graph of $f(x)$ periodically extended for three periods.}$$
### 13


$$
\begin{aligned}
\text{Given:} & \quad y'' + \omega^2 y = \sin(nt), \quad y(0) = 0, \quad y'(0) = 0 \\
\text{For } \omega^2 \neq n^2: & \\
y_p(t) & = \frac{\sin(nt)}{\omega^2 - n^2} \\
\text{General solution:} & \\
y(t) & = c_1 \cos(\omega t) + c_2 \sin(\omega t) + \frac{\sin(nt)}{\omega^2 - n^2} \\
\text{Applying initial conditions:} & \\
y(0) & = c_1 + \frac{0}{\omega^2 - n^2} = 0 \implies c_1 = 0 \\
y'(0) & = \omega c_2 + \frac{n \cos(nt)}{\omega^2 - n^2} \bigg|_{t=0} = 0 \implies \omega c_2 = 0 \\
c_2 & = 0 \implies y(t) = \frac{\sin(nt)}{\omega^2 - n^2} \\
\text{For } \omega^2 = n^2: & \\
y_p(t) & = \frac{t \cos(nt)}{2n} \\
\text{General solution:} & \\
y(t) & = c_1 \cos(nt) + c_2 \sin(nt) + \frac{t \cos(nt)}{2n} \\
\text{Applying initial conditions:} & \\
y(0) & = c_1 + \frac{0 \cdot \cos(0)}{2n} = 0 \implies c_1 = 0 \\
y'(0) & = n c_2 + \left( \frac{t \cdot (-n \sin(nt))}{2n} + \frac{\cos(nt)}{2n} \right) \bigg|_{t=0} = 0 \implies c_2 = 0 \\
\text{Thus,} & \quad y(t) = \frac{\sin(nt) - nt \cos(nt)}{2n^2}
\end{aligned}
$$

### 14

$$
\text{Given the initial value problem:}
$$

$$
y'' + \omega^2 y = \sin(nt), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
\text{where } n \text{ is a positive integer and } \omega^2 \neq n^2.
$$

$$
\text{Case 1: } \omega \neq n
$$

$$
y(t) = \sum_{n=1}^{\infty} b_n \sin(nt)
$$

$$
\left( \sum_{n=1}^{\infty} b_n (n^2 \sin(nt)) \right) + \omega^2 \left( \sum_{n=1}^{\infty} b_n \sin(nt) \right) = \sin(nt)
$$

$$
b_n (n^2 + \omega^2) = 1
$$

$$
b_n = \frac{1}{n^2 + \omega^2}
$$

$$
y_p(t) = \sum_{n=1}^{\infty} \frac{1}{n^2 + \omega^2} \sin(nt)
$$

$$
y(t) = A \cos(\omega t) + B \sin(\omega t) + \sum_{n=1}^{\infty} \frac{1}{n^2 + \omega^2} \sin(nt)
$$

$$
A = 0, \quad B = 0
$$

$$
y(t) = \sum_{n=1}^{\infty} \frac{\sin(nt)}{n^2 + \omega^2}
$$

$$
y = \sum_{n=1}^{\infty} \frac{b_n (\omega \sin(nt) - n \sin(\omega t))}{\omega (\omega^2 - n^2)}
$$

$$
\text{Case 2: } \omega = m
$$

$$
y(t) = \sum_{n=1}^{\infty} b_n \sin(nt)
$$

$$
\left( \sum_{n=1}^{\infty} b_n (n^2 \sin(nt)) \right) + m^2 \left( \sum_{n=1}^{\infty} b_n \sin(nt) \right) = \sin(nt)
$$

$$
b_n (n^2 + m^2) = 1, \quad b_n = \frac{1}{n^2 + m^2}
$$

$$
y_p(t) = \sum_{n=1, n \neq m}^{\infty} \frac{1}{n^2 + m^2} \sin(nt) + \frac{b_m (\sin(mt) - mt \cos(mt))}{2m^2}
$$

$$
y(t) = A \cos(m t) + B \sin(m t) + \sum_{n=1, n \neq m}^{\infty} \frac{1}{n^2 + m^2} \sin(nt) + \frac{b_m (\sin(mt) - mt \cos(mt))}{2m^2}
$$

$$
A = 0, \quad B = 0
$$

$$
y(t) = \sum_{n=1, n \neq m}^{\infty} \frac{1}{n^2 + m^2} \sin(nt) + \frac{b_m (\sin(mt) - mt \cos(mt))}{2m^2}
$$

$$
y = \sum_{n=1, n \neq m}^{\infty} \frac{b_n (m \sin(nt) - n \sin(mt))}{m (m^2 - n^2)} + \frac{b_m (\sin(mt) - mt \cos(mt))}{2m^2}
$$

### 15


$$
\text{Given:} \quad f(t) = \begin{cases} 
1, & 0 < t < \pi \\
0, & t = 0, \pi, 2\pi \\
-1, & \pi < t < 2\pi 
\end{cases}
$$

The Fourier series of \( f(t) \) is:

$f(t) = \frac{4}{\pi} \sum_{n=1,3,5,\ldots} \frac{1}{n} \sin(nt)$


Now, consider the differential equation:

$y'' + \omega^2 y = f(t)$

Express \( y \) as a Fourier series:
\
$y = \sum_{n=1}^{\infty} b_n \sin(nt)$

Thus,

$\sum_{n=1}^{\infty} b_n (-(n^2 - \omega^2) \sin(nt)) = \frac{4}{\pi} \sum_{n=1,3,5,\ldots} \frac{1}{n} \sin(nt)$


$b_n (-(n^2 - \omega^2)) = \frac{4}{\pi} \frac{1}{n}$

Solve for $b_n$ :

$b_n = \frac{4}{\pi} \frac{1}{n(n^2 - \omega^2)}$


Therefore, the solution is:

$y = \sum_{n=1,3,5,\ldots} \frac{4}{\pi} \frac{1}{n(n^2 - \omega^2)} \sin(nt)$

Combine the terms:

$y = \frac{4}{\pi} \sum_{n=1,3,5,\ldots} \frac{1}{n(n^2 - \omega^2)} \sin(nt)$



### 17


$$
\begin{align*}
f(x) &= \frac{a_0}{2} + \sum_{n=1}^{\infty} \left( a_n \cos\left( \frac{n \pi x}{L} \right) + b_n \sin\left( \frac{n \pi x}{L} \right) \right), \\
\frac{1}{L} \int_{-L}^{L} [f(x)]^2 dx &= \frac{1}{L} \int_{-L}^{L} \left( \frac{a_0}{2} + \sum_{n=1}^{\infty} \left( a_n \cos\left( \frac{n \pi x}{L} \right) + b_n \sin\left( \frac{n \pi x}{L} \right) \right) \right)^2 dx, \\
&= \frac{1}{L} \int_{-L}^{L} \left( \frac{a_0^2}{4} + \sum_{n=1}^{\infty} \left( \frac{a_0 a_n}{2} \cos\left( \frac{n \pi x}{L} \right) + \frac{a_0 b_n}{2} \sin\left( \frac{n \pi x}{L} \right) \right) \right. \\
&\quad + \sum_{m=1}^{\infty} \sum_{n=1}^{\infty} \left( a_m a_n \cos\left( \frac{m \pi x}{L} \right) \cos\left( \frac{n \pi x}{L} \right) + a_m b_n \cos\left( \frac{m \pi x}{L} \right) \sin\left( \frac{n \pi x}{L} \right) \right. \\
&\quad \left. \left. + b_m a_n \sin\left( \frac{m \pi x}{L} \right) \cos\left( \frac{n \pi x}{L} \right) + b_m b_n \sin\left( \frac{m \pi x}{L} \right) \sin\left( \frac{n \pi x}{L} \right) \right) \right) dx, \\
&= \frac{a_0^2}{4} + \sum_{n=1}^{\infty} \frac{a_0 a_n}{2L} \int_{-L}^{L} \cos\left( \frac{n \pi x}{L} \right) dx + \sum_{n=1}^{\infty} \frac{a_0 b_n}{2L} \int_{-L}^{L} \sin\left( \frac{n \pi x}{L} \right) dx \\
&\quad + \sum_{m=1}^{\infty} \sum_{n=1}^{\infty} \left( a_m a_n \frac{1}{L} \int_{-L}^{L} \cos\left( \frac{m \pi x}{L} \right) \cos\left( \frac{n \pi x}{L} \right) dx \right. \\
&\quad + a_m b_n \frac{1}{L} \int_{-L}^{L} \cos\left( \frac{m \pi x}{L} \right) \sin\left( \frac{n \pi x}{L} \right) dx \\
&\quad + b_m a_n \frac{1}{L} \int_{-L}^{L} \sin\left( \frac{m \pi x}{L} \right) \cos\left( \frac{n \pi x}{L} \right) dx \\
&\quad \left. + b_m b_n \frac{1}{L} \int_{-L}^{L} \sin\left( \frac{m \pi x}{L} \right) \sin\left( \frac{n \pi x}{L} \right) dx \right), \\
&= \frac{a_0^2}{4} + \sum_{n=1}^{\infty} \left( \frac{a_n^2}{2} + \frac{b_n^2}{2} \right), \\
\frac{1}{L} \int_{-L}^{L} [f(x)]^2 dx &= \frac{a_0^2}{2} + \sum_{n=1}^{\infty} \left( a_n^2 + b_n^2 \right).
\end{align*}
$$


## Section 10.4

### 3


$$f(x) = \tan(2x) 
\text{Odd Function:} 
\text{Since } \tan(-2x) = -\tan(2x), \text{ the function is odd.}
$$
### 5

$f(x) = |x|^3$
$\text{Even Function:} \text{Since } (|-x|)^3 = |x|^3, \text{ the function is even.}$

### 6

$f(x) = e^{-x}$ 
$$\text{Neither Even nor Odd:} 
\text{Since } e^{-(-x)} = e^{x} \neq e^{-x}, \text{ the function is neither.}$$ 


### 7

$$f(x) = 
\begin{cases} 
x & 0 \leq x < 2 \\
1 & 2 \leq x < 3 
\end{cases}$$
$$\text{Even Extension:} \\
f_{\text{even}}(x) = 
\begin{cases} 
-x & -2 < x \leq 0 \\
x & 0 \leq x < 2 \\
2-x & 2 \leq x < 4
\end{cases}$$ 

$$\text{Odd Extension:} \\
f_{\text{odd}}(x) = 
\begin{cases} 
-x & -2 < x \leq 0 \\
x & 0 \leq x < 2 \\
-x & 2 \leq x < 4
\end{cases}$$


![[Pasted image 20240726212743.png]]

### 12

$f(x) = 4 - x^2$ 
$$\text{Even Function:} \\
\text{Since } (4 - (-x)^2) = 4 - x^2, \text{ the function is even.}$$
### 16

Given:
$$f(x) = 
\begin{cases} 
x, & 0 < x < 1 \\
1, & 1 \leq x < 2 
\end{cases}$$


To find the Fourier sine series for $f(x)$, we need to compute the coefficients \($b_n$\):

$b_n = \frac{2}{L} \int_{0}^{L} f(x) \sin\left(\frac{n\pi x}{L}\right) dx$ 

Given \( $L = 2$ \), we have:

$b_n = \frac{1}{2} \left( \int_{0}^{1} x \sin\left(\frac{n\pi x}{2}\right) dx + \int_{1}^{2} 1 \sin\left(\frac{n\pi x}{2}\right) dx \right)$

Computing the first integral:

$\int_{0}^{1} x \sin\left(\frac{n\pi x}{2}\right) dx$

Using integration by parts, let \( $u = x$ \) and \( $dv = \sin\left(\frac{n\pi x}{2}\right) dx$\). Then \( $du = dx$ \) and \( $v = -\frac{2}{n\pi} \cos\left(\frac{n\pi x}{2}\right)$ \). 

$\int u \, dv = uv - \int v \, du$


$\int_{0}^{1} x \sin\left(\frac{n\pi x}{2}\right) dx = \left. -\frac{2x}{n\pi} \cos\left(\frac{n\pi x}{2}\right) \right|_{0}^{1} + \frac{2}{n\pi} \int_{0}^{1} \cos\left(\frac{n\pi x}{2}\right) dx$ 


Evaluating the first term:

$\left. -\frac{2x}{n\pi} \cos\left(\frac{n\pi x}{2}\right) \right|_{0}^{1} = -\frac{2}{n\pi} \cos\left(\frac{n\pi}{2}\right) + 0 = -\frac{2}{n\pi} \cos\left(\frac{n\pi}{2}\right)$

Computing the second integral:

$\frac{2}{n\pi} \int_{0}^{1} \cos\left(\frac{n\pi x}{2}\right) dx = \frac{2}{n\pi} \left. \frac{2}{n\pi} \sin\left(\frac{n\pi x}{2}\right) \right|_{0}^{1} = \frac{4}{(n\pi)^2} \sin\left(\frac{n\pi}{2}\right)$

So:

$\int_{0}^{1} x \sin\left(\frac{n\pi x}{2}\right) dx = -\frac{2}{n\pi} \cos\left(\frac{n\pi}{2}\right) + \frac{4}{(n\pi)^2} \sin\left(\frac{n\pi}{2}\right)$

Computing the second integral:

$\int_{1}^{2} \sin\left(\frac{n\pi x}{2}\right) dx = \left. -\frac{2}{n\pi} \cos\left(\frac{n\pi x}{2}\right) \right|_{1}^{2} = -\frac{2}{n\pi} \left( \cos(n\pi) - \cos\left(\frac{n\pi}{2}\right) \right)$

Combining both integrals to find \( $b_n$ \):

$b_n = \frac{1}{2} \left[ -\frac{2}{n\pi} \cos\left(\frac{n\pi}{2}\right) + \frac{4}{(n\pi)^2} \sin\left(\frac{n\pi}{2}\right) -\frac{2}{n\pi} \left( \cos(n\pi) - \cos\left(\frac{n\pi}{2}\right) \right) \right]$

Simplifying further, we get the Fourier sine series:

$f(x) = \sum_{n=1}^{\infty} \frac{2}{n\pi} \left( -\cos(n\pi) + \frac{\sin\left(\frac{n\pi}{2}\right)}{n\pi} \right) \sin\left(\frac{n\pi x}{2}\right)$


### 17


Given:

$f(x) = 1, \quad 0 \leq x \leq \pi$


This function is already constant and has a cosine series representation. The Fourier series is given by:

$a_0 = \frac{1}{\pi} \int_{0}^{\pi} f(x) \, dx = 1$

For \( $n \geq 1$ \):

$a_n = \frac{2}{\pi} \int_{0}^{\pi} 1 \cdot \cos(nx) \, dx = \frac{2}{\pi} \left[ \frac{\sin(nx)}{n} \right]_{0}^{\pi} = 0$


Therefore, the Fourier series representation is:

$f(x) = 1$



### 35


$$\begin{aligned}
&\text{Given the square wave function in Example 1 of Section 10.3:} \\
&f(x) = 
\begin{cases} 
L, & 0 < x < L \\
0, & -L < x < 0 
\end{cases} \\
&\text{The Fourier series of } f(x) \text{ is:} \\
&f(x) = \frac{L}{2} + \frac{2L}{\pi} \sum_{n=1, 3, 5, \ldots}^{\infty} \frac{1}{n} \sin \left( \frac{n\pi x}{L} \right) \\
&\text{Setting } L = \frac{\pi}{2} \text{ and evaluating at } x = \frac{\pi}{2}, \text{ we get:} \\
&\frac{\pi}{4} = \frac{\pi}{4} + \sum_{n=1, 3, 5, \ldots}^{\infty} \frac{(-1)^{(n-1)/2}}{n} \\
&\frac{\pi}{4} = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n + 1} \\
&\text{Thus, } \frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots \end{aligned}$$



### 36


$$\begin{aligned}
&\text{Given the triangular wave function in Example 1 of Section 10.2:} \\
&f(x) = 
\begin{cases} 
\frac{4}{\pi^2} \sum_{n=0}^{\infty} \frac{(-1)^n}{(2n+1)^2} \cos \left( \frac{(2n+1)\pi x}{L} \right), & -L < x < L \\
0, & \text{otherwise}
\end{cases} \\
&\text{Setting } L = \pi \text{ and evaluating at } x = 0, \text{ we get:} \\
&\frac{\pi^2}{8} = \sum_{n=0}^{\infty} \frac{1}{(2n+1)^2} \\
&\text{Thus, } \frac{\pi^2}{8} = 1 + \frac{1}{3^2} + \frac{1}{5^2} + \frac{1}{7^2} + \cdots
\end{aligned}$$
