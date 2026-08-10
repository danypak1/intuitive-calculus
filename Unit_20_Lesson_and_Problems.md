# Unit 20: Concavity and Curve Sketching

## 1. The idea, in plain words

You already know how to tell whether a graph is climbing or falling using $f'(x)$. This unit adds one more layer of detail: **is the graph curving upward like a cup (concave up), or curving downward like a frown (concave down)?** That extra layer of shape information comes from the **second derivative**, $f''(x)$ — the derivative of the derivative.

**Picture it like this:** a cup holds water — it curves upward, bending away from a straight line underneath it. A frown-shape spills water — it curves downward, bending away from a straight line above it. **Concave up ($f''(x)>0$) looks like a cup; concave down ($f''(x)<0$) looks like a frown.**

**Where the concavity switches from one to the other, that's called an inflection point.** Picture an S-curve: it starts curving one way, then smoothly flips to curving the other way — the exact spot where it flips is the inflection point.

**A bonus tool this unit gives you: the Second Derivative Test.** Instead of always doing a full sign chart with the first derivative to classify a critical point, you can sometimes just check the sign of $f''$ right at that point: a cup-shape ($f''>0$) sitting at a critical point means you're at the bottom of a dip — a local min. A frown-shape ($f''<0$) at a critical point means you're at the top of a hill — a local max. It's often much faster than a full sign chart — but it has a blind spot: if $f''(c)=0$ exactly, the test tells you nothing, and you have to fall back on the first derivative test instead.

**Putting it all together — full curve sketching.** By now you have every tool needed to build a complete, accurate picture of any function's graph without ever plotting a single point by brute force:

- **Domain** — where is the function even defined?
- **Asymptotes** — horizontal and vertical (from Unit 6).
- **$f'(x)$** — where is it increasing/decreasing, and where are the local max/min points?
- **$f''(x)$** — where is it concave up/down, and where are the inflection points?

Combine all four, and you can describe (or sketch) the entire shape of the graph with total confidence.

## 2. Toolbox

**Concavity Test:**
$$f''(x) > 0 \text{ on an interval} \implies f \text{ is concave up there (cup shape)}$$
$$f''(x) < 0 \text{ on an interval} \implies f \text{ is concave down there (frown shape)}$$

**Inflection point:** a point where the concavity **actually changes** — found where $f''(x)=0$ or $f''(x)$ is undefined, **and** the sign of $f''$ genuinely switches on either side (just like critical points, finding a candidate isn't enough — you must confirm the sign actually flips).

**Second Derivative Test** (a shortcut for classifying a critical point $c$ where $f'(c)=0$):

- If $f''(c) > 0$: **local minimum** at $c$ (cup shape — the bottom of a dip).
- If $f''(c) < 0$: **local maximum** at $c$ (frown shape — the top of a hill).
- If $f''(c) = 0$: **the test is inconclusive** — fall back on the First Derivative Test instead.

**The complete curve-sketching checklist:**

1. **Domain** of $f$.
2. **Asymptotes**: horizontal (compare degrees / take limits at $\pm\infty$) and vertical (denominator zero without cancellation).
3. **$f'(x)$**: find critical points, build a sign chart, identify increasing/decreasing intervals and local max/min points.
4. **$f''(x)$**: find candidate inflection points, build a sign chart, identify concave up/down intervals and genuine inflection points.
5. Combine everything into a full description (or sketch) of the graph.

## 3. Common mistakes

- **Mixing up which sign of $f''$ means which shape.** $f''>0$ is concave *up* (cup); $f''<0$ is concave *down* (frown). It's easy to flip these under pressure — the "cup holds water" picture is the fastest way to double-check yourself.
- **Calling every point where $f''=0$ an inflection point, without checking for an actual sign change.** Just like with critical points and extrema, a candidate point isn't automatically the real thing — you must verify concavity genuinely flips on either side.
- **Using the Second Derivative Test when $f''(c)=0$.** This case gives you no information at all — you have to go back to the First Derivative Test for that specific point.
- **Confusing concavity information with increasing/decreasing information.** These come from two *different* derivatives ($f'$ for direction, $f''$ for curviness) — a function can be increasing and concave down at the same time, or decreasing and concave up, and so on. All four combinations are possible.
- **Forgetting to check for asymptotes on a rational function** before finishing a full sketch — a curve-sketching problem involving a fraction almost always has at least a horizontal asymptote to report.

## 4. Problem Set

### 🟢 Warm-up

For each function, find the intervals of concavity and any inflection points.

1. $f(x)=x^3-3x^2+2$
2. $f(x)=x^4-6x^2$
3. $f(x)=x^3-6x^2+9x$
4. $f(x)=-x^3+3x$
5. $f(x)=x^4-4x^3+1$
6. $f(x)=x^3-3x+1$

### 🟡 Standard

7. $f(x)=x^3-6x^2+9x+1$ — use the Second Derivative Test to classify each critical point.
8. $f(x)=x^4-4x^3+2$ — use the Second Derivative Test where possible, and note where it's inconclusive.
9. $f(x)=2x^3-3x^2-12x+5$ — find the inflection point and concavity intervals.
10. $f(x)=x^4-2x^2+3$ — find concavity intervals and inflection points.
11. $f(x)=x^3-3x^2-9x+1$ — use the Second Derivative Test to classify each critical point.
12. $f(x)=3x^5-5x^3$ — find concavity intervals and all inflection points.

### 🔴 Challenge

For Problems 13–17, give a full analysis: domain, asymptotes (if any), increasing/decreasing intervals, local extrema, concavity intervals, and inflection points.

13. $f(x)=-x^3+6x^2-9x+3$
14. $f(x)=\dfrac{(x+1)^2}{1+x^2}$
15. $f(x)=x^4-4x^3+4x^2$
16. $f(x)=(x-2)^3$
17. $f(x)=\dfrac{1}{x^2+1}$

### 🌍 Applied

18. A company's cost (in dollars) is $C(x)=x^3-9x^2+30x+50$. Find the inflection point of the cost curve, and interpret it as the production level where the cost's growth transitions from "increasing at a decreasing rate" (diminishing marginal cost growth) to "increasing at an increasing rate" (accelerating marginal cost growth).
19. A new product's number of users is modeled by $N(t)=-t^3+15t^2+100$ for $t$ in $[0,10]$ months. Find the inflection point, and interpret it as the moment of fastest growth, after which growth continues but begins to slow.
20. An object's position is $s(t)=t^3-6t^2+9t$. Find the inflection point of the position curve, and explain what it tells you about the object's acceleration at that moment (connect this back to the "speeding up/slowing down" ideas from Unit 11).
21. A company's profit is $P(x)=-x^3+12x^2-20x$. Find the inflection point, and interpret it as the production level where returns begin to diminish (marginal profit switches from increasing to decreasing).
