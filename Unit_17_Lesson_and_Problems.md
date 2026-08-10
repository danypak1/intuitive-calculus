# Unit 17: Extreme Values of Functions on Closed Intervals

## 1. The idea, in plain words

Welcome to Chapter 4 — this is where all those derivative rules you've built up finally start *doing* something practical: finding the highest and lowest points on a graph.

**"Extreme values" just means the highest point (absolute maximum) and lowest point (absolute minimum)** that a function reaches over some interval. Picture a hiking trail with a start and an end point — the absolute max is the highest elevation anywhere along the trail, and the absolute min is the lowest elevation anywhere along it. Crucially, these extreme points can happen in exactly two kinds of places: **at a peak or valley somewhere in the middle of the trail**, or **right at the very start or end of the trail** (the endpoints).

**A guarantee worth knowing (the Extreme Value Theorem):** if a function is continuous (no breaks, no jumps — an unbroken trail) over a *closed* interval $[a,b]$ (meaning the endpoints themselves are included), then it's *guaranteed* to have both an absolute max and an absolute min somewhere on that interval. You don't have to wonder whether they exist — you just have to go find them.

**Where do you look?** Only two kinds of places can ever hold an extreme value:

1. **Critical points** — spots in the middle of the interval where the tangent line is flat ($f'(x)=0$) or where the derivative doesn't exist at all (a corner or cusp).
2. **The endpoints themselves** — $x=a$ and $x=b$.

**The winning strategy (the Closed Interval Method):** rather than trying to reason about which of these candidate points is the actual max or min, just **evaluate $f$ at every single one of them, and directly compare the numbers.** The biggest output is the absolute max; the smallest output is the absolute min. No guessing required — just a plain, direct comparison.

## 2. Toolbox

**Extreme Value Theorem:** if $f$ is continuous on a closed interval $[a,b]$, then $f$ has both an absolute maximum and an absolute minimum somewhere on $[a,b]$.

**Critical point:** a value $c$ in the domain of $f$ where either
$$f'(c)=0 \qquad \text{or} \qquad f'(c) \text{ is undefined}$$

**The Closed Interval Method — the complete procedure:**

1. Find $f'(x)$.
2. Find all critical points of $f$ that lie **inside** the interval $(a,b)$ — solve $f'(x)=0$, and also check for any points where $f'(x)$ is undefined (but $f(x)$ itself is still defined there).
3. Evaluate $f$ at **every** critical point found in Step 2, **and** at both endpoints, $x=a$ and $x=b$.
4. Compare all these output values directly. **The largest one is the absolute maximum; the smallest one is the absolute minimum.**

## 3. Common mistakes

- **Forgetting to check the endpoints.** This is the single most common error in this entire unit — the absolute max or min very often turns out to be sitting right at $x=a$ or $x=b$, not at a critical point at all.
- **Forgetting to check where $f'(x)$ is undefined**, and only solving $f'(x)=0$. A sharp corner or cusp (like in $x^{2/3}$) can absolutely be the location of an extreme value, even though the derivative doesn't exist there.
- **Discarding critical points incorrectly, or keeping ones outside the interval.** Only critical points that actually fall *inside* $[a,b]$ should be checked — solve $f'(x)=0$ first, then filter out any solutions that fall outside the given interval.
- **Assuming a critical point is automatically the max or min.** A critical point only marks a *candidate* location — you must still evaluate $f$ there and compare it against everything else. Some critical points turn out to be neither the max nor the min (just a local wiggle along the way).
- **Arithmetic slips when evaluating $f$ at several different points.** Take your time — a single sign error while plugging in a value can flip your entire final answer.

## 4. Problem Set

For each problem, find the absolute maximum and absolute minimum values of $f$ on the given closed interval, and state the $x$-value(s) where each occurs.

### 🟢 Warm-up

1. $f(x)=x^2-4x+3$ on $[0,5]$
2. $f(x)=x^3-3x$ on $[-2,2]$
3. $f(x)=x^2-6x+8$ on $[-1,4]$
4. $f(x)=x^3-6x^2+9x$ on $[0,5]$
5. $f(x)=x^2+2x-3$ on $[-3,1]$
6. $f(x)=-x^2+4x+1$ on $[0,5]$

### 🟡 Standard

7. $f(x)=x^3-3x^2-9x+5$ on $[-2,4]$
8. $f(x)=x^{2/3}$ on $[-1,8]$
9. $f(x)=x^4-2x^2$ on $[-2,2]$
10. $f(x)=x+\dfrac{1}{x}$ on $[0.5,4]$
11. $f(x)=\sin x+\cos x$ on $[0,\pi]$
12. $f(x)=x^3-12x$ on $[-3,1]$

### 🔴 Challenge

13. $f(x)=\dfrac13x^3-\dfrac32x^2+2x+1$ on $[0,3]$
14. $f(x)=3x^4-4x^3$ on $[-1,2]$
15. $f(x)=x^5-5x$ on $[-2,2]$
16. $f(x)=(x-1)^{2/3}$ on $[-7,9]$
17. $f(x)=2x^3-9x^2+12x+5$ on $[0,3]$

### 🌍 Applied

18. A company's profit (in thousands of dollars) from producing $x$ units is $P(x)=-2x^2+40x-150$, for $x$ in $[0,15]$. Find the production level(s) that give the absolute maximum and absolute minimum profit on this interval.
19. A projectile's height (in feet) $t$ seconds after launch is $h(t)=-16t^2+96t$, for $t$ in $[0,6]$. Find the maximum and minimum height reached during this time interval.
20. The temperature (in °F) $t$ hours after 6 AM is modeled by $T(t)=-t^2+8t+10$, for $t$ in $[0,10]$. Find the maximum and minimum temperature during this period.
21. A factory's cost (in dollars) to produce $x$ units is $C(x)=x^3-15x^2+63x+100$, for $x$ in $[0,10]$. Find the production level(s) that give the absolute maximum and absolute minimum cost on this interval.
