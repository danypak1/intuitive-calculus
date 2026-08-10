# Unit 5: Continuity

## 1. The idea, in plain words

A function is **continuous** at a point if you could trace its graph through that point without lifting your pencil off the paper. No holes, no sudden jumps, no shooting off to infinity — just a smooth, unbroken path.

In the last unit, we learned to check whether the left-hand and right-hand limits agree. That was step one. Continuity asks one more question on top of that: **does the function's actual value at that point match what it's approaching?**

Here's the full checklist — think of it like a 3-question inspection you run at a single point $x=a$:

1. **Is $f(a)$ actually defined?** (Is there even a dot on the graph there?)
2. **Does the limit exist as $x\to a$?** (Do the left and right limits agree — no jump?)
3. **Does that limit actually equal $f(a)$?** (Does the dot sit exactly where the two sides are heading — no hole, no mismatch?)

If all three answers are "yes," the function is continuous at $a$. If even one fails, it's discontinuous there.

**The three ways continuity can break, pictured:**

- **Removable discontinuity (a hole):** the limit exists just fine, but either $f(a)$ is undefined, or it's defined to some *other* value that doesn't match the limit. Picture an open circle on the curve with a lonely dot sitting somewhere else (or no dot at all). You could "fix" this by simply redefining that one point.
- **Jump discontinuity:** the left and right limits exist but disagree with each other — like a staircase step. No single point-fix can repair this; the two sides are just heading toward different places.
- **Infinite discontinuity:** the function shoots off toward $+\infty$ or $-\infty$ near that point (usually because of a denominator hitting zero without anything canceling it). Picture a vertical asymptote.

## 2. Toolbox

**The continuity checklist at $x=a$:** $f$ is continuous at $a$ if and only if all three hold:

$$\text{1. } f(a) \text{ is defined} \qquad \text{2. } \lim_{x\to a} f(x) \text{ exists} \qquad \text{3. } \lim_{x\to a}f(x) = f(a)$$

**Where continuity usually "just works" automatically:** polynomials are continuous everywhere; rational functions (fractions of polynomials) are continuous everywhere except where the denominator is zero; square roots are continuous everywhere they're defined (inside the domain).

**Solving for an unknown to force continuity at a breakpoint:** set the left-hand piece's value/limit equal to the right-hand piece's value/limit at that breakpoint, then solve the resulting equation for the unknown.

**Classifying a discontinuity:**

- Limit exists, but doesn't match $f(a)$ (or $f(a)$ is undefined) → **removable**
- Left limit $\ne$ right limit → **jump**
- Function blows up toward $\pm\infty$ → **infinite**

## 3. Common mistakes

- **Checking only that the left and right limits agree, and stopping there.** That only confirms the limit *exists* — you still have to check it matches $f(a)$.
- **Forgetting to check that $f(a)$ is even defined in the first place.** A function can't be continuous at a point where there's no dot at all.
- **Assuming a piecewise function is automatically continuous everywhere just because each individual piece is a nice, continuous formula.** You must still separately check every breakpoint where the pieces are glued together.
- **Mixing up removable and jump discontinuities.** A hole (removable) can be patched by redefining one point; a jump cannot, because the two sides are approaching genuinely different values.
- **Sign or algebra slips while solving for the unknown parameter.** These problems usually reduce to a simple one-variable equation — take it slow.

## 4. Problem Set

### 🟢 Warm-up

1. Let $f(x) = x^2+3$. Check whether $f$ is continuous at $x=2$ by verifying all three conditions.
2. Let $f(x) = \dfrac{x+1}{x-2}$. Check continuity at $x=0$ and at $x=2$. Explain what happens at $x=2$.
3. Let $f(x) = \begin{cases} x+2, & x<1 \\ 4, & x\ge 1\end{cases}$. Check continuity at $x=1$.
4. Let $f(x) = \begin{cases} x^2, & x\le 2 \\ 2x, & x>2\end{cases}$. Check continuity at $x=2$.
5. Let $f(x) = \begin{cases} 7, & x=0 \\ x^2+3, & x\ne 0\end{cases}$. Check continuity at $x=0$, and describe what kind of discontinuity (if any) occurs.
6. Let $f(x) = \dfrac{1}{x-3}$. Check continuity at $x=3$, and describe what kind of discontinuity (if any) occurs.

### 🟡 Standard

7. Find the value of $a$ that makes $f$ continuous at $x=3$, where $f(x) = \begin{cases} x^2-2x+3, & x<3 \\ 2ax, & x\ge 3\end{cases}$.
8. Find the value of $k$ that makes $f$ continuous at $x=2$, where $f(x) = \begin{cases} kx+1, & x<2 \\ x^2-1, & x\ge 2\end{cases}$.
9. Find the value of $b$ that makes $f$ continuous at $x=1$, where $f(x) = \begin{cases} 3x+b, & x\le 1 \\ x^2+2, & x>1\end{cases}$.
10. Find the value of $m$ that makes $f$ continuous at $x=-1$, where $f(x) = \begin{cases} x^2+4, & x<-1 \\ mx-3, & x\ge -1\end{cases}$.
11. Find the value of $a$ that makes $f$ continuous at $x=2$, where $f(x) = \begin{cases} ax^2, & x\le 2 \\ 4x-4, & x>2\end{cases}$.
12. Find the value of $c$ that makes $f$ continuous at $x=1$, where $f(x) = \begin{cases} x^3, & x<1 \\ c-x, & x\ge 1\end{cases}$.

### 🔴 Challenge

13. Let $f(x) = \begin{cases} ax+b, & x<0 \\ x^2+1, & 0\le x\le 2 \\ 3x-1, & x>2\end{cases}$. You're also told that $f(-2)=7$. Find $a$ and $b$ so that $f$ is continuous at $x=0$ and satisfies $f(-2)=7$. (As a bonus check, verify what happens at $x=2$.)
14. Let $f(x) = \begin{cases} \dfrac{x^2-9}{x-3}, & x\ne 3 \\ k, & x=3\end{cases}$. Find the value of $k$ that makes $f$ continuous at $x=3$.
15. Let $f(x) = \begin{cases} \sqrt{x+4}, & x\le 0 \\ 2x+a, & x>0\end{cases}$. Find the value of $a$ that makes $f$ continuous at $x=0$.
16. Let $f(x) = \begin{cases} x+1, & x<2 \\ 5, & x=2 \\ x+3, & x>2\end{cases}$. Determine whether $f$ is continuous at $x=2$. If not, classify the discontinuity (removable, jump, or infinite) and explain your reasoning.
17. Let $f(x) = \dfrac{1}{(x-4)^2}$. Determine whether $f$ is continuous at $x=4$. If not, classify the discontinuity and explain your reasoning.

### 🌍 Applied

18. A simplified tax model gives tax owed (in dollars) as $T(x) = \begin{cases} 0.10x, & x\le 50 \\ 0.12x-k, & x>50\end{cases}$, where $x$ is income in thousands. Find the value of $k$ that avoids a sudden jump in tax owed at $x=50$ (i.e., makes $T$ continuous there).
19. A shipping company's cost model is $C(w) = \begin{cases} 5+2w, & w\le 3 \\ b+3w, & w>3\end{cases}$ dollars, where $w$ is weight in pounds. Find the value of $b$ that makes the price transition smoothly (continuously) at $w=3$.
20. A phone data plan costs $D(x) = \begin{cases} 20, & x\le 1 \\ 20+m(x-1), & x>1\end{cases}$ dollars for $x$ gigabytes. You're told that using $5$ GB costs $\$52$. Find $m$. (As a bonus, notice that continuity at $x=1$ holds automatically no matter what $m$ is — explain why, by checking what the right-hand piece gives at $x=1$.)
21. A temperature model is $T(t) = \begin{cases} 2t+50, & t\le 4 \\ -3t+c, & t>4\end{cases}$ degrees, where $t$ is hours after midnight. Find the value of $c$ that avoids a sudden jump in temperature at $t=4$.
