## Autonomous Differential Equations

These have no independent variable on the RHS. It's a function of $y$ alone(**the dependent variable**).
General Form: $\frac{dy}{dt} = f(y) \gets$ no t on RHS.

Big deal! If there's no $t$ on the RHS then we can solve these by separating variables. So why are we discussing this. 🤕🤕

--------------------------------------------------------------------------
## Motivation
-  We may not be able to do integration required in the separation of variables to get an explicit solutions.
- We may not even need to solve the ODE to get certain types of information about it.

*PROBLEM*: Get qualitative information about the solution without actually solving the equations.

--------------------------------------------------------------------------
### How do the Direction Fields look like?

- Every horizontal line on the $ty$-plane is an isocline(Why?).
	Along any horizontal line the slope of the line elements are $\frac{dy}{dt} = f(y,0)$.  

- The integral curves are invariant under translation and hence you can get all of them by translating one integral curve along the x-axis

*Definition*:
	Critical Point: $y_0$ is a critical point if $f(y_{0)}= 0$
	For these types of ODE's $y'=y_{0}$ is a solutions
	*Proof*: Solution at constant function, $y_{0}$ , is $\frac{dy_{0}}{dt} =f(y_{0})$. Both sides are $0$.

Note that, other integral curves can't cross the solutions $y_{0}$. Will show these through examples later.

*General Process*:
	- Find the critical points by solving $f(y_{0}) = 0$
	- Graph $f(y)$. 
	- Check for where $f(y)$ > 0 , $f(y)$ < 0.  


Example 1:
	- $y$ = Money in the Bank Account
	- $r$ = (cont.) interest rate
	- $\frac{dy}{dt}$ = $ry$

Suppose your money is being embezzled from your account. Let $w$ be the rate of embezzlement.

$$\frac{dy}{dt} = ry - w$$

Notice we can subtract $w$ because $w$ is the time rate of embezzlement. The embezzler is stealing a certain fraction of the account, rather a certain amount of dollars.

Let's analyze the behavior of the solutions without solving by separating variables. Following the general process. 

We have:

- Critical Points
	$ry - w = 0$ $\implies$ $y = \frac{w}{r}$

- Plot $f(y)$
	Note that $f\left( \frac{w}{r} \right) = 0$.
	Plot on $f(y)y$ - plane
	$ry - w$ has intercepts on the plane above


--------------------------------------------------------------------------
### Logistic Equation

Describes population behavior $y(t)$ in the book. The basic population equation is:

$$\frac{dy}{dt} = ky$$

$k$ = growth rate, technically *net birth rate*. $k$ = birth rate - death rate 💀. If k is constant, it's called *simple* growth.

Logistical growth implies $k$ being constant is unrealistic! The growth rate declines as $y$ increases because resources decline. We can replace $k$ be a function that decreases as $y$ increases(Any ideas?).

*Simplest choice*: $k = a - by$ : simple linear and decreasing function.

Thus, 

$$\frac{dy}{dt} = ay -by^2$$


The explicit solutions(via separation of variables) involves *partial fractions*.

- Critical Points
	$y(a - by) = 0$, $y = 0$ and $y = \frac{a}{b}$

*Intuition*: If the population starts at 0 it will stay at 0, likewise if it starts at $\frac{a}{b}$. What happens in between?🤔

- Graph
	On $f(y) y$ - plane the intercepts will be at $0$ and $\frac{a}{b}$ for $f(y) = 0$
	The function will be a downward opening parabola(as $y \to \infty$, $\frac{dy}{dt} \ll 0$).
	The integral curves increase asymptotically between $\frac{a}{b}$ and $0$ to $\frac{a}{b}$ and decrease outside the two bounds (decrease to $\frac{a}{b}$ and decrease away from $0$).
Thus, $\frac{a}{b}$ is called the *stable* critical point/solution and $0$ is called the unstable *unstable* critical point(arrows point away from the point). 

Note: There are also *semi stable* critical points(the graph on $f(y)  y$ - plane is tangent to the the y axis and above $f(y) = 0$).

--------------------------------------------------------------------------
### Logistical Equation With Harvesting

Harvesting: at a constant time rate $$\frac{dy}{dy} = ay - by^{2}-h$$
$h$ is a term to take care of the constant harvesting rate.