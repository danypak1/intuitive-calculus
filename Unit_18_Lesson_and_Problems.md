# Unit 18: The Mean Value Theorem

## 1. The idea, in plain words

Imagine you drive $150$ miles in $3$ hours. Your **average speed** for the whole trip is $50$ mph. Now here's a question that sounds obvious once you hear it: at some *exact instant* during that drive, didn't your speedometer have to read *exactly* $50$ mph? Maybe you were going faster at times and slower at others — but somewhere in between, your speed had to pass through $50$ exactly, because that's what "average" means.

**That everyday intuition is the entire Mean Value Theorem (MVT), formalized.** It says: for a smooth, unbroken function over an interval $[a,b]$, there must be *at least one point* in between where the function's **instantaneous rate of change** ($f'(c)$) exactly equals its **average rate of change** over the whole interval.

**Picture it graphically:** draw the secant line connecting the two endpoints $(a,f(a))$ and $(b,f(b))$ — its slope is the average rate of change. The Mean Value Theorem guarantees that somewhere between $a$ and $b$, the curve has a tangent line that is **perfectly parallel** to that secant line. No matter how wiggly the curve is in between, it can't avoid having at least one point where its tangent matches the secant's slope exactly.

**A simpler special case worth knowing: Rolle's Theorem.** If a function starts and ends at the *same height* ($f(a)=f(b)$), then the secant line connecting them is perfectly flat (slope $0$). MVT then guarantees a point in between where the tangent line is also flat — meaning $f'(c)=0$ somewhere in the middle. This makes sense: if you leave from a point and come back to the exact same height, you must have paused or turned around somewhere along the way.

**What you need to be careful about:** MVT only works if the function is **continuous on the closed interval $[a,b]$** and **differentiable on the open interval $(a,b)$**. If either of those breaks down — a hole, a jump, a vertical asymptote, or a sharp corner anywhere in the interval — the theorem's guarantee no longer applies, and you can't assume such a point $c$ exists.

## 2. Toolbox

**Rolle's Theorem:** if $f$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a)=f(b)$, then there exists at least one $c$ in $(a,b)$ such that
$$f'(c) = 0$$

**Mean Value Theorem (MVT):** if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then there exists at least one $c$ in $(a,b)$ such that
$$f'(c) = \frac{f(b)-f(a)}{b-a}$$

**The general procedure to find $c$:**

1. Check that $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$ (for most everyday functions like polynomials, this is automatic — but watch for domain issues with fractions, roots, or corners).
2. Compute the average rate of change: $\dfrac{f(b)-f(a)}{b-a}$.
3. Compute $f'(x)$.
4. Set $f'(x)$ equal to the average rate of change from Step 2, and solve for $x$.
5. Keep only the solution(s) that actually fall **inside the open interval** $(a,b)$ — discard any that fall outside, or that land exactly on an endpoint.

## 3. Common mistakes

- **Forgetting to check the continuity and differentiability hypotheses.** If the function has a break, a hole, an asymptote, or a corner anywhere inside $[a,b]$, MVT simply doesn't apply — you can't use it at all in that case.
- **Keeping a solution for $c$ that falls outside the open interval $(a,b)$**, including one that lands exactly on an endpoint. Only genuine interior solutions count.
- **Expecting a unique answer.** MVT only guarantees *at least one* value of $c$ — sometimes the algebra produces more than one valid solution inside the interval, and all of them are correct.
- **Mixing up Rolle's Theorem's extra condition.** Rolle's Theorem is just MVT in the special case where $f(a)=f(b)$ — don't apply the "$f'(c)=0$" shortcut unless you've actually confirmed the endpoint heights are equal.
- **Sign errors computing the average rate of change.** Double-check the order of subtraction: $\dfrac{f(b)-f(a)}{b-a}$, not the other way around.

## 4. Problem Set

### 🟢 Warm-up

For each problem, verify MVT applies, then find the value(s) of $c$ guaranteed by the theorem.

1. $f(x)=x^2-4x$ on $[0,4]$
2. $f(x)=x^2+2x$ on $[-1,3]$
3. $f(x)=x^3$ on $[0,2]$
4. $f(x)=x^2-1$ on $[1,3]$
5. $f(x)=x^2-4x+3$ on $[1,3]$
6. $f(x)=2x^2-3x$ on $[0,2]$

### 🟡 Standard

7. $f(x)=x^3-3x$ on $[-1,2]$
8. $f(x)=\dfrac1x$ on $[1,3]$
9. $f(x)=x^3-x$ on $[-1,1]$
10. $f(x)=\sqrt{x}$ on $[0,4]$
11. $f(x)=\sin x$ on $[0,\pi]$
12. $f(x)=x^2-6x+5$ on $[0,6]$

### 🔴 Challenge

13. $f(x)=\dfrac1x$ on $[-1,1]$. Explain why the Mean Value Theorem does **not** apply here.
14. $f(x)=|x|$ on $[-2,2]$. Explain why the Mean Value Theorem does **not** apply here.
15. $f(x)=x^3-3x^2+2$ on $[0,3]$. Find all value(s) of $c$ guaranteed by MVT. (Be careful — the algebra may produce a solution that must be discarded.)
16. Suppose $f$ is differentiable everywhere and $f'(x)\le 2$ for every $x$. Suppose also $f(0)=0$ and $f(3)=10$. Use the Mean Value Theorem to show this is impossible — that no such function can exist.
17. A function $f$ is continuous on $[1,5]$ and differentiable on $(1,5)$, with $f(1)=3$ and $f(5)=15$. Use the Mean Value Theorem to show that at some point $c$ in $(1,5)$, $f'(c)=3$, and explain in words why the function's instantaneous rate of change can't stay strictly below $3$ (or strictly above $3$) across the whole interval.

### 🌍 Applied

18. A car travels $150$ miles in $3$ hours. Using the Mean Value Theorem, explain why the car's speedometer must have read exactly $50$ mph at some instant during the trip.
19. A company's profit was $\$200$ at the start of the year ($t=0$) and $\$1400$ at the end ($t=12$ months). Using MVT, show there must have been some moment when the instantaneous rate of profit growth was exactly $\$100$ per month.
20. A runner completes a $10$ km race in exactly $40$ minutes. Using MVT, argue that there must have been some instant during the race when their speed was exactly $15$ km/h.
21. A rocket's height (in feet) satisfies $h(0)=0$ and $h(10)=2000$, where $t$ is measured in seconds. Find the average velocity over this interval, and use MVT to explain why the rocket's instantaneous velocity must equal this value at some moment during the flight.
