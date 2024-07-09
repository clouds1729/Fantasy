## Substitutions
The simplest type is called **scaling**.   

$y_1 = \frac{y}{a}$ ,  $x_1 = \frac{x}{b}$ ,  where $a$ and $b$ are constants.

--------------------------------------------------------------------------
### Why do this?

- Change Units

- Make the variables Dimensionless

- Reduce the number of constants(or simplify the constants).
		
	Example:
	 Newton's Temperature Law: $\frac{dT}{dt}= k(M^{4}- T^4)$
		M = External Temperature(assumed to be constant)
		T = Internal Temperature

Notice you can solve this equation just as it stands, but you can also scale. $T_{1}= T/M$ , such that $T_1$ is dimensionless(3). To substitute, we write $T = M \cdot T_1$ .

It then becomes:
$$M \cdot \frac{dT_1}{dt}= kM^{4}(1 - T_{1}^4)$$

$T_1$ is dimensionless.  $k_1$ has units $time^{-1}$
$$M \cdot \frac{dT_1}{dt}= k_1(1 - T_{1}^4)$$ where $k_{1}= k M^4$

	One less constant is called "Lumping" Constants 💀💀💀


--------------------------------------------------------------------------
### Types of Substitution

- Direct:
		new variable = a 
		combination of old variables. Example: 
		
		$T_{1}= \frac{T}{M}$

- Inverse:
		old variable = new + *old variables*. Example: $T = M \cdot T_1$

$\int x \sqrt{1 - x^{2}}dx$  calls for a direct substitution: $u = 1-x^2$. $\int  \sqrt{1 - x^{2}}dx$ requires an indirect substitution: $x = \sin(u)$ .	 

#### Examples of Substitutions

- Direct Substitution:
	Applies to an equation of the form: $y' = p(x)y + q(x)y^n$ $[n \neq 0]$ . This equation is called the **Bernoulli equation**.

The main idea is to divide through by $y^n$.
Generalization:
	$\frac{y'}{y^n} = p(x) \cdot \frac{1}{y^{n-1}} + q(x)$
	$v = \frac{1}{y^{n-1}} = y^{1-n}$
	$v' = (1-n) \frac{1}{y^{n}}\cdot y'$
	$\frac{v'}{1-n} = p(x)v + q(x)$

Example 1:
	$y- xy' =y^2$
	$1/y - \frac{xy'}{y^{2}} = 1$
	$\frac{y'}{y^{2}} = \frac{1}{xy}-1$
	Let $v = \frac{1}{y}$, $v' = \frac{-1}{y^{2}}y'$
	$-v' = \frac{v}{x} -1$ 
	$v' + \frac{v}{x} = 1$
	$xv' + v = x$
	$(xv)'=x$
	$(xv) = \int x dx$
	$xv = \frac{x^2}{2}+ c$
	$v = \frac{x}{2}+ \frac{c}{x} = \frac{x^{2}+ 2c}{2x}$ 
	$\implies$ $y = \frac{2x}{x^{2}+c_{1}}$ 

--------------------------------------------------------------------------
- Inverse Substitutions
	Homogeneous ODE's
	Form:  $y' = F\left(\frac{y}{x}\right)$
	Example: $y' = \frac{x^{2}y}{x^{3}+y^{3}} = \frac{y/x}{1+(\frac{y}{x})^3}$
	Example: $y' = \sqrt{x^{2}+ y^{2}}= \sqrt{1 + (\frac{y}{x})^2}$
- Homogenous equations are invariant under "zoom".😑 
		Def(zoom): $x \to ax_1$ and $y \to ay_1$ where a is the same for both scaling of $y$ and $x$. First:
		$\frac{y}{x}= \frac{y_1}{x_{1}}$ , since both were scaled equally.
		$dx = a dx_1$ and $y = ady_1$ $\frac{dy}{dx} = \frac{adx_1}{ady_{1}} = F(y_1/x_1)$

- Example 1:
	$y' = F(\frac{y}{x})$ and let $z  = \frac{y}{x}$. Then, $y = xz$.
	$y' = z + xz'$
	$z + xz' = F(z)$
	$x \frac{dz}{dx} = F(z) - z$
	- Separate variables to solve

- Example 2:
	Drug boat escapes from lighthouse beam at $45^\theta$ . What is the boat's path?
	- What do we know?
		- The boat's path is a curve, which can be represented with an unknown function.
		- The slope of the boat's path makes a $45^\theta$ with the lighthouse beam. So the slope makes a known angle with a known angle. 😀

	$y' = \tan(\alpha + 45^\theta)$ and $\tan(\alpha) = \frac{y}{x}$
	$y' = \tan(\alpha + 45^{\theta)}= \frac{\tan(\alpha + \tan(45^{\theta}))}{1-\tan(\alpha)\tan(45^\theta)}$
	$y' = \frac{\left( \frac{y}{x} \right) + 1}{1-\frac{y}{x}} = \frac{y+x}{x-y}$
	$z = \frac{y}{x}$ . Then, $y' = z'x + z$
	$y' = z'x + z = \frac{\left( z \right) + 1}{1-z}$
	$x\frac{dz}{dx} = \frac{\left( z \right) + 1}{1-z} -z = \frac{z^{2}+ 1}{1-z}$
	$\frac{1-z}{z^{2}+1}dz = \frac{1}{x}dx$
	$\arctan(z) - \frac{1}{2} \ln(z^{2}+ 1) = \ln(x) + c$ 
	$\arctan(z) = \ln(x\sqrt{z^{2}+ 1}) + c$
	$\arctan\left( \frac{y}{x} \right) = \ln(\sqrt{ x^{2}+ y^{2}}) + c$
	$\implies \theta = \ln (r) +c$
	$\implies r = c_{1} e^\theta$
