## Linear First Order
General Form: $y' + ky = q(t)$

Solve: $y' + ky = q(t)$

$\implies y = e^{-kt} \int q(t)e^{kt} dt + ce^{-kt}$

As $t \to \infty$ , $e^{-kt} \int q(t)e^{kt} dt$ is called the *steady-state* or long term solution because it stays as a function(doesn't "disappear"). But, $ce^{-kt}$  disappears no matter the value of $c$. This implies that all the other solutions approach the steady state solution. It's called the *transient*.

The *transient* uses the initial condition, usually $y(0)$.


Input: $q(t)$ - RHS of the differential equation. 
*Intuition*: Think of the temperature model. External temperature drives the change in internal temperature.


Response / Output: $y(t)$ is the solution to the differential equation


#### Special Form

$$y' + ky = kq_{}{e} (t)$$
*Hint*: To solve you first divide through by k.



### Superposition Of Inputs

If the input $q_{1}(t) \to y_{1} (t)$ and $q_{2}(t) \to y_{2} (t)$  , then 

$$q_{1}(t) + q_{2}(t) \to y_{1} (t) + y_{2} (t)$$

and
$$c q_{1} \to c y_{1}$$

Uses the *LINEARITY* of the ODE. If there's a term $y^n$  for $n > 1$, then this doesn't apply.


What happens if the inputs are trigonometric?🤔

### Fourier Series

Consider

$y' + ky = kq_{e} (t)$

$y' + ky = k \cos( \omega t)$                       

$\omega =$  number of complete oscillations in the interval $2 \pi$ = angular frequency

For the physical input $q_{e} (t) = \cos( \omega t)$, find the response

Idea: complexify the problem

We use the fact that $e^{i (\omega t)} = \cos( \omega t) + i \sin (\omega t)$

$y' + ky = k e^{(i \omega t)}$                       

$y$ is the real function that solves the problem so we need to change $y$

$\tilde{y'} + k \tilde{y} = k e^{(i \omega t)}$                    

where $\tilde{y} = y_{1} + i y_{2}$                             (complex solution) 

Why that sum?

Find $\tilde{y}$ then $y_{1}$ will solve the original ODE.


Thus, we have,

$(\tilde{y}e^{kt})' = k e^{(k + i \omega )t}$

$\tilde{y}e^{kt} = \frac{k}{ k + i \omega } e^{(k + i \omega )t}$

Two ways to solve:
- Polar Form
- Cartesian Form

We resort to polar form:

$\tilde{y} = \frac{1}{ 1 + i (\frac{\omega}{k}) } e^{(i \omega )t}$


Reminder: $\alpha$ complex

$\frac{1}{\alpha} \cdot \alpha = 1$

$\frac{1}{|\alpha|}  = |\alpha|$

$arg\left(\frac{1}{\alpha}\right)+ arg(\alpha) = 0$

$arg\left( \frac{1}{\alpha} \right) = - arg(\alpha)$

Polar Form:

$\frac{1}{1 + i\left( \frac{\omega}{k} \right)} = \frac{1}{\sqrt{ 1 + (\left( \frac{\omega}{k} \right)^2 }} e^{- i \phi}$ 


$\tilde{y} = \frac{1}{\sqrt{ 1 + (\left( \frac{\omega}{k} \right)^{2 }}} e^{i(wt-  \phi)}$

Thus,

$y_{1} =\frac{1}{\sqrt{ 1 + (\left( \frac{\omega}{k} \right)^{2 }}} \cdot \cos(\omega t - \phi)$

where $\phi = \tan^{-1}\left( \frac{w}{k} \right)$ which is called the *phase lag* of the function.


--------------------------------------------------------------------------
## Detailed Explanation

$\textbf{First Order Linear Equation}$
$$y'(x)+a(x)y(x)=f(x)$$
$\text{Multiply both sides by the }integrating~factor~I(x):=e^{\int a(x)\mathrm{~d}x},~\text{which satisfies}$
$I^{\prime}(x)=a(x)I(x).$ Hence $(Iy)^\prime=Iy^{\prime}+aIy=If$, so integrating gives
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



