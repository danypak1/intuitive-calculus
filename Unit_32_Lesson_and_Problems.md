# Unit 32: Exponential Functions

## 1. The idea, in plain words

Meet the single most well-behaved function in all of calculus: $e^x$. **Its derivative is itself.** Not a scaled version, not a shifted version — literally, exactly the same function you started with:
$$\frac{d}{dx}\big[e^x\big] = e^x$$

**Picture what this means:** at every single point on the graph of $y=e^x$, the *height* of the curve and the *slope* of the curve are the same number. If the curve is at height $5$, its slope right there is also $5$. This is genuinely unique — no other basic function behaves this way — and it's exactly why $e$ (a special constant, $\approx2.71828$) shows up everywhere in calculus, from compound interest to population growth to radioactive decay.

**A warning about a very natural, very wrong instinct:** because you're so used to the power rule bringing an exponent down front, it's tempting to think $\dfrac{d}{dx}[e^x]$ should involve "bringing down" something. **It doesn't.** $e^x$ isn't $x$ raised to a power — it's a *constant* raised to a variable power, which is a completely different kind of function, and it plays by its own (much simpler) rule.

**Since $e^x$ is a function like any other, the chain rule still applies whenever the exponent is something more complicated than plain $x$** — you just multiply by the derivative of that exponent, exactly like every other composed function you've handled.

**Because $\ln x$ and $e^x$ are inverse functions of each other** (from Unit 31), solving an equation with $e$ raised to some expression is just a matter of taking $\ln$ of both sides to pull the exponent back down to ground level.

## 2. Toolbox

**Derivative:**
$$\frac{d}{dx}\big[e^x\big] = e^x$$

**Chain rule version** (for $e$ raised to anything more complex than plain $x$):
$$\frac{d}{dx}\big[e^u\big] = e^u\cdot u'$$

**Antiderivative:**
$$\int e^x\,dx = e^x+C \qquad \qquad \int e^u\cdot u'\,dx = e^u+C \ \text{(via substitution)}$$

**Basic exponent properties** (same rules as any exponent):
$$e^0=1 \qquad e^a\cdot e^b = e^{a+b} \qquad \frac{e^a}{e^b}=e^{a-b} \qquad (e^a)^b = e^{ab}$$

**Inverse relationship with $\ln$:**
$$e^{\ln x}=x \qquad \ln(e^x)=x$$

**Solving an equation with $e$ raised to an expression:** isolate the exponential term first if needed, then take $\ln$ of both sides to bring the exponent down:
$$e^{(\text{expression})} = k \quad\Longrightarrow\quad \text{expression} = \ln k$$

## 3. Common mistakes

- **Trying to apply the power rule to $e^x$.** $\dfrac{d}{dx}[e^x]$ is just $e^x$ — there's no exponent to "bring down" and no reduction in power. This is the single most common error in this entire unit.
- **Forgetting the chain rule multiplier when the exponent isn't plain $x$.** $\dfrac{d}{dx}[e^{3x}]$ is $3e^{3x}$, not just $e^{3x}$ — you must multiply by the derivative of the exponent.
- **Forgetting to isolate the exponential term before taking $\ln$.** If there's addition or subtraction happening around the $e^{(\cdot)}$ term (like $2e^x-3=7$), you must isolate the exponential piece by itself *before* taking the log of anything.
- **Sign errors in the exponent when solving equations.** Take care carrying negative signs through, especially in decay problems.
- **Forgetting that $\int e^x\,dx = e^x+C$ doesn't follow the power-rule pattern.** There's no "$+1$" to the exponent and no dividing by a new exponent — $e^x$ is simply its own antiderivative too.

## 4. Problem Set

### 🟢 Warm-up

1. $\dfrac{d}{dx}\big[e^x\big]$
2. $\dfrac{d}{dx}\big[e^{2x}\big]$
3. $\dfrac{d}{dx}\big[3e^x\big]$
4. Solve for $x$: $e^x=5$.
5. $\displaystyle\int e^x\,dx$
6. $\dfrac{d}{dx}\big[e^x+x^2\big]$

### 🟡 Standard

7. $\dfrac{d}{dx}\big[e^{x^2}\big]$
8. $\dfrac{d}{dx}\big[e^{3x+1}\big]$
9. $\dfrac{d}{dx}\big[xe^x\big]$
10. $\dfrac{d}{dx}\left[\dfrac{e^x}{x}\right]$
11. Solve for $x$: $e^{2x-1}=7$.
12. $\displaystyle\int 3e^{2x}\,dx$
13. $\displaystyle\int_0^1 e^x\,dx$

### 🔴 Challenge

14. Solve for $x$: $e^{3x-6}=9$.
15. $y=(9x^2-6x+2)e^{3x}$. Find $\dfrac{dy}{dx}$.
16. $\dfrac{d}{dx}\big[e^{\sin x}\big]$
17. $\displaystyle\int 2xe^{x^2}\,dx$
18. Solve for $x$: $2e^{x}-3=7$.

### 🌍 Applied

19. An investment grows according to $A(t)=1000e^{0.06t}$ (continuously compounded). Find the time $t$ when the investment doubles.
20. A population grows according to $P(t)=200e^{0.03t}$. Find the growth rate function $\dfrac{dP}{dt}$, and evaluate it at $t=10$.
21. A drug's concentration in the bloodstream is $C(t)=50e^{-0.5t}$ mg. Find the rate of change of concentration, $\dfrac{dC}{dt}$, at $t=2$.
22. A cooling object's temperature difference from room temperature is modeled by $D(t)=80e^{-0.1t}$. Find the total accumulated area under this curve from $t=0$ to $t=10$.
