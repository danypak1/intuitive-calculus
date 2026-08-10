# Unit 23: Antiderivatives

## 1. The idea, in plain words

Every skill so far has gone one direction: start with a function, find its derivative. **This unit runs the movie backward.** Given a derivative, can you figure out what function it came from? That "undoing" process is called finding an **antiderivative**.

**Picture it like this:** if differentiation is "what's my speed, given my position?", antiderivatives ask the reverse question: "given my speed the whole time, what was my position?" You already have great intuition for this from Unit 11 — position, velocity, and acceleration are all connected by derivatives, so they must also be connected by *antiderivatives*, just read in the opposite direction.

**Here's the catch that makes antiderivatives a little different from derivatives: they're never unique.** The derivative of $x^2$ is $2x$ — but so is the derivative of $x^2+5$, or $x^2-100$, or $x^2$ plus *any* constant, since a constant's derivative is always $0$. So when you're asked to find "the" antiderivative of $2x$, the honest answer is a whole family of functions: $x^2+C$, where $C$ can be *any* constant. We always tack on that mystery constant, written $+C$, to represent every possible antiderivative at once.

**If you're given extra information** — like the function's value at one specific point — you can pin down exactly which member of that family you want, by solving for the specific value of $C$ that makes it fit.

## 2. Toolbox

**Notation:** the antiderivative of $f(x)$ is written $\displaystyle\int f(x)\,dx$, and read "the indefinite integral of $f$." If $F'(x)=f(x)$, then:
$$\int f(x)\,dx = F(x)+C$$

**Power Rule for antiderivatives** (the reverse of the power rule for derivatives): bump the exponent up by one, then divide by the new exponent.
$$\int x^n\,dx = \frac{x^{n+1}}{n+1}+C \qquad (\text{for } n \ne -1)$$

*(The case $n=-1$, i.e., $\int\frac{1}{x}dx$, needs a special function — natural logarithms — which we haven't covered yet. We'll come back to it in a later unit.)*

**Constant Multiple and Sum Rules** (same as for derivatives):
$$\int c\cdot f(x)\,dx = c\int f(x)\,dx \qquad \int\big[f(x)\pm g(x)\big]\,dx = \int f(x)\,dx \pm \int g(x)\,dx$$

**Basic trig antiderivatives:**
$$\int \sin x\,dx = -\cos x + C \qquad \int \cos x\,dx = \sin x + C$$
$$\int \sec^2x\,dx = \tan x + C \qquad \int \csc^2x\,dx = -\cot x + C$$
$$\int \sec x\tan x\,dx = \sec x + C \qquad \int \csc x\cot x\,dx = -\csc x + C$$

**Solving for $C$ using extra information (an "initial condition"):** find the general antiderivative first (with $+C$ still attached), then plug in the given point to solve for the exact value of $C$.

**Chaining antiderivatives together (for motion problems):** since $a(t)=v'(t)$ and $v(t)=s'(t)$, you can work backward: antidifferentiate acceleration to get velocity (using $v(0)$ to solve for the constant), then antidifferentiate that velocity to get position (using $s(0)$ to solve for the next constant).

## 3. Common mistakes

- **Forgetting the $+C$.** This is the single most common error in this entire unit — every single indefinite integral needs it, even if the problem seems simple.
- **Sign errors with $\sin x$ and $\cos x$.** Remember the antiderivative of $\sin x$ is $-\cos x$ (with a negative sign) — it's easy to drop that minus sign, especially since the *derivative* rules go the opposite direction.
- **Applying the power rule to $x^{-1}$.** This case is special (it needs natural logs, covered later) — don't try to force the regular power rule formula onto it, since dividing by $n+1=0$ is undefined anyway.
- **Forgetting to distribute the antiderivative across every term in a sum**, or forgetting a term entirely when there are several to keep track of.
- **Forgetting to actually solve for $C$ in an initial-value problem.** Finding the general antiderivative with a leftover $+C$ isn't the final answer if you were given a specific point — you must use that point to pin down the exact value of $C$.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int x^3\,dx$
2. $\displaystyle\int 5\,dx$
3. $\displaystyle\int x^4\,dx$
4. $\displaystyle\int 3x^2\,dx$
5. $\displaystyle\int (x^2+2x)\,dx$
6. $\displaystyle\int (4x^3-3x^2+1)\,dx$
7. $\displaystyle\int \sqrt{x}\,dx$

### 🟡 Standard

8. $\displaystyle\int \sin x\,dx$
9. $\displaystyle\int (3\cos x - 2\sin x)\,dx$
10. $\displaystyle\int \sec^2x\,dx$
11. $\displaystyle\int \frac{2}{x^3}\,dx$
12. $\displaystyle\int \left(x^2-\frac{1}{x^2}\right)dx$
13. $\displaystyle\int (\sec x\tan x + \csc x\cot x)\,dx$
14. $\displaystyle\int (4x^3-6\sqrt{x})\,dx$

### 🔴 Challenge

15. Find $f(x)$ given $f'(x)=3x^2-4x+1$ and $f(0)=5$.
16. Find $f(x)$ given $f'(x)=6x^2-2$ and $f(1)=3$.
17. A particle's acceleration is $a(t)=6t-4$. Given $v(0)=3$ and $s(0)=2$, find $v(t)$ and $s(t)$.
18. Find $f(x)$ given $f'(x)=2\sin x+3\cos x$ and $f(0)=4$.
19. $\displaystyle\int (x+1)(x-2)\,dx$

### 🌍 Applied

20. A ball is thrown upward with acceleration due to gravity $a(t)=-32$ ft/s², initial velocity $v(0)=48$ ft/s, and initial height $s(0)=0$. Find $v(t)$ and $s(t)$, then find the ball's maximum height.
21. A company's marginal cost is $MC(x)=3x^2-12x+15$ dollars per unit, and fixed costs are $\$200$ (i.e., $C(0)=200$). Find the total cost function $C(x)$.
22. A company's marginal revenue is $MR(x)=50-2x$, with $R(0)=0$. Find the revenue function $R(x)$.
23. A car brakes with acceleration $a(t)=-10$ ft/s², starting from velocity $v(0)=60$ ft/s. Find $v(t)$, and determine how long it takes the car to come to a complete stop.
