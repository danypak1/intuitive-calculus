# Unit 31: Natural Logarithms

## 1. The idea, in plain words

You've been carefully steering around one particular antiderivative for a while now — $\int \dfrac{1}{x}\,dx$ — because the power rule breaks down exactly there (you'd be dividing by $n+1=0$). **This unit finally gives you the tool that fills that gap: the natural logarithm, $\ln x$.**

**What is $\ln x$, really?** It's the *inverse function* of $e^x$ (where $e\approx2.71828$ is a special constant that shows up throughout calculus). Just like $\sqrt{x}$ undoes squaring, $\ln x$ undoes raising $e$ to a power. So $\ln x = k$ means exactly the same thing as $e^k = x$ — they're two ways of writing the same relationship.

**Why logarithms are so useful: they turn multiplication into addition, and powers into multiplication.** This isn't just a neat trick — it's a genuine simplification tool. Before differentiating a complicated expression full of products, quotients, and powers wrapped inside a $\ln(\cdot)$, it's almost always worth **expanding it using log properties first** — you'll often turn one nasty differentiation problem into three or four trivially easy ones.

**The derivative of $\ln x$ is refreshingly simple:** $\dfrac{d}{dx}[\ln x] = \dfrac1x$. And since $\ln x$ is a function like any other, the chain rule applies the moment you have $\ln(\text{something more complicated than plain }x)$.

**And the antiderivative you've been waiting for:**
$$\int \frac1x\,dx = \ln|x| + C$$

## 2. Toolbox

**Definition (inverse relationship with $e^x$):**
$$\ln x = k \iff e^k = x \qquad \qquad e^{\ln x} = x \qquad \qquad \ln(e^x) = x$$

**Basic values:** $\ln 1 = 0$, $\quad \ln e = 1$.

**Log properties (the "expand first" toolkit):**
$$\ln(ab) = \ln a + \ln b \qquad \ln\left(\frac{a}{b}\right) = \ln a - \ln b \qquad \ln(a^n) = n\ln a$$

**Important: these rules only work for products, quotients, and powers — never for sums.** $\ln(a+b)$ does **not** equal $\ln a + \ln b$; there's no simplification for that at all.

**Derivative:**
$$\frac{d}{dx}[\ln x] = \frac1x \qquad (x>0)$$

**Chain rule version** (for $\ln$ of anything more complex than plain $x$):
$$\frac{d}{dx}[\ln u] = \frac{u'}{u}$$

**Antiderivative:**
$$\int \frac1x\,dx = \ln|x| + C$$

**Solving equations involving $\ln$:** if $\ln(\text{expression})=k$, exponentiate both sides ($e^{(\cdot)}$) to clear the log: $\text{expression} = e^k$.

## 3. Common mistakes

- **Applying a log property to a sum.** $\ln(a+b) \ne \ln a + \ln b$ — this only works for products, quotients, and powers, never addition.
- **Forgetting the absolute value in the antiderivative.** $\dfrac1x$ is defined for negative $x$ too, even though $\ln x$ alone isn't — that's exactly why the antiderivative needs $\ln|x|$, not just $\ln x$.
- **Forgetting the domain restriction $x>0$ for $\ln x$ itself.** When solving an equation like $\ln(x-8)=5$, remember the *inside* of the log must be positive — always check your solution makes sense in that light.
- **Forgetting the chain rule when differentiating $\ln(u)$ for $u \ne x$.** You must multiply by $u'$ — don't just write $\dfrac1u$ and stop.
- **Diving straight into product/quotient rule on a messy log expression instead of simplifying with log properties first.** This is the single biggest time-saver in this whole unit — always check whether expanding first will make the derivative dramatically easier.

## 4. Problem Set

### 🟢 Warm-up

1. Simplify $\ln(8)$ in terms of $\ln 2$.
2. Find $\dfrac{d}{dx}\big[\ln(5x)\big]$.
3. Find $\dfrac{d}{dx}\big[\ln(x^2+1)\big]$.
4. Solve for $x$: $\ln(x)=3$.
5. Find $\displaystyle\int \frac{3}{x}\,dx$.
6. Simplify $\ln(x^3y^2)$ using log properties.

### 🟡 Standard

7. Solve for $x$: $\ln(x-8)=5$.
8. Find $\dfrac{d}{dx}\big[x\ln x\big]$.
9. Find $\dfrac{d}{dx}\left[\dfrac{\ln x}{x}\right]$.
10. Simplify $\ln\big(x^2\sqrt{x+3}\big)$ using log properties, then find its derivative.
11. Find $\displaystyle\int \frac{2x}{x^2+1}\,dx$.
12. Solve for $x$: $\ln(2x+1)=0$.
13. Find $\dfrac{d}{dx}\big[\ln(\sin x)\big]$.

### 🔴 Challenge

14. $y = \dfrac{x^5}{4}\ln x - \dfrac{x^4}{4}$. Find $\dfrac{dy}{dx}$.
15. $y = \ln\left(\dfrac{1}{x^2\sqrt{x+1}}\right)$. Simplify first using log properties, then find $\dfrac{dy}{dx}$.
16. $y = \ln\big(3x^3 e^{x^2}\big)$. Simplify first using log properties, then find $\dfrac{dy}{dx}$.
17. Solve for $x$: $2\ln(x)+\ln(4)=\ln(36)$.
18. Find $\displaystyle\int \frac{x^2+1}{x}\,dx$.

### 🌍 Applied

19. A population grows according to $P(t)=500e^{0.05t}$. Find the time $t$ when the population reaches $1000$.
20. A radioactive sample decays according to $A(t)=100e^{-0.2t}$ (grams). Find the time $t$ when only $25$ grams remain.
21. A company's marginal cost is $MC(x)=\dfrac{10}{x}$ dollars per unit, for $x\ge1$. Find the total cost increase from $x=1$ to $x=5$.
22. A tank's volume changes at a rate of $\dfrac{dV}{dt}=\dfrac{6}{t}$ (gallons/hour), for $t\ge1$. Find the total volume change from $t=1$ to $t=e$ hours.
