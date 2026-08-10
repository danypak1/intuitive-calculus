# Unit 2: Limit of a Function and Limit Laws

## 1. The idea, in plain words

A **limit** answers the question: "As $x$ gets closer and closer to some number, what value does $f(x)$ get closer and closer to?" It's not asking what happens *at* that exact number — it's asking what $f(x)$ is *heading toward* as you approach it.

**Picture it:** Imagine walking toward a friend's house. You never actually need to teleport there — you just need to know that with each step, you're getting closer and closer. The limit is the address you're walking toward, whether or not you ever technically "arrive" (i.e., whether or not $f$ is even defined right at that point).

For most of the functions you'll meet early on — polynomials, square roots, nice fractions — the function behaves the way you'd expect, and the limit is simply what you get by plugging the number in. This is called **direct substitution**.

But sometimes, plugging the number straight in gives you $\dfrac{0}{0}$, which tells you *nothing* — it's a mathematical dead end, not an answer. When this happens, it usually means the top and bottom of the fraction share a hidden common piece that's causing trouble at that one point. Our job is to dig that hidden piece out — either by **factoring and canceling**, or by **rationalizing** (multiplying by a clever form of $1$ to get rid of an awkward square root) — and then try substituting again.

## 2. Toolbox

**Limit notation:** $\displaystyle\lim_{x\to a} f(x) = L$ means "as $x$ approaches $a$, $f(x)$ approaches $L$."

**Direct substitution rule:** If $f(x)$ is a polynomial, or any combination of $+,-,\times,\div,\sqrt{\ }$ that doesn't cause a division by zero at $x=a$, then:
$$\lim_{x\to a} f(x) = f(a)$$

**Limit laws** (these let you break a complicated limit into simpler pieces): if $\displaystyle\lim_{x\to a}f(x)$ and $\displaystyle\lim_{x\to a}g(x)$ both exist,

$$\lim_{x\to a}\big[f(x)+g(x)\big] = \lim_{x\to a}f(x) + \lim_{x\to a}g(x)$$
$$\lim_{x\to a}\big[f(x)\cdot g(x)\big] = \lim_{x\to a}f(x) \cdot \lim_{x\to a}g(x)$$
$$\lim_{x\to a}\frac{f(x)}{g(x)} = \frac{\lim_{x\to a}f(x)}{\lim_{x\to a}g(x)}, \quad \text{as long as } \lim_{x\to a}g(x)\ne 0$$
$$\lim_{x\to a}\big[c\cdot f(x)\big] = c \cdot \lim_{x\to a}f(x) \quad \text{(for any constant } c\text{)}$$
$$\lim_{x\to a} x^n = a^n$$

**The $\frac{0}{0}$ fix-it kit:**

- **Factor and cancel:** if plugging in gives $\frac{0}{0}$ on a fraction of polynomials, factor the top and bottom. There will always be a matching factor that cancels out — that factor is exactly what was causing the $0/0$.
- **Rationalize:** if there's a square root involved, multiply the top and bottom by the **conjugate** of the square-root part (same terms, opposite sign in the middle). This uses the pattern $(\sqrt{u}-v)(\sqrt{u}+v) = u - v^2$ to make the square root disappear from one part of the fraction, which usually reveals a common factor you can cancel.

## 3. Common mistakes

- **Giving up when you see $\frac{0}{0}$.** This is *not* the final answer — it's a signal to factor or rationalize and try again.
- **Forgetting to factor completely.** If you cancel one factor but the numerator or denominator still has more work to do, you might miss a further simplification (or a further cancellation).
- **Sign errors while factoring quadratics.** Double-check by mentally re-expanding your factored form before moving on.
- **Canceling terms instead of factors.** You can only cancel something that is *multiplied* on both top and bottom — never cancel a piece that's part of a sum, like trying to cancel the $x$'s in $\dfrac{x+3}{x+5}$ (that's not allowed; $x$ isn't a common factor there).
- **Forgetting to multiply the denominator by the conjugate too.** When rationalizing, whatever you multiply the top by, you must also multiply the bottom by — you're really just multiplying by a clever version of $1$.

## 4. Problem Set

### 🟢 Warm-up (direct substitution)

1. $\displaystyle\lim_{x\to 3}(2x+1)$
2. $\displaystyle\lim_{x\to -2}(x^2-3x+4)$
3. $\displaystyle\lim_{x\to 1}(3x^2-2x+5)$
4. $\displaystyle\lim_{x\to 0}(x^3+2x^2-1)$
5. $\displaystyle\lim_{x\to 4}\sqrt{x+5}$
6. $\displaystyle\lim_{x\to 2}\frac{x^2+1}{x+3}$
7. $\displaystyle\lim_{x\to 5}\frac{x+5}{x^2-20}$

### 🟡 Standard (factor and cancel)

8. $\displaystyle\lim_{x\to 2}\frac{x^2-7x+10}{x-2}$
9. $\displaystyle\lim_{x\to 3}\frac{x^2-9}{x-3}$
10. $\displaystyle\lim_{x\to -1}\frac{x^2+3x+2}{x+1}$
11. $\displaystyle\lim_{x\to 4}\frac{x^2-16}{x-4}$
12. $\displaystyle\lim_{x\to 1}\frac{x^3-1}{x-1}$
13. $\displaystyle\lim_{x\to 2}\frac{x^2-5x+6}{x^2-4}$
14. $\displaystyle\lim_{x\to 3}\frac{x^2-2x-3}{x^2-9}$

### 🔴 Challenge (rationalizing and trickier algebra)

15. $\displaystyle\lim_{x\to 4}\frac{x-4}{\sqrt{x}-2}$
16. $\displaystyle\lim_{x\to 2}\frac{\sqrt{x^2+12}-4}{x-2}$
17. $\displaystyle\lim_{x\to 0}\frac{\sqrt{x+9}-3}{x}$
18. $\displaystyle\lim_{x\to 9}\frac{x-9}{\sqrt{x}-3}$
19. $\displaystyle\lim_{h\to 0}\frac{(2+h)^2-4}{h}$
20. $\displaystyle\lim_{x\to 1}\frac{\frac{1}{x}-1}{x-1}$

### 🌍 Applied

21. A company's revenue (in dollars) from selling $x$ units is $R(x) = 5x - 0.01x^2$. Find $\displaystyle\lim_{x\to 10}R(x)$, and explain what this number means about the revenue as production nears $10$ units.
22. A factory's total cost to make $x$ items is $C(x) = 200+3x$ dollars. The **average cost per item** is $\dfrac{C(x)}{x}$. Find $\displaystyle\lim_{x\to 50}\frac{C(x)}{x}$.
23. A population model gives the number of bacteria (in thousands) after $t$ hours as $P(t) = \dfrac{100t}{t+5}$. Find $\displaystyle\lim_{t\to 5}P(t)$.
24. An object's velocity model is $v(t) = \dfrac{t^2-4}{t-2}$ for $t$ near $2$ (this model happens to be undefined exactly at $t=2$). Find $\displaystyle\lim_{t\to 2}v(t)$, and explain what it tells us about the object's velocity as $t$ gets close to $2$, even though the formula itself breaks down right at $t=2$.
