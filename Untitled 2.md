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


#### 17


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
