# Unit 9: Power Rule & Basic Rules

## 1. The idea, in plain words

Good news: all that limit-grinding from the last two units was worth it, because it's about to pay off. Mathematicians already did the hard work of running the limit definition on every basic type of function, and packaged the results into simple shortcut rules. From now on, for most everyday functions, you'll almost never need to touch the limit definition again — you'll just apply these rules directly.

**Picture the power rule like this:** whenever you have $x$ raised to some power, the exponent "comes down front" as a multiplier, and then the exponent itself drops by one. That's it. $x^5$ turns into $5x^4$. $x^{10}$ turns into $10x^9$. Same move, every time.

**Constants disappear.** A plain number like $7$ or $100$, sitting by itself with no $x$ attached, has a derivative of $0$. Why? Because a constant's graph is a flat horizontal line — completely unchanging — so its slope is always zero, everywhere (we actually proved this with the limit definition back in Unit 8).

**Constants tag along for the ride.** If a term is a number multiplied by a power of $x$ (like $7x^3$), the number just comes along unchanged while you apply the power rule to the $x^3$ part.

**Sums and differences split apart term by term.** If your function is built out of several terms added or subtracted together, you can differentiate each term completely separately, then just add/subtract the results back together. No special trick needed — this is one of the most convenient facts in all of calculus.

**The one prep step that trips people up:** the power rule only works directly on things that look like $x^n$. If you see a square root or a fraction with $x$ in the denominator, **rewrite it as a power first**, using negative and fractional exponents, before differentiating.

## 2. Toolbox

**Power Rule:**
$$\frac{d}{dx}\big[x^n\big] = n\,x^{n-1} \quad \text{for any real number } n$$

**Constant Rule:**
$$\frac{d}{dx}\big[c\big] = 0 \quad \text{(for any constant } c\text{)}$$

**Constant Multiple Rule:**
$$\frac{d}{dx}\big[c \cdot f(x)\big] = c \cdot f'(x)$$

**Sum/Difference Rule:**
$$\frac{d}{dx}\big[f(x) \pm g(x)\big] = f'(x) \pm g'(x)$$

**Rewriting radicals and fractions as powers, before you differentiate:**
$$\sqrt{x} = x^{1/2} \qquad \sqrt[n]{x} = x^{1/n} \qquad \frac{1}{x^n} = x^{-n} \qquad \frac{c}{x^n} = c\,x^{-n}$$

## 3. Common mistakes

- **Forgetting to rewrite radicals and fractions as powers before applying the rule.** You can't apply the power rule directly to $\sqrt{x}$ or $\dfrac{1}{x^2}$ as written — convert them to $x^{1/2}$ and $x^{-2}$ first.
- **Sign errors with negative exponents.** Remember that the exponent itself drops by $1$ — so $x^{-2}$ becomes $-2x^{-3}$, not $-2x^{-1}$. Double-check your new exponent by subtracting $1$ carefully, especially when starting from a negative or fractional exponent.
- **Dropping the constant multiplier by accident.** In $7x^3$, the $7$ stays out front; only the $x^3$ part transforms — you get $21x^2$, not $7x^2$ or $3x^2$.
- **Leaving a lone constant term in the final derivative.** If your original function has a plain number added on (like the $+5$ in $4x^2-3x+5$), that entire term vanishes completely in the derivative — don't accidentally carry it along.
- **Thinking a product like $x(x^2-3)$ needs a special "product rule."** For now, when one factor is a simple polynomial times another, just expand the multiplication first, then use the sum rule term by term. (An actual product rule for trickier cases is coming in the very next unit.)

## 4. Problem Set

### 🟢 Warm-up

1. $y = x^5$
2. $y = x^{10}$
3. $y = 7x^3$
4. $y = 4x^2-3x+5$
5. $y = x^3-2x^2+x-9$
6. $y = -3x^4+2x^2$
7. $y = 10$
8. $y = 6x$

### 🟡 Standard

9. $y = \sqrt{x}$
10. $y = \dfrac{1}{x^2}$
11. $y = \dfrac{1}{x^3}$
12. $y = 3\sqrt{x} - \dfrac{2}{x}$
13. $y = x^{3/2}$
14. $y = \dfrac{4}{\sqrt{x}}$
15. $y = 2x^3 - 5\sqrt{x} + \dfrac{1}{x}$

### 🔴 Challenge

16. $y = (x^2+1)^2$ (expand first, then differentiate)
17. $y = x(x^2-3)$ (expand first, then differentiate)
18. $y = \dfrac{x^3+2x^2-5x}{x}$ (divide every term by $x$ first, then differentiate)
19. $y = \dfrac{2x^4-3x^2+x}{x^2}$ (divide every term by $x^2$ first, then differentiate)
20. $y = (2x-1)^2$ (expand first, then differentiate)
21. Find all $x$-values where the tangent line to $y=x^3-3x$ is horizontal.

### 🌍 Applied

22. An object's position in meters after $t$ seconds is $s(t) = t^3-6t^2+9t$. Find the velocity function $v(t)=s'(t)$, then evaluate $v(1)$.
23. A company's cost (in dollars) to produce $x$ units is $C(x) = 0.01x^3-0.6x^2+13x+100$. Find the marginal cost function $C'(x)$, then evaluate $C'(10)$.
24. A rectangular garden bed has one side of length $x$ and the opposite arrangement forces its area to be $A(x) = x(20-x)$. Find $\dfrac{dA}{dx}$, then find the value of $x$ where $\dfrac{dA}{dx}=0$.
25. A company's revenue (in dollars) is modeled by $R(x) = 50x-0.02x^2$. Find $R'(x)$, then evaluate $R'(100)$.
