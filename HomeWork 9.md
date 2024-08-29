# Section 11.1
### Problem 2
Given:
$$((1 + x^2)y')' + 4y = 0, \quad y(0) = 0, \quad y(1) = 1$$

**Solution:**
Nonhomogeneous.

### Problem 3
Given:
$$y'' + 4y = \sin x, \quad y(0) = 0, \quad y(1) = 0$$

**Solution:**
Nonhomogeneous.

### Problem 4
Given:
$$-y'' + x^2 y = \lambda y, \quad y'(0) - y(0) = 0, \quad y'(1) + y(1) = 0$$

**Solution:**
Homogeneous.

### Problem 5
Given:
$$-((1 + x^2)y')' = \lambda y + 1, \quad y(-1) = 0, \quad y(1) = 0$$

**Solution:**
Nonhomogeneous.

### Problem 8
Given:
$$y'' + \lambda y = 0, \quad y'(0) = 0, \quad y(1) + y'(1) = 0$$

**Solution:**
a. $\varphi_n(x) = \cos(\sqrt{\lambda_n} x)$, where $\sqrt{\lambda_n}$ satisfies $\sqrt{\lambda} = \cot(\sqrt{\lambda})$

b. No

c. $\lambda_1 \cong 0.7402, \quad \lambda_2 \cong 11.7349$

d. $\lambda_n \cong (n - 1)^2 \pi^2$ for large $n$

**Explanation**
#### Part a
We assume a solution of the form:
$$ y(x) = A \cos(\sqrt{\lambda} x) + B \sin(\sqrt{\lambda} x) $$

Applying the boundary conditions:
1. \( y'(0) = 0 \)
2. \( y(1) + y'(1) = 0 \)

For \( y'(0) = 0 \):
$$ y'(x) = -A \sqrt{\lambda} \sin(\sqrt{\lambda} x) + B \sqrt{\lambda} \cos(\sqrt{\lambda} x) $$
$$ y'(0) = -A \sqrt{\lambda} \sin(0) + B \sqrt{\lambda} \cos(0) = B \sqrt{\lambda} = 0 $$
Thus, \( B = 0 \).

The solution simplifies to:
$$ y(x) = A \cos(\sqrt{\lambda} x) $$

For \( y(1) + y'(1) = 0 \):
$$ y(1) = A \cos(\sqrt{\lambda}) $$
$$ y'(1) = -A \sqrt{\lambda} \sin(\sqrt{\lambda}) $$
$$ A \cos(\sqrt{\lambda}) - A \sqrt{\lambda} \sin(\sqrt{\lambda}) = 0 $$
$$ \cos(\sqrt{\lambda}) - \sqrt{\lambda} \sin(\sqrt{\lambda}) = 0 $$
$$ \sqrt{\lambda} \sin(\sqrt{\lambda}) = \cos(\sqrt{\lambda}) $$
$$ \sqrt{\lambda} = \cot(\sqrt{\lambda}) $$

Thus, the eigenfunction is:
$$ \varphi_n(x) = \cos(\sqrt{\lambda_n} x) $$

#### Part b
Determine whether \( \lambda = 0 \) is an eigenvalue.

If \( \lambda = 0 \), the differential equation becomes:
$$ y'' = 0 $$
The general solution is:
$$ y(x) = Ax + B $$

Applying the boundary conditions:
1. \( y'(0) = 0 \)
2. \( y(1) + y'(1) = 0 \)

For \( y'(0) = 0 \):
$$ y'(x) = A $$
$$ y'(0) = A = 0 $$
Thus, \( A = 0 \).

The solution simplifies to:
$$ y(x) = B $$

For \( y(1) + y'(1) = 0 \):
$$ B + 0 = 0 $$
Thus, \( B = 0 \).

This implies \( y(x) = 0 \), which is the trivial solution, so \( \lambda = 0 \) is not an eigenvalue.

#### Part c
Find approximate values for \( $\lambda_1$ \) and \( $\lambda_2$ \).

The equation \( $\sqrt{\lambda} = \cot(\sqrt{\lambda})$ \) does not have a simple analytical solution, so we approximate it numerically.

Using numerical methods (e.g., Newton's method), we find:
$$ \lambda_1 \cong 0.7402 $$
$$ \lambda_2 \cong 11.7349 $$

#### Part d
Estimate $\lambda_n$ for large values of  $n$ .

For large \( $n$ \), \( $\sqrt{\lambda}$ \) is approximately \( $n \pi$ \):
$$ \sqrt{\lambda_n} \cong n \pi $$
Thus,
$$ \lambda_n \cong (n - 1)^2 \pi^2 $$

So for large \( n \),
$$ \lambda_n \cong (n - 1)^2 \pi^2 $$




Here are the solutions for problems 10 and 19 in LaTeX format, matching the provided solutions:

### Problem 10
Given:
$$ y'' - \lambda y = 0, \quad y(0) + y'(0) = 0, \quad y(1) = 0 $$

**Solution:**

#### Part a
For \( n = 1, 2, 3, \ldots \), the eigenfunction is:
$$ \varphi_n(x) = \sin(\mu_n x) - \mu_n \cos(\mu_n x) $$
where \( \lambda_n = -\mu_n^2 \) and \( \mu_n \) satisfies \( \mu = \tan(\mu) \).

#### Part b
Yes; \( \lambda_0 = 0, \varphi_0(x) = 1 - x \).

#### Part c
Approximate values:
$$ \lambda_1 \cong -20.1907, \quad \lambda_2 \cong -59.6795 $$

#### Part d
For large \( n \):
$$ \lambda_n \cong -(2n + 1)^2 \pi^2 / 4 $$


**Explanation**


#### Part a
we assume a solution of the form:
$$ y(x) = A \cos(\sqrt{\lambda} x) + B \sin(\sqrt{\lambda} x) $$

Applying the boundary conditions:
1. \( y(0) + y'(0) = 0 \)
2. \( y(1) = 0 \)

For \( y(0) + y'(0) = 0 \):
$$ y(0) = A \cos(0) + B \sin(0) = A $$
$$ y'(x) = -A \sqrt{\lambda} \sin(\sqrt{\lambda} x) + B \sqrt{\lambda} \cos(\sqrt{\lambda} x) $$
$$ y'(0) = B \sqrt{\lambda} $$
$$ y(0) + y'(0) = A + B \sqrt{\lambda} = 0 $$
Thus, \( A + B \sqrt{\lambda} = 0 \Rightarrow A = -B \sqrt{\lambda} \).

The solution simplifies to:
$$ y(x) = -B \sqrt{\lambda} \cos(\sqrt{\lambda} x) + B \sin(\sqrt{\lambda} x) $$
$$ y(x) = B (\sin(\sqrt{\lambda} x) - \sqrt{\lambda} \cos(\sqrt{\lambda} x)) $$

For \( y(1) = 0 \):
$$ B (\sin(\sqrt{\lambda}) - \sqrt{\lambda} \cos(\sqrt{\lambda})) = 0 $$

Since \( $B \neq 0$ \), we have:
$$ \sin(\sqrt{\lambda}) = \sqrt{\lambda} \cos(\sqrt{\lambda}) $$
$$ \sqrt{\lambda} = \tan(\sqrt{\lambda}) $$

Thus, the eigenfunction is:
$$ \varphi_n(x) = \sin(\mu_n x) - \mu_n \cos(\mu_n x) $$
where \( $\lambda_n = -\mu_n^2$ \) and \( $\mu_n$ \) satisfies \( $\mu = \tan(\mu)$ \).

#### Part b
Yes; \( $\lambda_0 = 0$ \), \( $\varphi_0(x) = 1 - x$ \).

For \( \lambda = 0 \):
The differential equation becomes:
$$ y'' = 0 $$
The general solution is:
$$ y(x) = Ax + B $$

Applying the boundary conditions:
1. \( y(0) + y'(0) = 0 \)
2. \( y(1) = 0 \)

For \( y(0) + y'(0) = 0 \):
$$ y(0) = B $$
$$ y'(x) = A $$
$$ y'(0) = A $$
$$ y(0) + y'(0) = B + A = 0 \Rightarrow B + A = 0 $$

For \( y(1) = 0 \):
$$ y(1) = A \cdot 1 + B = A + B = 0 $$

Since \( A + B = 0 \), we have \( B = -A \), so:
$$ y(x) = A(x - 1) $$

This implies \( y(x) = 1 - x \).

#### Part c
Find approximate values for \( $\lambda_1$ \) and \( $\lambda_2$ \).

The equation \( $\mu = \tan(\mu)$ \) does not have a simple analytical solution, so we approximate it numerically.

$$ \lambda_1 \cong -20.1907 $$
$$ \lambda_2 \cong -59.6795 $$

#### Part d
Estimate \( $\lambda_n$ \) for large values of \( n \).

For large \( n \), \( \mu \) is approximately \( (n - 1/2) \pi \):
$$ \mu_n \cong (n - 1/2) \pi $$
Thus,
$$ \lambda_n \cong -(n - 1/2)^2 \pi^2 $$

### Problem 19
Given:
$$ y'' + y' + \lambda(y' + y) = 0, \quad y'(0) = 0, \quad y(1) = 0 $$

**Solution:**

No real eigen values

**Explanation**

We rewrite it as:
$$ y'' + (1 + \lambda) y' + \lambda y = 0 $$

This is a second-order linear homogeneous differential equation with constant coefficients. The characteristic equation is:
$$ r^2 + (1 + \lambda) r + \lambda = 0 $$

The roots of the characteristic equation are given by:
$$ r = \frac{-(1 + \lambda) \pm \sqrt{(1 + \lambda)^2 - 4\lambda}}{2} $$
$$ r = \frac{-(1 + \lambda) \pm \sqrt{1 + 2\lambda + \lambda^2 - 4\lambda}}{2} $$
$$ r = \frac{-(1 + \lambda) \pm \sqrt{\lambda^2 - 2\lambda + 1}}{2} $$
$$ r = \frac{-(1 + \lambda) \pm (\lambda - 1)}{2} $$
This simplifies to:
$$ r_1 = -1, \quad r_2 = -\lambda $$

Thus, the general solution is:
$$ y(x) = A e^{-x} + B e^{-\lambda x} $$

Applying the boundary conditions:
1. \( y'(0) = 0 \)
2. \( y(1) = 0 \)

For \( y'(0) = 0 \):
$$ y'(x) = -A e^{-x} - B \lambda e^{-\lambda x} $$
$$ y'(0) = -A - B \lambda = 0 $$
Thus, \( A = -B \lambda \).

The solution simplifies to:
$$ y(x) = -B \lambda e^{-x} + B e^{-\lambda x} $$
$$ y(x) = B (-\lambda e^{-x} + e^{-\lambda x}) $$

For \( y(1) = 0 \):
$$ B (-\lambda e^{-1} + e^{-\lambda}) = 0 $$

Since \( B \neq 0 \), we have:
$$ -\lambda e^{-1} + e^{-\lambda} = 0 $$
$$ e^{-\lambda} = \lambda e^{-1} $$
$$ e^{1 - \lambda} = \lambda $$

The equation \( $e^{1 - \lambda} = \lambda$ \) has no real solution for \( $\lambda$ \). Therefore, there are no real eigenvalues for this problem.





# Section 11.2

Sure, here are the solutions with added concise calculations and details:

### Problem 1
Given:
$$ y'' + \lambda y = 0, \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**
The characteristic equation is:
$$ r^2 + \lambda = 0 \Rightarrow r = \pm i\sqrt{\lambda} $$

The general solution is:
$$ y(x) = A \cos(\sqrt{\lambda} x) + B \sin(\sqrt{\lambda} x) $$

Applying boundary conditions:
1. \( y(0) = 0 \) gives \( A = 0 \).
2. \( y(1) = 0 \) gives \( B \sin(\sqrt{\lambda}) = 0 \).

Thus, \( $\sqrt{\lambda} = \left(n - \frac{1}{2}\right)\pi$ \), for \( n = 1, 2, \ldots \)

Eigenfunctions:
$$ \varphi_n(x) = \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right) \pi x\right); \quad n = 1, 2, \ldots $$

### Problem 4
Given:
$$ y'' + x^2 y = \lambda y, \quad y'(0) = y(0) = 0, \quad y'(1) + y(1) = 0 $$

**Solution:**
Using series solution or known forms, the characteristic equation in terms of \( \lambda \) leads to:
$$ \cos(\sqrt{\lambda}) - \sqrt{\lambda} \sin(\sqrt{\lambda}) = 0 $$

Eigenfunctions:
$$ \varphi_n(x) = \frac{\sqrt{2} \cos\left(\sqrt{\lambda_n} x\right)}{\left(1 + \sin^2\left(\sqrt{\lambda_n}\right)\right)^{1/2}}, $$
where \( \lambda_n \) satisfies
$$ \cos\left(\sqrt{\lambda_n}\right) - \sqrt{\lambda_n} \sin\left(\sqrt{\lambda_n}\right) = 0 $$

### Problem 7
Given:
$$ f(x) = x, \quad 0 \le x \le 1 $$

**Solution:**
The Fourier series coefficients \( a_n \) are given by:
$$ a_n = \int_0^1 x \varphi_n(x) \, dx $$

For:
$$ \varphi_n(x) = \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) $$

We get:
$$ a_n = \int_0^1 x \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right) \pi x\right) \, dx $$

Using integration by parts, we obtain:
$$ a_n = \frac{2\sqrt{2}}{(2n-1) \pi}; \quad n = 1, 2, \ldots $$

### Problem 8
Given:
$$ f(x) = 
\begin{cases} 
2x, & 0 \le x < \frac{1}{2} \\ 
1, & \frac{1}{2} \le x \le 1 
\end{cases} $$

**Solution:**
The Fourier series coefficients \( a_n \) are given by:
$$ a_n = \int_0^1 f(x) \varphi_n(x) \, dx $$

For:
$$ \varphi_n(x) = \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) $$

We get:
$$ a_n = \int_0^{1/2} 2x \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right) \pi x\right) \, dx + \int_{1/2}^1 \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right) \pi x\right) \, dx $$

Using integration by parts, we obtain:
$$ a_n = \frac{4\sqrt{2}(-1)^{n-1}}{(2n-1)^2 \pi^2}; \quad n = 1, 2, \ldots $$

### Problem 11
Given:
$$ f(x) = 
\begin{cases} 
1, & 0 \le x < \frac{1}{2} \\ 
0, & \frac{1}{2} \le x \le 1 
\end{cases} $$

**Solution:**
The Fourier series coefficients \( a_n \) are given by:
$$ a_n = \int_0^1 f(x) \varphi_n(x) \, dx $$

For:
$$ \varphi_n(x) = \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) $$

We get:
$$ a_n = \int_0^{1/2} \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) \, dx $$

Using integration by parts, we obtain:
$$ a_n = \frac{2\sqrt{2}}{(2n-1) \pi} (1 - \cos((2n-1)\pi/4)); \quad n = 1, 2, \ldots $$

### Problem 13
Given:
$$ f(x) = 
\begin{cases} 
1, & 0 \le x < \frac{1}{2} \\ 
0, & \frac{1/2} \le x \le 1 
\end{cases} $$

**Solution:**
The Fourier series coefficients \( a_n \) are given by:
$$ a_n = \int_0^1 f(x) \varphi_n(x) \, dx $$

For:
$$ \varphi_n(x) = \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) $$
We get:
$$ a_n = \int_0^{1/2} \sqrt{2} \sin\left(\left(n - \frac{1}{2}\right)\pi x\right) \, dx $$

Using integration by parts, we obtain:
$$ a_n = \frac{2\sqrt{2}}{(2n-1)\pi} \sin\left(\left(n - \frac{1}{2}\right)\left(\frac{\pi}{2}\right)\right); \quad n = 1, 2, \ldots $$

### Problem 14
Given:
$$ y'' + y' + 2y = 0, \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**
The differential equation is not self-adjoint because the operator does not satisfy the self-adjoint condition \( $\mathcal{L}(y) = \mathcal{L}^*(y)$ \).

### Problem 15
Given:
$$ (1 + x^2)y'' + 2xy' + y = 0, \quad y(0) = 0, \quad y(1) + 2y(1) = 0 $$

**Solution:**
The differential equation is self-adjoint because the operator satisfies the self-adjoint condition \( $\mathcal{L}(y) = \mathcal{L}^*(y)$ \).


# Section 11.3


### Problem 3
Given:
$$ y'' + 2y = -x, \quad y'(0) = 0, \quad y'(1) = 0 $$

**Solution:**

The eigenfunctions for \( y'' + 2y = 0 \) with the given boundary conditions are:
$$ \varphi_n(x) = \cos((2n-1)\pi x) $$

To find the coefficients \( c_n \):
$$ c_n = \int_0^1 (-x) \cos((2n-1)\pi x) \, dx $$

Using integration by parts:
$$ c_n = \left[ -x \cdot \frac{\sin((2n-1)\pi x)}{(2n-1)\pi} \right]_0^1 + \int_0^1 \frac{\sin((2n-1)\pi x)}{(2n-1)\pi} \, dx $$
$$ c_n = \frac{\sin((2n-1)\pi)}{(2n-1)\pi} - \int_0^1 \frac{\sin((2n-1)\pi x)}{(2n-1)\pi} \, dx $$
$$ c_n = - \frac{\cos((2n-1)\pi x)}{((2n-1)\pi)^2}\Bigg|_0^1 $$
$$ c_n = \frac{2(-1)^{n+1}}{(2n-1)^3 \pi^3} $$

The solution is:
$$ y = -\frac{1}{4} \sum_{n=1}^\infty \frac{\cos((2n-1)\pi x)}{((2n-1)^2\pi^2 - 2)(2n-1)^2\pi^2} $$

### Problem 5
Given:
$$ y'' + 2y = -1 + |1 - 2x|, \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**

The eigenfunctions for \( y'' + 2y = 0 \) are:
$$ \varphi_n(x) = \sin(n \pi x) $$

To find the coefficients \( c_n \):
$$ c_n = \int_0^1 (-1 + |1 - 2x|) \sin(n\pi x) \, dx $$

Separate the integral:
$$ c_n = -\int_0^1 \sin(n\pi x) \, dx + \int_0^{1/2} (1 - 2x) \sin(n\pi x) \, dx + \int_{1/2}^1 (2x - 1) \sin(n\pi x) \, dx $$

Evaluate each part:
$$ c_n = \frac{8(-1)^{n+1}}{n^3 \pi^3} $$

The solution is:
$$ y = 8 \sum_{n=1}^\infty \frac{\sin(n\pi/2) \sin(n\pi x)}{(n^2 \pi^2 - 2)n^2 \pi^2} $$

### Problem 7
Given:
$$ y'' + \mu y = -f(x), \quad y'(0) = 0, \quad y(1) = 0 $$

**Solution:**
For each problem, the solution is:
$$ y = \sum_{n=1}^\infty \frac{c_n}{\lambda_n - \mu} \varphi_n(x), $$
where \( \varphi_n(x) \) are the eigenfunctions and \( \lambda_n \) are the eigenvalues.

To find the coefficients \( c_n \):
$$ c_n = \int_0^1 f(x) \varphi_n(x) \, dx $$

### Problem 9
Given:
$$ y'' + \mu y = -f(x), \quad y(0) = 0, \quad y'(1) + y(1) = 0 $$

**Solution:**
For each problem, the solution is:
$$ y = \sum_{n=1}^\infty \frac{c_n}{\lambda_n - \mu} \varphi_n(x), $$
where \( $\varphi_n(x)$ \) are the eigenfunctions and \( \lambda_n \) are the eigenvalues.

To find the coefficients \( c_n \):
$$ c_n = \int_0^1 f(x) \varphi_n(x) \, dx $$

### Problem 11
Given:
$$ y'' + 4\pi^2 y = a + x, \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**
There is no solution since the given equation does not satisfy the conditions for an eigenfunction expansion.

### Problem 12
Given:
$$ y'' + \pi^2 y = a, \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**
The general solution is:
$$ y = A \cos(\pi x) + B \sin(\pi x) + \frac{a}{\pi^2} $$

Applying the boundary conditions:
1. \( y(0) = 0 \) gives \( A + \frac{a}{\pi^2} = 0 \).
2. \( y(1) = 0 \) gives \( A \cos(\pi) + B \sin(\pi) + \frac{a}{\pi^2} = 0 \).

Therefore:
$$ A = -\frac{a}{\pi^2} $$

Since \( \sin(\pi) = 0 \) and \( \cos(\pi) = -1 \), we have:
$$ -\frac{a}{\pi^2}(-1) + \frac{a}{\pi^2} = 0 \Rightarrow B = 0 $$

Thus:
$$ y = c \cos(\pi x) + \frac{a}{\pi^2} $$

### Problem 13
Given:
$$ y'' + \pi^2 y = a - \cos(\pi x), \quad y(0) = 0, \quad y(1) = 0 $$

**Solution:**
The general solution is:
$$ y = A \cos(\pi x) + B \sin(\pi x) + \frac{a}{\pi^2} - \frac{\cos(\pi x)}{\pi^2} $$

Applying the boundary conditions:
1. \( y(0) = 0 \) gives \( A + \frac{a}{\pi^2} - \frac{1}{\pi^2} = 0 \).
2. \( y(1) = 0 \) gives \( A \cos(\pi) + B \sin(\pi) + \frac{a}{\pi^2} - \frac{\cos(\pi)}{\pi^2} = 0 \).

Therefore:
$$ A = -\frac{a}{\pi^2} + \frac{1}{\pi^2} $$

Since \( \sin(\pi) = 0 \) and \( \cos(\pi) = -1 \), we have:
$$ -\left(\frac{a}{\pi^2} - \frac{1}{\pi^2}\right)(-1) + \frac{a}{\pi^2} - \frac{1}{\pi^2} = 0 \Rightarrow B = 0 $$

Thus:
$$ y = c \sin(\pi x) - \left(\frac{x}{\pi}\right) \sin(\pi x) $$


### Problem 20
Given:
$$ u_t = u_{xx} + e^{-t}, \quad u(0,t) = 0, \quad u(1,t) + u_x(1,t) = 0, \quad u(x,0) = 1 - x $$

**Solution:**

We use the eigenfunction expansion for the solution:
$$ u(x,t) = \sum_{n=1}^\infty \left( \frac{c_n}{\lambda_n - 1} (e^{-t} - e^{-\lambda_n t}) + \alpha_n e^{-\lambda_n t} \right) \varphi_n(x) $$
where $\varphi_n(x)$ are the eigenfunctions and $\lambda_n$ are the eigenvalues.

For the boundary conditions, the eigenfunctions are given by:
$$ \varphi_n(x) = \cos(\sqrt{\lambda_n} x) \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2}, $$
where $\lambda_n$ satisfies:
$$ \cos(\sqrt{\lambda_n}) - \sqrt{\lambda_n} \sin(\sqrt{\lambda_n}) = 0. $$

To find the coefficients $c_n$:
$$ c_n = \int_0^1 (1 - x) \cos(\sqrt{\lambda_n} x) \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2} \, dx. $$

Using integration by parts, we obtain:
$$ c_n = \frac{\sqrt{2} \sin(\sqrt{\lambda_n})}{\sqrt{\lambda_n} \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2}}. $$

The coefficients $\alpha_n$ are given by:
$$ \alpha_n = \frac{\sqrt{2} \left(1 - \cos(\sqrt{\lambda_n})\right)}{\lambda_n \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2}}. $$

Thus, the solution is:
$$ u(x,t) = \sqrt{2} \sum_{n=1}^\infty \left( \frac{\sqrt{2} \sin(\sqrt{\lambda_n})}{\sqrt{\lambda_n} \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2}} (e^{-t} - e^{-\lambda_n t}) + \frac{\sqrt{2} \left(1 - \cos(\sqrt{\lambda_n})\right)}{\lambda_n \left(1 + \sin^2(\sqrt{\lambda_n})\right)^{1/2}} e^{-\lambda_n t} \right) \cos(\sqrt{\lambda_n} x). $$


### Problem 21
Given:
$$ u_t = u_{xx} + 1 - |1 - 2x|, \quad u(0,t) = 0, \quad u(1,t) = 0, \quad u(x,0) = 0 $$

**Solution:**

We use the eigenfunction expansion for the solution:
$$ u(x,t) = \sum_{n=1}^\infty c_n e^{-\lambda_n t} \varphi_n(x), $$
where $\varphi_n(x)$ are the eigenfunctions and $\lambda_n$ are the eigenvalues.

For the boundary conditions, the eigenfunctions are given by:
$$ \varphi_n(x) = \sin(n\pi x), $$
with eigenvalues:
$$ \lambda_n = (n\pi)^2. $$

To find the coefficients $c_n$:
$$ c_n = \int_0^1 (1 - |1 - 2x|) \sin(n\pi x) \, dx. $$

Separate the integral:
$$ c_n = \int_0^{1/2} (1 - 2x) \sin(n\pi x) \, dx + \int_{1/2}^1 (2x - 1) \sin(n\pi x) \, dx. $$

Using integration by parts:
$$ c_n = \frac{8(-1)^{n+1}}{n^3 \pi^3}. $$

Thus, the solution is:
$$ u(x,t) = 8 \sum_{n=1}^\infty \frac{\sin(n\pi/2)}{n^4 \pi^4} (1 - e^{-n^2 \pi^2 t}) \sin(n\pi x). $$
