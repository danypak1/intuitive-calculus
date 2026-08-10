# Unit 27: The Fundamental Theorem of Calculus

## 1. The idea, in plain words

Here's the payoff for everything you've built so far. Back in Units 24–25, computing an exact area meant grinding through a limit of Riemann sums — real work, every single time. **The Fundamental Theorem of Calculus (FTC) says you never have to do that again.** It reveals a stunning, tight connection between the two big ideas of calculus — derivatives and areas — and turns definite integral computation into something you can do in a few lines.

**The Fundamental Theorem has two parts, and they say two different (but related) things.**

**Part 1 — differentiating an integral gives you back the original function.** If you build a new function by integrating $f$ from a fixed starting point up to a *variable* endpoint $x$, then *differentiating that new function* just hands you $f(x)$ right back. Picture it like this: integrating is "accumulating," and differentiating measures "the rate of accumulation" — and the rate at which you're accumulating $f$ is, quite naturally, just $f$ itself. Integration and differentiation are, in a real sense, opposite operations that undo each other.

**Part 2 — the one you'll use constantly — lets you evaluate any definite integral using an antiderivative.** If $F$ is *any* antiderivative of $f$ (found using everything you learned in Unit 23), then:
$$\int_a^b f(x)\,dx = F(b)-F(a)$$
That's it. No limits, no rectangles — just find an antiderivative, plug in the top number, plug in the bottom number, and subtract. **This single fact is why antiderivatives matter so much:** they're not just an abstract "undo the derivative" exercise — they're the literal key that unlocks exact area computation.

## 2. Toolbox

**FTC Part 1** (the derivative of an accumulation function):
$$\frac{d}{dx}\left[\int_a^x f(t)\,dt\right] = f(x)$$

**FTC Part 1, chain rule version** (when the upper limit is itself a function of $x$, not just plain $x$):
$$\frac{d}{dx}\left[\int_a^{g(x)} f(t)\,dt\right] = f\big(g(x)\big)\cdot g'(x)$$

**FTC Part 2 (the Evaluation Theorem)** — the one you'll use most often:
$$\int_a^b f(x)\,dx = F(b)-F(a) = \Big[F(x)\Big]_a^b$$
where $F$ is any antiderivative of $f$ (found using the techniques from Unit 23). Notice: since the constant $+C$ would appear in both $F(b)$ and $F(a)$, it always cancels out during the subtraction — so you can safely ignore it entirely for definite integrals.

**The practical procedure for Part 2:**

1. Find an antiderivative $F(x)$ of $f(x)$ (no need for $+C$).
2. Evaluate $F$ at the top limit, and at the bottom limit.
3. Subtract: (value at top) $-$ (value at bottom).

## 3. Common mistakes

- **Subtracting in the wrong order.** It's always $F(b)-F(a)$ — top limit's value minus bottom limit's value — never the reverse.
- **Forgetting the chain rule when the upper limit of an FTC Part 1 problem isn't plain $x$.** If the upper limit is something like $x^2$ or $\sin x$, you must multiply by the derivative of that upper limit too.
- **Trying to carry a $+C$ through a definite integral evaluation.** It's unnecessary and just adds confusion — the constant always cancels, so leave it out entirely once you're evaluating with specific bounds.
- **Algebra slips when evaluating $F$ at each limit.** Take it slow, especially with fractions or negative numbers — a small arithmetic error here throws off the whole final answer.
- **Not simplifying the integrand first when it's a disguised sum** (like a fraction that splits into several power-rule-friendly pieces) before hunting for the antiderivative.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int_0^2 x^2\,dx$
2. $\displaystyle\int_1^3 (2x+1)\,dx$
3. $\displaystyle\int_0^4 x\,dx$
4. $\displaystyle\int_{-1}^2 3x^2\,dx$
5. $\displaystyle\int_0^1 (x^3+x)\,dx$
6. $\displaystyle\int_1^2 4\,dx$
7. $\displaystyle\int_0^\pi \sin x\,dx$

### 🟡 Standard

8. $\displaystyle\int_0^{\pi/2} \cos x\,dx$
9. $\displaystyle\int_1^4 \sqrt{x}\,dx$
10. $\displaystyle\int_1^2 \frac{1}{x^2}\,dx$
11. $\displaystyle\int_0^2 (x^2-2x+3)\,dx$
12. Find $\dfrac{d}{dx}\left[\displaystyle\int_2^x (t^2+1)\,dt\right]$.
13. Find $\dfrac{d}{dx}\left[\displaystyle\int_0^x \sin t\,dt\right]$.
14. $\displaystyle\int_{-2}^2 x^3\,dx$ (confirm using FTC that this matches what symmetry alone would predict)

### 🔴 Challenge

15. Find $\dfrac{d}{dx}\left[\displaystyle\int_1^{x^2} (t^3+1)\,dt\right]$.
16. Find $\dfrac{d}{dx}\left[\displaystyle\int_0^{\sin x} \sqrt{1+t^2}\,dt\right]$.
17. $\displaystyle\int_1^2 \frac{x^4+x^2}{x^2}\,dx$ (simplify first!)
18. Evaluate $\displaystyle\int_0^3 |x-1|\,dx$ (split into pieces at $x=1$ first).
19. Given $F(x)=\displaystyle\int_0^x (t^2-4)\,dt$, find the critical points of $F(x)$ and classify each as a local max or local min.

### 🌍 Applied

20. A particle's velocity is $v(t)=3t^2-6t$ m/s. Find its displacement (net change in position) over $[0,3]$ using FTC Part 2.
21. Water flows into a tank at a rate of $r(t)=6t+2$ gal/min. Find the total gallons collected over $[0,5]$ minutes using FTC Part 2.
22. A company's marginal cost is $MC(x)=2x+10$. Find the total additional cost of increasing production from $x=5$ to $x=10$ using FTC Part 2.
23. Total distance traveled is modeled by $D(t)=\displaystyle\int_0^t v(s)\,ds$, where $v(s)=4s+1$. Find $D'(t)$ using FTC Part 1, and explain what it represents physically.
