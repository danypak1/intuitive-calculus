# Unit 19: Monotonic Functions and the First Derivative Test

## 1. The idea, in plain words

You already know that $f'(x)$ tells you the slope of $f$ at each point. This unit turns that fact into a full map of a function's shape: **where the slope is positive, the graph is climbing (increasing); where the slope is negative, the graph is falling (decreasing).** That's really all "monotonic" means — climbing, or falling, over a stretch of the graph.

**Picture it like a hiking trail again:** if your elevation is always rising as you walk forward, the derivative (your steepness reading) stays positive the whole way. The moment you crest a hill and start heading downhill, your steepness reading flips to negative. **The exact spot where you crest the hill — the transition point — is a critical point,** and it corresponds to a *local maximum*. Cresting a valley (bottoming out and then climbing again) is a *local minimum*.

**The First Derivative Test formalizes exactly this "cresting" idea:** at each critical point, check whether $f'(x)$ switches from positive to negative (a local max — the graph was climbing, now it's falling), switches from negative to positive (a local min — the graph was falling, now it's climbing), or doesn't change sign at all (neither — just a flat "shoulder" where the graph pauses but keeps going the same direction).

**The overall game plan:**

1. Find $f'(x)$.
2. Find all critical points (where $f'(x)=0$ or is undefined).
3. Use the critical points to chop the number line into separate intervals.
4. Pick one test point inside each interval and check the sign of $f'$ there.
5. Positive sign = increasing on that interval; negative sign = decreasing.
6. At each critical point, compare the signs on either side to classify it as a local max, local min, or neither.

## 2. Toolbox

**Increasing/Decreasing Test:**
$$f'(x) > 0 \text{ on an interval} \implies f \text{ is increasing there}$$
$$f'(x) < 0 \text{ on an interval} \implies f \text{ is decreasing there}$$

**First Derivative Test** (for classifying a critical point $c$):

- If $f'$ changes from **positive to negative** at $c$: **local maximum** at $c$.
- If $f'$ changes from **negative to positive** at $c$: **local minimum** at $c$.
- If $f'$ **doesn't change sign** at $c$ (same sign on both sides): **neither** a local max nor min.

**Building a sign chart (the practical tool):** draw a number line, mark every critical point on it, then pick one convenient test value inside each resulting interval and plug it into a **factored** form of $f'(x)$ — factoring makes it easy to read off the sign of each piece without a full computation.

## 3. Common mistakes

- **Testing only some of the intervals, or forgetting an interval entirely.** Every critical point splits the line into one more region — make sure you test all of them.
- **Sign errors when evaluating a factored expression at a test point.** Take it slow: figure out the sign of each individual factor first, then multiply the signs together.
- **Confusing "$f$ is increasing" with "$f'$ is increasing."** These are two completely different statements — this unit is only about the sign of $f'$, not whether $f'$ itself is growing.
- **Forgetting critical points where $f'$ is undefined**, not just where $f'=0$ — a cusp or vertical tangent can still be a local max or min.
- **Mixing up the sign-change directions.** Positive-to-negative is a max (the graph was going up, now down — a peak); negative-to-positive is a min (a valley). It's easy to flip these under pressure — always double check against the "cresting a hill" picture.

## 4. Problem Set

For each problem, find the intervals where $f$ is increasing and decreasing, and classify each critical point as a local max, local min, or neither.

### 🟢 Warm-up

1. $f(x)=x^2-4x+1$
2. $f(x)=-x^2+6x-5$
3. $f(x)=x^3-3x$
4. $f(x)=x^3-12x$
5. $f(x)=x^2+2x-3$
6. $f(x)=2x^3-6x$

### 🟡 Standard

7. $f(x)=x^3-3x^2-9x+5$
8. $f(x)=x^4-4x^3$
9. $f(x)=3x^4-4x^3-12x^2+1$
10. $f(x)=\dfrac{x}{x^2+1}$
11. $f(x)=(x-1)^2(x+2)$
12. $f(x)=x^5-5x$

### 🔴 Challenge

13. $f(x)=x^3-\dfrac32x^2-6x+3$
14. $f(x)=x^{2/3}(x-5)$
15. $f(x)=\sin x+\cos x$ on $[0,2\pi]$
16. $f(x)=x^4-8x^2+3$
17. $f(x)=\dfrac{x^2-4}{x}$

### 🌍 Applied

18. A company's profit (in thousands of dollars) is $P(x)=-x^3+15x^2-48x+10$ for $x\ge0$ units produced. Find where profit is increasing and decreasing, and identify the production level giving a local maximum profit.
19. A population (in thousands) is modeled by $P(t)=-t^3+9t^2+120$ for $t$ in $[0,10]$ years. Find where the population is increasing and decreasing, and identify when it reaches a local maximum.
20. A ball's height (in feet) is modeled by $h(t)=-16t^2+64t+5$. Find where the height is increasing and decreasing, and identify the time of the local maximum height.
21. A greenhouse's temperature (in °F) is modeled by $T(t)=t^3-6t^2+9t+20$ for $t$ in $[0,5]$ hours. Find where the temperature is increasing and decreasing, and identify the local max and local min temperatures.
