## Lecture 1
### Overview:

#### Differences between complex analysis and real analysis.

So the first one is that trigonometric functions and excellent functions turn out to stay. And so there's a very famous identity due to Euler that says that $e^{ix} = \cos(x) + i\sin(x)$. And using this, we can write all trigonometric functions in terms of exponential functions, for example.

Cosine of $X$ is equal to $E$ to the $9$ plus $\eta -9 / 2$ and this saves a lot of labour because all the complicated identities for trigonometric functions that no one can ever really remember automatically. Special cases of identities for exponential function, so there's a lot less to remember.

So the second difference is, suppose you've got a real function.

So suppose we've got a function that looks like this. Suppose it might be 0 for $X < 0$, and it might be $y = X^2$.

For $X < 0$, now we can take the derivative of this function.

And its derivative is still 0 down here, and its linear up here, and it's not differentiable here.

So there are some functions we can differentiate once and some we can differentiate twice and some we can differentiate three times and so on. For complex analysis, there's no analogue of this. So for complex functions.

So this would take the complex numbers to the complex numbers. So if it's differentiable once, it's automatically.

Differentiable twice. And if it's differentiable twice, you can apply the same argument to show it's differentiable three times and so on, so you can differentiate it any number of times. And this is really bizarre if you're used to real analysis. You seem to be getting something for free that somehow just insisting a function as differential once. There doesn't seem to be any obvious reason why it should be differentiable twice.

So, you know, it's a sort of example of you say you can't get a free lunch or sometimes in complex analysis you can get things for free.

So differentiation behaves better for complex, functions. Now, let's look a bit about integration. So.

Suppose we want to integrate $\int_{0}^{1} F(x) \, dx$. Now if you're integrating real numbers.

We're integrating from zero to one, and there's only one way to go from zero to 1, just go along like that. So let's kill what this interval is meant. On the other hand, if we're integrating in the complex plane, so here is one and here is $I$ from zero to one, there seem to be a lot of different ways you would go from zero to 1. So we could either go along like that or we could go like that, or we could go like that and so on.

So the integral from zero to one seems to depend on which path you take.

But it turns out that it almost doesn't. So we have Cauchy's theorem, which is one of the central theorems of convex analysis. So the integral from zero to one of $F(x) \, dx$ is almost.

Independent.

Of the path we take from zero to one. Actually there are some cases when it does depend on the path that we'll discuss this later. So this applies to the functions $F$ that are differentiable. It certainly doesn't apply to all complex functions.

So this saves an awful lot of trouble because we don't have to specify the path of integration, or at least.

Well adopted the minor problem that we will discuss later.

And this turns out to be incredibly useful because in real analysis there are various integrals like the integral from zero to Infinity of $\frac{\sin(x)}{x} \, dx$, and various sums such as $\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2}$, and so on, which you don't learn how to evaluate in ordinary introductory capitalist courses.

In fact, $\frac{\sin x}{x}$ is one of these functions where you can't write down an explicit elementary formula for the interval, so.

Integral from zero to $X$ of $\frac{\sin x}{x} \,dx$ just can't be written explicitly in terms of elementary functions. However, it turns out you can evaluate the integral to Infinity. It turns out to be $\frac{\pi}{2}$. And again, you don't learn how to evaluate something like this in most introductory analysis courses and most techniques you learn just don't work. This turns out to be $\frac{\pi^2}{6}$.

And we're going to see how to work out both of these.

Using complex integration.

And this may be a little bit surprising because neither of these this integral and this sum don't have anything to do with complex numbers at first sight. But it turns out that complex integration gives a way to evaluate series and sums like that.

Next we have the phenomenon of analytic continuation.

So suppose.

I give you a function.

When considering a function defined on the interval $[0,1]$, and provided it is a real differential function, the function can be described as being 0 up to $\frac{1}{2}$ and then transforming into a parabola from $\frac{1}{2}$ to 1. Given this context, when asked to calculate its value at point -1, it is outside the domain of definition of the function as specified by the interval $[0,1]$. Therefore, the function's value at point -1 is not defined within the given constraints.

This is a completely stupid question because if I tell you the function between zero and one, there's just no way you can evaluate -1 I mean, it's you can guess maybe it continues to 0, or maybe it continues.

Like that or whatever, we just have no real information about its value of -1. However, for complex functions, if I give you a function on the interval from zero to one and it's differentiable.

Umm, it's automatically determined in any connected region, so a function.

One say naughty one is determined.

Uniquely.

On any larger open connected set.

And that's provided the function is complex differentiable function.

And again, we seem to be getting something for nothing and only telling you a function on say the interval 0 to one or some small region, and somehow this magically determines it on on a much larger region. So there's a very famous or possibly notorious example of this which is the Riemann.

Zeta function.

The notation for Zeta of $S$ is $\zeta(S) = \frac{1}{1^s} + \frac{1}{2^s} + \frac{1}{3^s} + \ldots$. So, for example, $\zeta(2) = \frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \ldots + \frac{\pi^2}{6}$ as we will see later.

And this is possibly the single most notorious function in mathematics.

Particularly because of the Riemann Hypothesis.

Which says all zeros.

Of theater of $S$ are either real or have real parts.

So let's draw a picture of this. So here's the complex plane, and here's the .0, and here's the .1. And here's the point I. And the Riemann Zeta function has all its zeros, but it's got a few zeros at -2 and -4, so that we won't worry about. But there's the so-called critical line.

Which has a real part of heart and imaginary part. Then the claim is that all zeros of the Riemann Zeta function lie on this pink line apart from the ones that. Well, the problem is the Riemann hypothesis makes no sense at all because if we try and evaluate this, this only converges.



## Lecture 2


This lecture is part of an introductory undergraduate course on complex analysis and will be about complex arithmetic.

So I'm going to spend the first three or four lectures of this course just covering basic stuff like arithmetic and trig functions and so on, before we get to the interesting stuff about complex analysis. So first of all, we recall what a complex number is.

Well, if you're a computer, the complex number is an ordered pair of real numbers. So this is for computers. If you're a human, you write a complex number as $x + iy$ for a reason become rather obvious moment. So this is for humans.

And writing it as an ordered pair XY is actually quite good for human too, because this means you can identify complex numbers with the plane. You can just use X&Y as plane coordinates. So you can represent each complex number as a point on the plane in the much the same way you represent each real member as a point on the line. Now we need to define addition and subtraction and multiplication, and we'll do division a little bit later, so addition is completely obvious.

Addition is just the same As for addition of vectors in the planes of $A + IB$ times $C + ID$ is just rather obviously given by $A + C + I \times (B + D)$.

Multiplication is a little bit less obvious. If you write numbers as ordered pairs, then the rule for multiplication is given like this. 

$$AB \times CD = AC - BD.$$

An $AD + BC$. And this looks completely mysterious. You know, you think, where on earth does this formula come from? And you can't possibly remember it. But if you write the numbers as $A + iB \times C + iD$, then it's much more obvious because you multiply the surface $AC + i^2 BD + iBC + iAD$. And now we use the fact that $i^2$ is by definition $\sqrt{-1}$.

AC minus BD plus I times BC plus AD. So that's why we write numbers in this form rather than this one. It makes the multiplication of complex numbers trivial to remember.

Now what we really ought to do is to check with these satisfy.

The usual rules of algebra.

So for example, we might want to check that $A * B + C$ is equal to $AB$ plus $AC$ and $AB$ times $C$ is equal to $A$ times $BC$ and so on. And there are several ways to do this. One, we can do a long, somewhat tedious check, which we're not going to bother because it's somewhat long and tedious. Secondly, you can go to an abstract algebra course.

And in an abstract algebra course, you find that this definition of the complex numbers, which is often written as AC for complex numbers.

Can we define you take the ring of polynomials over the reels polynomials in a variable $I$ and you quotient that by the ideal generated by $I^2 + 1$ and this gives a ring with this additional multiplication. And there are general theorems in abstract algebra about quoting out by these sorts of ideas, which means this is automatically a ring. So if you go through an abstract algorithm, of course you don't have to bother doing this long check.

So.

But the one thing I haven't yet mentioned is division.

And this is a little bit less obvious, so we want to check that $A + iB$ has an inverse.

If it is not equal to 0, which of course stands for $0 + 0i$.

And to do this, we're going to use complex conjugation.

So complex conjugation takes $X + iY$ to $X - iY$ and.

It's denoted by putting a bar over $X + iY$, so, so so. This overline means complex conjugation, and the reason this turns up a lot is which said $i^2 = -1$.

But $-1$ actually is $2 \sqrt{2}$, because $(-i)^2$ is also equal to $-1$. So when we talk about $\sqrt{-1}$, we don't really know which square root, and in fact these two square roots are completely equivalent.

Yeah. And anything you can say about one square root, you can say about the other square root. So you can sort of flip from one square root to the other without really changing anything. So complex conjugation actually preserves all properties of the complex numbers. So for example, if we've got complex numbers $Z_1$ and $Z_2$ and we take their complex conjugate, this is equal to $\overline{Z_1} \times \overline{Z_2}$, $\overline{Z_1 + Z_2} = \overline{Z_1} + \overline{Z_2}$.

In fact.

Complex conjugation $C \to \bar{Z}$ is an automorphism.

Both of the complex numbers. This just means it's a map from the complex numbers to itself. That's a bijection. Preserves all the structure you can think of. If you've done a Galois theory course, another way of saying this is the Galois group.

Of the complex numbers over the reels, it has two elements which are one and complex conjugation.

So anyway, using complex conjugation.

We can find the inverse of any similar complex number as follows. First of all.

We notice the difficult $Z$ was $X + iY$. Then $Z$ times its complex conjugate is real because $X + iY$ and $X - iY$ is $X^2 + Y^2$ and division by real numbers is easy. So we want to $\frac{1}{Z}$. Well, we don't really know how to divide by by a complex number $Z$ yet, but we can multiply the top and bottom by the complex conjugate.

And now this division is easy because because this bit here is now real. So let's carry this out. We have $\frac{1}{X + IY}$ or this is $\frac{X - IY}{X + IY}$, which is equal to $\frac{X - IY}{X^2 + Y^2}$ which is equal to $\frac{X}{X^2 + Y^2} -$.

$IY over X ^2 + y ^2$ so.

$IY over X ^2 + y ^2$ so.

This is a formula for the inverse of the complex number $X + iY$. And of course, you shouldn't waste time remembering this formula. What you should do is remember this trick of multiplying the numerator and denominator by the complex conjugate of the denominator. For example, let's just work out $\frac{1 + 2i}{3 + 4i}$. Well, as we said, we multiply the top and the bottom by the complex conjugate of this, so we get $1 + 2i$.

$I + 3 - 4I \div (3 + 4I)$

3 - 4 five, and now we can multiply out the top and we get $11 + 2i$. Now we multiply at the bottom and we get $3^2 + 4^2$, which is 25. So this is $\frac{11}{25} + \frac{2}{25}i$. So division of complex numbers is also reasonably easy.

By the way, I should put in an awful warning here that there's a Greek letter $\zeta$.

Which kind of looks like this. And you must never use zai as the name of a complex variable, because if you do, you might end up having to take $\Psi$ divided by the complex conjugate of the sine. If you write this out, where we've got $\Psi$ divided by the complex conjugate of $\Psi$, which means the price for the most important mathematical notation of all time. Another useful property of complex numbers is the absolute value.

So for a real number $X$ we know the absolute value of $X$ is equal to $X$ for $X > 0$.

$$f(x) = \left\{
\begin{array}{ll}
-x & \text{for } x < 0 \\
\text{distance} & \text{otherwise}
\end{array}
\right.$$

Of $X$ from zero, and we're going to define the absolute value of a complex number in the same way, so $Z$ is going to be the distance.

Of $Z$ from zero. That's easy to work out. So $Z$ is equal to $X + iY$. And we're talking about the distance of $Z$ from zero when we represent numbers as the plane. So we want to know the distance from the point $(X,Y)$.

To zero, and we know what this is. By Pythagoras it's just $\sqrt{x^2 + y^2}$. And now we notice that this turned up when we were doing complex conjugate. So this is just $\sqrt{z \cdot \bar{z}}$.

And now we see that the absolute value of $C_1Z_2$ is equal to the absolute value of $Z_1$ times the absolute value of $Z_2$ using because it is equal to this, and that obviously preserves that formula.

And we also get all the rules of absolute value. For instance the absolute value of $Z_1 - C_2$ is less than or equal to the absolute value of $C_1$ plus the absolute value of $C_2$ because this just says the distance from $Z_1$ to $Z_2$.

Is at most the distance from $Z_1$ to $0$ plus the distance from $Z_2$ to $0$, which is obviously what $Z_1$ here and $Z_2$ here. Then this distance here is the active value of $Z_1$, this distance here is the absolute value of $Z_2$, and this distance here is the absolute value of $Z_1 - Z_2$. So most of the usual rules you're used to absolute values of reels will also work with absolute values of complex numbers.

If you've done metric spaces, you can make the complex numbers into a metric space in the obvious way. You just define the distance from $Z_1$ to $Z_2$ to be the absolute value of $Z_1 - Z_2$, and this is just the same as the usual distance in the plane.

So now let's see some applications of this.

So let's first have an application to the following problem, which integers.

Are sums or two squares?

So this is a very old problem in number theory and.

It's quite complicated to work out the arts. We're not going to work out a complete answer, but what we notice is the integers that are sums of two squares close.

Under multiplication. In other words, if you've got two integers which are sums of two squares, then so is their product. And the proof of this is as follows. Suppose we've got one integer which is the sum of 2 squares. We multiply it by another integer, which is the sum of 2 squares. Well, we can write this as a sum of two squares because it's $(AC - BD)^2 + (AD + BC)^2$.

Squared. Well, that's a very neat proof that.

Where on earth does this formula come from? Well, it comes from complex numbers. So we notice that $a^2 + b^2$ is equal to $\lvert A + iB \rvert^2$. And of course $c^2 + d^2$ is equal to $\lvert C + iD \rvert^2$. So $a^2 + b^2 * c^2 + d^2$ is equal to the absolute value of $a + iB$.

And $C^2i^2$ and we now just multiply this at $0AC-BD+i$ times.

$AB + BC$

$4 ^2$ and now.

$X + iY$ squared is just $X^2 + Y^2 = AC - BD)^2 + (AD + BC)^2$. So complex numbers help to explain this formula. I mean, of course, you don't need complex numbers to prove this form, you could just write it down. You can easily check it by multiplying it out. But.

That that proof doesn't really explain why this formula exists. And this exists because of complex numbers.

So let's just give an example of this. So we have $5 = 1^2 + 2^2$ and $13 = 2^2 + 3^2$. And we notice that $5 \times 13 = 65$, which is equal to $8^2 + 1^2$. Well, it's also equal to $4^2 + 7^2$. So why are there two ways to write $65$ as a sum of two squares? Well, let's take a look.

This corresponds to.

Taking $1 + 2i$. So we notice the absolute value of $1 + 2i$ squared is equal to five and this comes from looking at $2 + 3i$. So the absolute value of this squared is $13$. So what we should do is multiply $1 + 2$.

I $*$ 2 + 3 I and this gives us 2 - 6 which is equal to -4.

And plus seven $I$. So here we get the $4^2 + 7^2$ or rather $-4^2 + 7^2$. But who cares? But there's another thing you can do because you can change this to its complex conjugate. We can take $1 + 2I$ and $2 - 3I$. And this, this is now slightly different because we get this is input $8$.

Plus I and this one is giving you the other way of representing 65 as a sum of 2 squares.

Of course, there are other things we could do. We could change this to $1 - i$, $2i$, or we've used $2 - i$ or something. But these would just give variations on these two formulas. We get things like $8^2 + (-1)^2$ and so on. So you see the two ways of writing $65$ as a sum of two squares correspond to these two different products of complex
numbers.

So next application, let's take a look at Pythagoras theorem $a^2 + b^2 = c^2$.

And we want to be able to find solutions to this. For example, everybody knows $3^2 + 4^2 = 5^2$ or $5^2 + 12^2 = 13^2$ and so on. And the question is how can we generate lots of solutions to this easily?

Well, let's suppose that $A + BI = X + IY^2$ with some $X\&Y$. Then $a^2 + b^2$ is equal to.

$|\text{X} + i\text{Y}|$

Squared all squared.

So, it's equal to $x^2 + y^{2^2}$. And here we've got a distribution of $a^2 + b^2 = \text{something}^2$. So let's just try this. Let's try $x + iy = 2 + i$.

$2 + i^2 = 3 + 4i$ and $|2 + i|^2 = 5$, which gives us a solution $3^2 + 4^2 = 5^2$ if we try.

$2 + 3i$ This is equal to.

Square of this is equal to $a - \sqrt{b} + 12i$ and we see that $5^2 + 12^2$.

Is equal to $2^2 + 3^{2^2}$ which is equals $13^2$. So you can just choose more or less any random complex number with integer coordinates and square it and that will give you a solution of Pythagoras equation.

Well, after people discovered you could extend the real numbers, the complex numbers, that there were quite a number of attempts to extend the complex numbers to something even bigger by adding.

Further variables may be the square root of something else and people try to, you know, the complex numbers are two-dimensional. So people, several people try to find a three-dimensional version of the complex numbers and no one came up with anything very convincing. Hamilton.

Found four-dimensional version of the complex numbers called the quaternion.

So.

So complex numbers are written as $A + Bi$.

And the quaternions, the four variables, they're $A + BI + CJ + DK$. So these are the quaternions.

Quaternions means a collection of four things.

And you need to know what is, what are the problems of these? So the complex numbers you just need $i^2 = -1$, the quaternions $i^2 = -1$.

$J^2 = -1$ and $K^2 = -1$. Well, you also need to know how to multiply $I$ and $J$. Well $IJ = K$ and you might think that means $JI = K$. But no, this is even $-J \cdot I$ and $JK = I$ which is equal to $-KJ$ and $KI = J - IK$. So.

There's a minus sign there, so the.

And quaternions are not commutative.


