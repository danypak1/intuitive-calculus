# Unit 36: Using Basic Integration Formulas

## 1. The idea, in plain words

You now have a whole toolkit of antiderivative formulas scattered across several units — the power rule, trig forms, $e^x$, $\ln|x|$, and (from Unit 35) the inverse trig forms. **This unit is about recognizing which formula fits a given integral, and — when the integral doesn't quite match any formula as written — reshaping it with algebra until it does.**

**The biggest new skill here: completing the square to unlock a hidden $\arcsin$ or $\arctan$ form.** Whenever you see a quadratic expression sitting under a square root, or sitting alone in a denominator, and it doesn't factor nicely, try completing the square. This rewrites the quadratic as $(x-h)^2$ plus or minus a constant — and that shape is *exactly* what the $\arcsin$ and $\arctan$ antiderivative formulas are built around.

**Picture it like fitting a puzzle piece.** The formulas $\displaystyle\int\frac{dx}{\sqrt{a^2-x^2}}=\arcsin\left(\frac xa\right)+C$ and $\displaystyle\int\frac{dx}{a^2+x^2}=\frac1a\arctan\left(\frac xa\right)+C$ only fit a very specific shape: a perfect square subtracted from (or added to) a constant. A messy quadratic like $x^2-6x+13$ doesn't look like that shape at first glance — but after completing the square, it becomes $(x-3)^2+4$, which *is* exactly that shape (with $u=x-3$ standing in for the variable).

## 2. Toolbox

**The basic formulas, all in one place:**
$$\int x^n\,dx = \frac{x^{n+1}}{n+1}+C \ (n\ne-1) \qquad \int \frac1x\,dx = \ln|x|+C \qquad \int e^x\,dx = e^x+C$$
$$\int \sin x\,dx=-\cos x+C \qquad \int \cos x\,dx = \sin x+C$$
$$\int \frac{dx}{\sqrt{a^2-x^2}} = \arcsin\left(\frac{x}{a}\right)+C \qquad \int \frac{dx}{a^2+x^2} = \frac1a\arctan\left(\frac{x}{a}\right)+C$$

**Completing the square, step by step** (for a quadratic $x^2+bx+c$):

1. Take half of $b$, square it: $\left(\dfrac b2\right)^2$.
2. Add and subtract that amount: $x^2+bx+\left(\dfrac b2\right)^2-\left(\dfrac b2\right)^2+c$.
3. The first three terms form a perfect square: $\left(x+\dfrac b2\right)^2$.
4. Combine the leftover constants.

**Matching the completed-square form to the right formula:**

- If it ends up as (constant) $-(x-h)^2$ under a square root $\to$ use the $\arcsin$ formula, with $u=x-h$.
- If it ends up as $(x-h)^2+$ (constant) in a plain denominator $\to$ use the $\arctan$ formula, with $u=x-h$.

**Don't forget the substitution when the coefficient on $x$ isn't $1$** — if the quadratic has a coefficient like $4x^2$ instead of plain $x^2$, a quick substitution (e.g., $u=2x$) usually cleans it up before completing the square.

## 3. Common mistakes

- **Forgetting the scaling factor "$a$" in the $\arcsin$/$\arctan$ formulas.** These formulas aren't just $\arcsin(x)$ or $\arctan(x)$ unless $a=1$ — always divide by the correct $a$ both inside the inverse trig function and (for arctan) out front.
- **Sign errors while completing the square**, especially when a leading negative sign is involved (like $-x^2+4x-3$) — factor the negative out carefully before completing the square on what's left.
- **Misidentifying which formula applies.** A quadratic under a square root pairs with $\arcsin$; a quadratic alone in a denominator (no square root) pairs with $\arctan$. Mixing these up leads to the wrong antiderivative shape entirely.
- **Forgetting to substitute back at the end**, if you introduced a $u=x-h$ substitution partway through.
- **Forgetting to double check your completed-square work** by mentally re-expanding it — a small arithmetic slip here throws off everything that follows.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int \frac{dx}{\sqrt{1-x^2}}$
2. $\displaystyle\int \frac{dx}{1+x^2}$
3. $\displaystyle\int x^4\,dx$
4. $\displaystyle\int e^{5x}\,dx$
5. $\displaystyle\int \cos(4x)\,dx$
6. $\displaystyle\int \frac{dx}{\sqrt{4-x^2}}$

### 🟡 Standard

7. $\displaystyle\int \frac{dx}{9+x^2}$
8. $\displaystyle\int \frac{dx}{\sqrt{16-x^2}}$
9. $\displaystyle\int \frac{3\,dx}{x^2+4}$
10. $\displaystyle\int \frac{dx}{\sqrt{9-4x^2}}$
11. Complete the square: rewrite $x^2-6x+13$ in the form $(x-h)^2+k$.
12. $\displaystyle\int \frac{dx}{x^2-6x+13}$ (use your result from Problem 11)
13. $\displaystyle\int \frac{dx}{\sqrt{-x^2+2x+3}}$

### 🔴 Challenge

14. $\displaystyle\int \frac{dx}{\sqrt{-x^2+4x-3}}$
15. $\displaystyle\int \frac{dx}{x^2+4x+13}$
16. $\displaystyle\int \frac{dx}{\sqrt{8-2x-x^2}}$
17. $\displaystyle\int \frac{(2x+3)\,dx}{x^2+4}$ (split into two pieces first!)
18. $\displaystyle\int \frac{dx}{\sqrt{3-2x-x^2}}$

### 🌍 Applied

19. A particle's velocity is $v(t) = \dfrac{1}{\sqrt{4-t^2}}$. Find the position function $s(t)$, given $s(0)=0$.
20. An electrical current model is $I(x) = \dfrac{1}{x^2+9}$. Find the total charge $\displaystyle\int_0^3 I(x)\,dx$.
21. A structural deflection model requires evaluating $\displaystyle\int \frac{dx}{\sqrt{-x^2+6x-5}}$. Complete the square and find the general antiderivative.
22. Evaluate $\displaystyle\int_{-2}^{2} \frac{dx}{\sqrt{4-x^2}}$.
