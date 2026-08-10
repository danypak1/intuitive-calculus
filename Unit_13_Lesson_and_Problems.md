# Unit 13: The Chain Rule

## 1. The idea, in plain words

So far, every function you've differentiated has had $x$ sitting "bare" inside — like $x^4$, or $\sin x$. But what happens when there's a whole expression tucked *inside* another function, like $(x^2+1)^4$ or $\sin(3x)$? You can't just apply the power rule or the trig formulas directly to the outside and call it done — you have to account for the fact that the "inside" is doing its own thing too.

**Picture it like a set of Russian nesting dolls.** $(x^2+1)^4$ has an **outer layer** (something to the 4th power) wrapped around an **inner layer** ($x^2+1$). To differentiate the whole thing, you differentiate the outer layer first — *pretending the inside is just a single blob* — and then, because that inside blob isn't actually just "$x$," you have to multiply by the inside's own derivative too. That extra multiplication is the entire chain rule in one sentence.

**Another way to picture it:** imagine you're tracking how fast your friend's friend's friend is influencing you — a chain of connections. If A affects B, and B affects C, and C affects you, then the *total* effect of A on you is the product of each link's individual effect: (effect of A on B) $\times$ (effect of B on C) $\times$ (effect of C on you). The chain rule works the exact same way — you multiply together the "rate of change" at every layer of the nesting.

**The most common version you'll use constantly — the Power Chain Rule:** whenever you see *anything* raised to a power — not just plain $x$, but a whole expression $u$ — the rule is: bring the exponent down, drop the exponent by one, and then **multiply by the derivative of whatever's inside** ($u'$). That last step, multiplying by $u'$, is the one people forget the most — and it's the entire point of this unit.

## 2. Toolbox

**The Chain Rule (general form):** if $y = f(g(x))$ — an "outer" function $f$ wrapped around an "inner" function $g$ — then

$$\frac{dy}{dx} = f'\big(g(x)\big) \cdot g'(x)$$

In plain words: **derivative of the outside (leaving the inside untouched) times derivative of the inside.**

**Power Chain Rule** (the version you'll use most often — here $u$ stands for any expression involving $x$):
$$\frac{d}{dx}\big[u^n\big] = n\,u^{n-1}\cdot u'$$

**Trig Chain Rule versions** (again, $u$ is any inner expression, not just plain $x$):
$$\frac{d}{dx}[\sin u] = \cos u \cdot u' \qquad \frac{d}{dx}[\cos u] = -\sin u \cdot u'$$
$$\frac{d}{dx}[\tan u] = \sec^2 u \cdot u' \qquad \frac{d}{dx}[\cot u] = -\csc^2 u \cdot u'$$
$$\frac{d}{dx}[\sec u] = \sec u \tan u \cdot u' \qquad \frac{d}{dx}[\csc u] = -\csc u \cot u \cdot u'$$

**How to identify the layers:** ask yourself, "what's the very last operation being done to $x$?" That outermost operation is your "outer function." Whatever's left inside it is your "inner function," $u$.

**Combining with earlier rules:** the chain rule doesn't replace the product or quotient rule — it works *alongside* them. If a problem has both a product and a composition, you'll need to use both rules together, one at each spot where they're needed.

## 3. Common mistakes

- **Forgetting to multiply by the derivative of the inside — by far the most common mistake in this entire unit.** Differentiating $(x^2+1)^4$ as just $4(x^2+1)^3$ and stopping there is incomplete — you must still multiply by the derivative of $x^2+1$, which is $2x$.
- **Applying the chain rule when it isn't needed.** If the inside is just plain $x$ (like $x^4$ by itself), there's no extra multiplication needed — the "derivative of the inside" is just $1$, which doesn't change anything. The chain rule matters when the inside is something *other* than plain $x$.
- **Mixing up which function is "outer" and which is "inner."** Always ask what the very last operation applied to $x$ is — that's the outer layer.
- **Forgetting to also use the product or quotient rule when a problem needs both.** A function like $x^2\sin^4x$ needs the product rule (for the two factors $x^2$ and $\sin^4x$) *and* the chain rule (to differentiate $\sin^4 x$ itself).
- **Sign errors when the inner function involves subtraction or a trig function.** Take extra care finding $u'$ before you multiply it in.

## 4. Problem Set

### 🟢 Warm-up

1. $y=(x+3)^4$
2. $y=(2x-1)^5$
3. $y=(3x+2)^3$
4. $y=(x^2+1)^3$
5. $y=(5-x)^4$
6. $y=(4x+7)^2$
7. $y=(x^2-2x)^2$

### 🟡 Standard

8. $y=\sin(3x)$
9. $y=\cos(x^2)$
10. $y=(2x^2-3)^{-1}$
11. $y=\sqrt{x^2+4}$
12. $y=\tan(2x)$
13. $y=(3x-1)^{1/3}$
14. $y=\sin^2 x$ (that is, $(\sin x)^2$)

### 🔴 Challenge

15. $y=\left(\dfrac{x^2}{2}+x-\dfrac{1}{x}\right)^4$
16. $y=\sin^4 x$
17. $y = x^2\sin^4 x + x\cos^{-2}x$
18. $y = (x^2+1)^3(x-1)^2$
19. $y = \sqrt{\sin x}$
20. $y = (1+\cos x)^3$

### 🌍 Applied

21. A balloon's radius (in cm) grows according to $r(t)=2t$, and its volume is $V(r)=\dfrac{4}{3}\pi r^3$. Using the chain rule, find $\dfrac{dV}{dt}$, then evaluate it at $t=1$.
22. A wave's height (in cm) is modeled by $h(t)=3\sin(2t)$. Find $h'(t)$ using the chain rule, then evaluate $h'(0)$ and interpret what it means.
23. A company's production level (in units) is $x(t)=10t$, and its cost (in dollars) is $C(x)=\sqrt{x^2+50}$. Using the chain rule, find $\dfrac{dC}{dt}$, then evaluate it at $t=2$.
24. A greenhouse's temperature (in °F) is modeled by $T(t) = (t+2)^3-5$. Find $T'(t)$ using the chain rule, then evaluate $T'(1)$.
