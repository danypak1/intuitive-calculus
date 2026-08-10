# Unit 41: Improper Integrals

## 1. The idea, in plain words

Every definite integral you've computed so far has had two well-behaved, finite boundaries, with a perfectly continuous function in between. **This unit asks: what happens if one of those assumptions breaks?** What if the interval stretches out to infinity? What if the function itself shoots up to infinity somewhere inside (or at the edge of) the interval? These are called **improper integrals**, and remarkably, many of them still have a well-defined, finite answer.

**The fix for both situations is the same core idea: replace the "bad" boundary with a variable, and take a limit as that variable approaches the problem spot.** You're not integrating all the way to infinity (or all the way to a vertical asymptote) directly — you're integrating up to some safe stopping point $b$, and then asking what happens as $b$ creeps closer and closer to the danger zone.

**Type 1 — an infinite interval.** Picture trying to find the area under a curve that stretches on forever to the right. Instead of computing that area directly (impossible), compute the area up to some finite point $b$, and then take the limit as $b\to\infty$:
$$\int_a^\infty f(x)\,dx = \lim_{b\to\infty}\int_a^b f(x)\,dx$$

**Type 2 — a discontinuous integrand (a vertical asymptote somewhere in the interval).** Picture a function that shoots up to infinity right at one edge of your interval (or somewhere in the middle). Instead of integrating straight through the danger point, sneak up to it with a limit:
$$\int_a^b f(x)\,dx = \lim_{t\to a^+}\int_t^b f(x)\,dx \quad \text{(if the trouble is at } x=a\text{)}$$

**The verdict — converges or diverges.** If the limit works out to an actual finite number, we say the improper integral **converges** to that value. If the limit turns out to be infinite (or doesn't settle down to any single number), we say it **diverges** — there's no finite area to report.

**A crucial nuance: some intervals hide a discontinuity you might not notice at first glance.** Always scan the *entire* interval — including any points strictly inside it, not just the endpoints — for anywhere the function blows up. If you find one in the interior, you must **split the integral into two pieces at that point**, and check each piece separately — and if even one of the two pieces diverges, the *whole* original integral diverges, no matter how well-behaved the other piece is.

## 2. Toolbox

**Type 1 (infinite interval):**
$$\int_a^\infty f(x)\,dx = \lim_{b\to\infty}\int_a^b f(x)\,dx \qquad \int_{-\infty}^b f(x)\,dx = \lim_{a\to-\infty}\int_a^b f(x)\,dx$$

For an integral from $-\infty$ to $\infty$, split at any convenient point (usually $0$) and require **both** halves to converge:
$$\int_{-\infty}^{\infty} f(x)\,dx = \int_{-\infty}^{0} f(x)\,dx + \int_{0}^{\infty} f(x)\,dx$$

**Type 2 (discontinuity in the integrand):**

- Discontinuity at the **lower** endpoint $a$: $\displaystyle\int_a^b f(x)\,dx = \lim_{t\to a^+}\int_t^b f(x)\,dx$
- Discontinuity at the **upper** endpoint $b$: $\displaystyle\int_a^b f(x)\,dx = \lim_{t\to b^-}\int_a^t f(x)\,dx$
- Discontinuity at an **interior** point $c$: split into $\displaystyle\int_a^c f(x)\,dx + \int_c^b f(x)\,dx$, and require **both** pieces to converge.

**A useful reference (the "p-integral" pattern):**
$$\int_1^\infty \frac{1}{x^p}\,dx \text{ converges if } p>1, \text{ diverges if } p\le1$$
$$\int_0^1 \frac{1}{x^p}\,dx \text{ converges if } p<1, \text{ diverges if } p\ge1$$

## 3. Common mistakes

- **Treating $\infty$ like a number you can "plug in" directly**, instead of properly setting up a limit first.
- **Missing a hidden discontinuity strictly inside the interval.** Always check the *whole* interval, not just the two endpoints — a function like $\frac{1}{x^2}$ blows up at $x=0$ even if $0$ is buried in the middle of an otherwise normal-looking interval like $[-2,2]$.
- **Forgetting that both pieces of a split integral must converge.** If you split at a trouble spot and one piece diverges, the entire original integral diverges — you can't average it out or ignore the bad piece.
- **Sign or limit errors when a term involves a negative exponent approaching $0$ or $\infty$.** Take care tracking whether an expression like $\frac1b$ or $\frac{1}{\sqrt a}$ is heading toward $0$ or blowing up as the boundary variable approaches its target.
- **Confusing "diverges to infinity" with "does not converge" more generally.** Both count as divergence, but it's worth being able to describe which is happening.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int_1^\infty \frac{1}{x^2}\,dx$
2. $\displaystyle\int_1^\infty \frac{1}{x}\,dx$
3. $\displaystyle\int_0^\infty e^{-x}\,dx$
4. $\displaystyle\int_{-\infty}^0 e^{x}\,dx$
5. $\displaystyle\int_1^\infty \frac{1}{x^3}\,dx$
6. $\displaystyle\int_4^\infty \frac{1}{x^{3/2}}\,dx$

### 🟡 Standard

7. $\displaystyle\int_0^1 \frac{1}{x}\,dx$
8. $\displaystyle\int_0^1 \frac{1}{x^2}\,dx$
9. $\displaystyle\int_0^4 \frac{1}{\sqrt{x}}\,dx$
10. $\displaystyle\int_{-\infty}^{\infty} \frac{1}{1+x^2}\,dx$
11. $\displaystyle\int_2^\infty \frac{1}{(x-1)^2}\,dx$
12. $\displaystyle\int_0^3 \frac{1}{3-x}\,dx$

### 🔴 Challenge

13. $\displaystyle\int_0^\infty \frac{1}{1+x^2}\,dx$
14. $\displaystyle\int_1^\infty \frac{1}{x^{3/2}}\,dx$
15. $\displaystyle\int_0^1 \frac{1}{\sqrt{x}}\,dx$
16. $\displaystyle\int_{-1}^{1} \frac{1}{x^{3/4}}\,dx$ (interpret using $|x|^{3/4}$ for real-valued evaluation)
17. $\displaystyle\int_{-2}^2 \frac{1}{x^2}\,dx$ (check the whole interval carefully!)

### 🌍 Applied

18. A drug's concentration decays continuously over an infinite time horizon: $D(t)=D_0e^{-kt}$. Find the total accumulated dose, $\displaystyle\int_0^\infty D(t)\,dt$, in general form, then evaluate it for $D_0=100$ mg and $k=0.2$.
19. Verify that $\displaystyle\int_0^\infty 2e^{-2x}\,dx = 1$ (confirming this models a valid total-probability distribution).
20. Find the present value of a perpetual income stream: $\displaystyle\int_0^\infty 500e^{-0.05t}\,dt$.
21. Find the total work $\displaystyle\int_0^1 \frac{1}{\sqrt{1-x}}\,dx$ done against a force that grows without bound as $x\to1$.
