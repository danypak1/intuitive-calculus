# Unit 28: Indefinite Integrals and the Substitution Method

## 1. The idea, in plain words

The power rule for antiderivatives works great — as long as the "inside" of what you're integrating is just plain $x$. But what happens with something like $\int (x^2+1)^3(2x)\,dx$? That's not a plain power of $x$ — it's a power of a whole *expression*, multiplied by something that looks suspiciously like the derivative of that expression. **This is the exact pattern the chain rule creates when you differentiate — and substitution is simply the chain rule, run in reverse.**

**Picture it like unwrapping a package.** The integral has a hidden "inner function" wrapped inside an "outer function," and multiplied by the inner function's own derivative — exactly the leftover crumbs the chain rule leaves behind. Substitution's whole trick is to **give that inner function a new, temporary name — $u$ — so the messy expression turns into something the basic power rule (or basic trig rules) can handle directly.**

**The step-by-step process:**

1. **Spot the pattern:** look for a function tucked inside another function, with the inner function's derivative (or a constant multiple of it) sitting right there as a separate factor.
2. **Let $u$ equal the inner function.**
3. **Compute $du$** — the derivative of $u$ with respect to $x$, times $dx$.
4. **Rewrite the entire integral in terms of $u$ only** — every single $x$ needs to disappear, replaced by $u$'s and $du$'s. If you can't fully clear out the $x$'s, you may have picked the wrong $u$.
5. **Integrate using the basic rules**, now that it's a simple expression in $u$.
6. **Substitute back**, replacing $u$ with the original expression in $x$, and add $+C$.

**For definite integrals, you have two options:** either substitute back to $x$ before plugging in the original bounds, or — often faster — **convert the bounds themselves into $u$-values** right when you substitute, and then never bother switching back to $x$ at all.

## 2. Toolbox

**The substitution method (indefinite integral):**
$$\int f\big(g(x)\big)\cdot g'(x)\,dx \;\overset{u=g(x)}{=}\; \int f(u)\,du = F(u)+C = F\big(g(x)\big)+C$$

**Changing the bounds for a definite integral (the shortcut — no need to substitute back):**
$$\int_a^b f\big(g(x)\big)g'(x)\,dx = \int_{g(a)}^{g(b)} f(u)\,du$$

**Common signals that a substitution is likely the right move:**

- A power of a whole expression, multiplied by that expression's derivative (or a constant multiple).
- A square root (or any fractional power) of an expression, multiplied by that expression's derivative.
- A trig function applied to an expression other than plain $x$, multiplied by that expression's derivative.

## 3. Common mistakes

- **Choosing a $u$ that doesn't actually simplify the integral.** If, after substituting, you still have leftover $x$'s that won't cancel, try a different choice of $u$.
- **Forgetting to convert $dx$ into $du$ properly.** If $du = g'(x)\,dx$, and the constant in front doesn't match exactly, you may need to divide (or multiply) both sides by that constant to solve for the piece you actually need.
- **Leaving some $x$'s in the integral after substitution.** A fully correct substitution should result in an expression purely in terms of $u$ — if any $x$ remains, something's gone wrong.
- **Forgetting to substitute back to $x$ at the end** (for indefinite integrals) — your final answer should generally be expressed in the original variable, unless you're doing a definite integral where you changed the bounds to $u$-values instead.
- **Mixing up the two approaches for definite integrals** — either change the bounds to $u$-values and finish entirely in $u$, or substitute back to $x$ and use the original bounds. Don't accidentally use $x$-bounds with a $u$-expression, or vice versa.
- **Forgetting the $+C$** on indefinite integrals.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int (x^2+1)^3(2x)\,dx$
2. $\displaystyle\int (3x+1)^4\,dx$
3. $\displaystyle\int 2x\sqrt{x^2+4}\,dx$
4. $\displaystyle\int (x^3+2)^2(3x^2)\,dx$
5. $\displaystyle\int (2x-5)^6\,dx$
6. $\displaystyle\int x(x^2+3)^5\,dx$
7. $\displaystyle\int \sin(3x)\,dx$

### 🟡 Standard

8. $\displaystyle\int \frac{4x}{\sqrt{2x^2+1}}\,dx$
9. $\displaystyle\int x^2(x^3+1)^4\,dx$
10. $\displaystyle\int \cos(2x+1)\,dx$
11. $\displaystyle\int \frac{2x}{(x^2+1)^2}\,dx$
12. $\displaystyle\int \sec^2x\tan x\,dx$
13. $\displaystyle\int (2x+3)(x^2+3x+1)^2\,dx$
14. $\displaystyle\int 3x^2\sin(x^3)\,dx$

### 🔴 Challenge

15. $\displaystyle\int x\sqrt{x+1}\,dx$ (this one needs an extra step — after substituting, you'll need to rewrite $x$ itself in terms of $u$)
16. $\displaystyle\int_0^1 2x(x^2+1)^3\,dx$ (change the bounds to $u$-values)
17. $\displaystyle\int_0^2 \frac{x}{\sqrt{x^2+9}}\,dx$ (change the bounds to $u$-values)
18. $\displaystyle\int \sin^3x\cos x\,dx$
19. $\displaystyle\int x^3\sqrt{x^4+5}\,dx$

### 🌍 Applied

20. A population's growth rate is modeled by $\dfrac{dP}{dt} = \dfrac{100t}{\sqrt{t^2+9}}$ people per year. Use substitution to find the general form of $P(t)$.
21. A company's marginal revenue is $MR(x)=6x^2(x^3+10)^2$. Use substitution to find the general revenue function $R(x)$.
22. Water flows into a tank at a rate of $r(t)=\dfrac{8t}{(t^2+1)^2}$ gal/min. Use substitution to find the total water collected over $[0,2]$ minutes.
23. An object's velocity is $v(t)=t\sin(t^2)$ m/s. Use substitution to find the exact distance traveled over $\left[0,\sqrt{\pi}\right]$.
