## Section 5.1

### Problem 1
Given the series:
$$ \sum_{n=0}^{\infty} (x - 3)^n $$

**Solution:**

This is a geometric series with ratio \( r = x - 3 \).

The radius of convergence \( \rho \) is given by:
$$ \rho = \frac{1}{|r|} = 1 $$

### Problem 5
Given the series:
$$ \sum_{n=1}^{\infty} \frac{(x - x_0)^n}{n} $$

**Solution:**

We apply the ratio test to find the radius of convergence \( \rho \):
$$ \lim_{n \to \infty} \left|\frac{a_{n+1}}{a_n}\right| = \lim_{n \to \infty} \left|\frac{1}{n+1} \cdot \frac{n}{1}\right| = 1 $$
Thus, the radius of convergence \( \rho = 1 \).

### Problem 12
Given the series:
$$ \sum_{n=0}^{\infty} x^n $$

**Solution:**

This is a geometric series with ratio \( r = x \).

The radius of convergence \( \rho \) is given by:
$$ \rho = \frac{1}{|x|} = 1 $$

### Problem 13
Given the series:
$$ \sum_{n=0}^{\infty} (-1)^n (x - 2)^n $$

**Solution:**

We apply the ratio test to find the radius of convergence \( \rho \):
$$ \lim_{n \to \infty} \left|\frac{(-1)^{n+1} (x - 2)^{n+1}}{(-1)^n (x - 2)^n}\right| = \lim_{n \to \infty} |x - 2| = 1 $$
Thus, the radius of convergence \( \rho = 1 \).

### Problem 18
Rewrite the given expression:
$$ \sum_{n=2}^{\infty} n(n - 1) a_n x^{n-2} $$

**Solution:**

This expression can be rewritten as:
$$ \sum_{n=0}^{\infty} (n+2)(n+1) a_{n+2} x^n $$

### Problem 19
Rewrite the given expression:
$$ x \sum_{n=1}^{\infty} n a_n x^{n-1} + \sum_{k=0}^{\infty} a_k x^k $$

**Solution:**

This expression can be rewritten as:
$$ \sum_{n=0}^{\infty} (n+1) a_{n+1} x^n $$

### Problem 21
Rewrite the given expression:
$$ a_1 + \sum_{n=1}^{\infty} ((n+1)a_{n+1} + a_{n-1}) x^n $$

**Solution:**

This expression can be rewritten as:
$$ a_1 + \sum_{n=0}^{\infty} ((n+1)a_{n+1} + a_n) x^n $$

## Section 5.2


### Problem 2
Given:
$$ y'' + 3y' = 0, \quad x_0 = 0 $$

**Solution:**

The recurrence relation is:
$$ a_{n+2} = \frac{-3}{n+2} a_{n+1} $$

First four nonzero terms:
$$ y_1(x) = 1 + x + \frac{x^2}{2} + \frac{x^3}{6} + \dots $$
$$ y_2(x) = x + \frac{x^2}{2} + \frac{x^3}{6} + \dots $$
The general term for $y_2(x)$ is:
$$ y_2(x) = \sum_{n=0}^{\infty} \frac{(-3)^n}{n!} x^n = \frac{1}{3}(1 - e^{-3x}) $$

### Problem 10
Given:
$$ 2(n+2)(n+1) a_{n+2} + (n+3) 3 a_n = 0 $$

**Solution:**

The recurrence relation is:
$$ a_{n+2} = \frac{-(n+3) 3}{2(n+2)(n+1)} a_n $$

First four nonzero terms:
$$ y_1(x) = 1 - \frac{3}{4} x^2 + \frac{5}{32} x^4 - \frac{7}{384} x^6 + \dots $$
$$ y_2(x) = x - \frac{x^3}{6} + \frac{x^5}{120} + \dots $$

### Problem 15
Given:
$$ y'' + (x-1)^2 y' + (x^2-1) y = 0 $$

**Solution:**

The recurrence relation is:
$$ a_{n+2} = \frac{-(n+1)(n+2)}{(n+1)(n+2) - 2(n+1)} a_n $$

First four nonzero terms:
$$ y_1(x) = 1 - \frac{1}{3}(x-1)^3 + \frac{1}{12}(x-1)^4 + \dots $$
$$ y_2(x) = (x-1) - \frac{1}{4}(x-1)^2 + \dots $$

The Wronskian for $y_1$ and $y_2$ at $x_0 = 1$ confirms that they form a fundamental set of solutions.


## Section 5.3

### Problem 3

Given the differential equation:
$$
y'' + x^2 y' + (\sin x) y = 0
$$
with initial conditions $y(0) = a_0$ and $y'(0) = a_1$.

For $\phi''(0)$, $\phi'''(0)$, and $\phi^{(4)}(0)$.

1. Taylor series expansion:
   $$
   y(x) = \phi(x) = \sum_{n=0}^{\infty} \frac{\phi^{(n)}(0)}{n!}x^n
   $$

2. Substitute into the differential equation and equate coefficients of powers of $x$.

Thus, we find:
$$
\phi''(0) = 0, \quad \phi'''(0) = -a_0, \quad \phi^{(4)}(0) = -4a_1
$$

### Problem 8

Given the Chebyshev equation:
$$
(1-x^2)y'' - x y' + \alpha^2 y = 0
$$

**Part (a):** Determine the solutions in the form of a series around $x=0$.

For small $x$, assume the solution as a power series:
$$
y(x) = \sum_{n=0}^{\infty} c_n x^n
$$

Substituting this series into the equation and solving for the coefficients, we get:
$$
y_1(x) = 1 - \frac{\alpha^2 x^2}{2!} + \frac{(\alpha^2 - 1)(\alpha^2 - 4)x^4}{4!} - \cdots
$$
$$
y_2(x) = x + \frac{1-\alpha^2}{3!}x^3 + \frac{(1-\alpha^2)(9-\alpha^2)}{5!}x^5 + \cdots
$$

**Part (b):** Termination condition.

If $n$ is an integer, either $y_1(x)$ or $y_2(x)$ terminates, forming a polynomial solution.

**Part (c):** Polynomial solutions for $\alpha = n$.

For $n = 0, 1, 2, 3$, the solutions are polynomials that terminate.

### Problem 11

Given the differential equation:
$$
(\cos x)y'' + x y' - 2y = 0
$$

Assume a power series solution:
$$
y(x) = \sum_{n=0}^{\infty} c_n x^n
$$

Substituting into the differential equation and solving for coefficients:
$$
y_1(x) = 1 + \frac{x^2}{2!} + \frac{x^4}{4!} + \cdots = \cosh x
$$
$$
y_2(x) = x + \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots = \sinh x
$$

For the radius of convergence, we find:
$$
\rho = \frac{\pi}{2}
$$


### Problem 15:

**Given:**
$$ (1 - x)y'' = y $$

**Solution:**

Assume a solution of the form \( y(x) = \sum_{n=0}^{\infty} a_n x^n \).

Differentiating, we have:
$$ y'(x) = \sum_{n=1}^{\infty} n a_n x^{n-1} $$
$$ y''(x) = \sum_{n=2}^{\infty} n(n-1) a_n x^{n-2} $$

Substitute into the differential equation:
$$ (1 - x)\sum_{n=2}^{\infty} n(n-1) a_n x^{n-2} = \sum_{n=0}^{\infty} a_n x^n $$

Simplify and match coefficients for each power of \( x \):

$$ a_n = \frac{a_{n-2}}{n(n-1)} $$


Given the initial condition \( a_0 = 1 \) and \( a_1 = 0 \), the series solution is:

$$y(x) = \sum_{n=0}^{\infty} x^n = \frac{1}{1-x}$$

Thus,
$$ y(x) = \frac{1}{1-x} $$



### Problem 22:
**Given:**
$$ ((1 - x^2) y')' = -\alpha (\alpha + 1)y $$

We recognize this as the Legendre differential equation:
$$ (1 - x^2)y'' - 2xy' + \alpha(\alpha + 1)y = 0 $$

**Solution:**

We express the Legendre polynomial \( P_n(x) \) as:
$$ P_n(x) = \frac{1}{2^n n!} \frac{d^n}{dx^n}[(x^2 - 1)^n] $$

which simplifies to:
$$ ((1 - x^2) y')' = \sum_{n=0}^{\infty} \frac{(-1)^n (\alpha + n)!}{n!(\alpha + 2n + 1)} x^n $$

This equation suggests that \( y(x) \) satisfies the Legendre polynomial relation:
$$ P_n(x) = \frac{1}{2^n n!} \frac{d^n}{dx^n} [(x^2 - 1)^n] $$

### Problem 23:
**Given:**
$$ f(x) = \sum_{k=0}^{n} a_k P_k(x) $$

**Solution:**

The coefficients \( a_k \) are found using the orthogonality property of the Legendre polynomials:

$$ \int_{-1}^{1} P_m(x)P_n(x)dx = 0 \quad \text{for } m \neq n $$
This gives:
$$ a_k = \frac{2k + 1}{2} \int_{-1}^{1} f(x)P_k(x)dx $$

This is derived from the fact that:
$$ f(x) = \sum_{k=0}^{n} a_k P_k(x) $$
and using the orthogonality:
$$ a_k = \frac{2k + 1}{2} \int_{-1}^{1} f(x)P_k(x)dx $$

