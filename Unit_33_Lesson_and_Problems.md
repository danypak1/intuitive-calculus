# Unit 33: Exponential Change and Separable Differential Equations

## 1. The idea, in plain words

So far, every derivative problem has started with a function and asked you to find its rate of change. **This unit flips that around: you're given the rate of change (as an equation involving $\dfrac{dy}{dx}$), and your job is to find the original function $y$ that produces it.** An equation like this — one that involves a derivative — is called a **differential equation**, and solving it means finding the family of functions $y$ that satisfy it.

**A "separable" differential equation is one where you can physically pull the $x$'s and $y$'s apart onto opposite sides of the equation.** Picture $\dfrac{dy}{dx}$ as a fraction (it isn't technically one, but it behaves enough like one for this purpose) — if the right-hand side factors into "a piece with only $x$'s" times "a piece with only $y$'s," you can shuffle every $y$ term (along with $dy$) to one side, and every $x$ term (along with $dx$) to the other side.

**Once separated, you just integrate both sides.** The left side gives you something in terms of $y$; the right side gives you something in terms of $x$; and you tie them together with a single constant of integration. If possible, you then solve algebraically for $y$ to get an **explicit** solution — a genuine formula for $y$ in terms of $x$. Sometimes solving for $y$ isn't practical, and you leave the answer in **implicit** form instead (an equation relating $x$ and $y$, without $y$ isolated).

**A famous special case worth deriving once and remembering forever: the Law of Exponential Change.** Whenever a quantity's rate of change is proportional to the quantity itself ($\dfrac{dy}{dt}=ky$), separating and integrating always produces the same shape of answer: $y=y_0e^{kt}$, where $y_0$ is the starting amount. This is exactly the formula behind population growth, radioactive decay, compound interest, and Newton's Law of Cooling — and now you'll see precisely *why* it always takes that shape, instead of just being handed the formula.

## 2. Toolbox

**The separation-and-integration procedure:**

1. Rewrite $\dfrac{dy}{dx} = f(x)g(y)$ by moving all $y$-terms (with $dy$) to one side, and all $x$-terms (with $dx$) to the other:
$$\frac{dy}{g(y)} = f(x)\,dx$$
2. Integrate both sides:
$$\int \frac{dy}{g(y)} = \int f(x)\,dx$$
3. Add a single constant of integration (the two separate $+C$'s from each side combine into one).
4. Solve for $y$ explicitly if possible; if not, leave the relationship implicit.
5. If given an initial condition (like $y(0)=y_0$), plug it in to solve for the specific value of the constant.

**The Law of Exponential Change** (a direct consequence of separating $\dfrac{dy}{dt}=ky$):
$$\frac{dy}{dt} = ky \quad\Longrightarrow\quad y = y_0e^{kt}$$
where $y_0=y(0)$ is the initial amount, and $k>0$ means growth, $k<0$ means decay.

**Newton's Law of Cooling** (a shifted version of the same idea): if $\dfrac{dT}{dt}=-k(T-T_s)$ (where $T_s$ is the surrounding/ambient temperature), then
$$T(t) = T_s + (T_0-T_s)e^{-kt}$$

## 3. Common mistakes

- **Trying to integrate before separating.** You cannot integrate $\dfrac{dy}{dx}=f(x)g(y)$ directly — the variables must be fully separated onto opposite sides first.
- **Forgetting the constant of integration**, or adding two separate constants (one from each side) instead of combining them into a single overall constant.
- **Losing track of signs when solving for $y$ after integrating**, especially when a $\ln|y|$ term needs to be exponentiated back out.
- **Forgetting to apply the initial condition**, if one is given — a general solution with an unresolved constant is not the final answer if you were handed a starting value.
- **Trying to force a non-separable equation into this framework.** Always double-check that the right-hand side genuinely factors into "$x$-stuff times $y$-stuff" before attempting to separate.

## 4. Problem Set

### 🟢 Warm-up

Find the general solution to each differential equation.

1. $\dfrac{dy}{dx} = x$
2. $\dfrac{dy}{dx} = 2y$
3. $\dfrac{dy}{dx} = \dfrac{x}{y}$
4. $\dfrac{dy}{dx} = 3x^2$, with $y(0)=5$
5. $\dfrac{dy}{dx} = \dfrac{y}{x}$ (for $x>0$)
6. $\dfrac{dy}{dx} = -2y$, with $y(0)=10$

### 🟡 Standard

7. $\dfrac{dy}{dx} = xe^{-y}$
8. $\dfrac{dy}{dx} = \dfrac{\cos x}{y}$
9. $\dfrac{dy}{dx} = y\cos x$
10. $\dfrac{dy}{dx} = x^2y$, with $y(0)=2$
11. $\dfrac{dy}{dx} = 2xy^2$
12. $\dfrac{dy}{dx} = e^{x+y}$ (rewrite using exponent rules first!)

### 🔴 Challenge

13. Solve $\dfrac{dy}{dx} = \sin x\cdot e^{-y}$.
14. Starting from $\dfrac{dy}{dt}=ky$, separate and integrate to derive $y=Ce^{kt}$, then explain how the constant $C$ relates to $y_0=y(0)$.
15. Solve $\dfrac{dy}{dx} = y^2\sin x$, with $y(0)=1$.
16. Solve $\dfrac{dy}{dx} = \dfrac{x+1}{y-2}$, with $y(0)=4$.
17. Solve $\dfrac{dy}{dx} = -xy$, with $y(0)=3$.

### 🌍 Applied

18. A population grows according to $\dfrac{dP}{dt}=0.04P$, with $P(0)=1000$. Find $P(t)$, and find the population after $20$ years.
19. An object cools according to Newton's Law of Cooling: $\dfrac{dT}{dt}=-0.1(T-70)$, with $T(0)=200$ (ambient temperature $70°$). Find $T(t)$, and find the temperature after $10$ minutes.
20. A radioactive sample decays according to $\dfrac{dA}{dt}=-0.05A$, with $A(0)=200$ grams. Find $A(t)$, and find the time it takes to decay to $100$ grams.
21. A drug's concentration in the bloodstream decreases according to $\dfrac{dC}{dt}=-0.3C$, with $C(0)=80$ mg. Find $C(t)$, and find the concentration after $5$ hours.
