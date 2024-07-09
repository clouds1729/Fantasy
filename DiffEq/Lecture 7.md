## Linear First Order
General Form: $y' + ky = q(t)$

Solve: $y' + ky = q(t)$

$\implies y = e^{-kt} \int q(t)e^{kt} dt + ce^{-kt}$

As $t \to \infty$ , $e^{-kt} \int q(t)e^{kt} dt$ is called the *steady-state* or long term solution because it stays as a function(doesn't "disappear"). But, $ce^{-kt}$  disappears no matter the value of $c$. This implies that all the other solutions approach the steady state solution. It's called the *transient*.

The *transient* uses the initial condition, usually $y(0)$.


Input: $q(t)$ - RHS of the differential equation.

Response / Output: $y(t)$ is the solution to the differential equation



--------------------------------------------------------------------------
## Detailed Explanation

$\textbf{First Order Linear Equation}$
$$y'(x)+a(x)y(x)=f(x)$$
$\begin{aligned}\text{Multiply both sides by the }integrating~factor~I(x):=e^{\int a(x)\mathrm{~d}x},~\text{which satis-}\end{aligned}$
$\operatorname*{fies}I^{\prime}(x)=a(x)I(x).$ Hence $(Iy)^\prime=Iy^{\prime}+aIy=If$, so integrating gives
$$y(x)=I(x)^{-1}\int^xI(s)f(s)\:\mathrm{d}s+AI(x)^{-1}.$$
Example. $y'=x+2y.$ The integrating factor is $I(x)=e^\int-2=e^{-2x}$,
$$\begin{aligned}(e^{-2x}y)'&=e^{-2x}(y'-2y)=xe^{-2x}\\\Rightarrow\:e^{-2x}y&=\int xe^{-2x}\:\mathrm{d}x=-\frac12xe^{-2x}-\frac14e^{-2x}+c\\\Rightarrow\:y(x)&=ce^{2x}-\frac12(x+\frac12)\end{aligned}$$
--------------------------------------------------------------------------
### Some Relevant Theorems

The Superposition Principle and Undetermined Coefficients Revisited

#### Theorem  (Superposition Principle). 

If $y_1\textit{ is }a\textit{ solution to the equation}$
$$ay''+by'+cy=f_1(t),$$
and $y_2$ $is$ $a$ solution $to$
$$ay^{\prime\prime}+by^{\prime}+cy=f_2(t),$$
then for any constants $k_{1}$ and $k_{2}$, the function $k_{1}y_{1}+k_{2}y_{2}$ is a solution to the differential equation.
$$ay''+by'+cy=k_1f_1(t)+k_2f_2(t).$$
$Proof.$
$$\begin{aligned}ay''+by'+cy&=a(k_1y_1+k_2y_2)''+b(k_1y_1+k_2y_2)'+c(k_1y_1+k_2y_2)\\&=k_1(ay_1''+by_1'+cy_1)+k_2(ay_2''+by_2'+cy_2)\\&=k_1f_1(t)+k_2f_2(t).\end{aligned}$$

--------------------------------------------------------------------------


