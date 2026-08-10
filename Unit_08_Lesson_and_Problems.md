# Unit 8: The Derivative as a Function

## 1. The idea, in plain words

In Unit 7, you computed $f'(a)$ — the slope at one single, specific point. That's a little like measuring the steepness of a hiking trail at just one particular mile marker. This unit asks: **why stop at one point?** Instead of plugging in a fixed number $a$, we keep $x$ as a variable all the way through the computation. What comes out the other end isn't just one number anymore — it's a whole new **function**, $f'(x)$, that tells you the slope at *every single point* at once.

**Picture it:** if $f(x)$ is a hiking trail's elevation, then $f'(x)$ is a second trail map that shows you the steepness at every mile marker, all in one shot. Plug in any $x$-value into $f'(x)$, and out pops the slope of the original trail at exactly that spot — no need to redo the whole limit computation from scratch every time.

**Reading the slope-function off the shape of the graph:** since $f'(x)$ is just "the slope of $f$ at $x$," you can often tell a lot about $f'$ just by looking at a picture of $f$:

- Where $f$ is **going uphill** (increasing), $f'(x)$ is **positive**.
- Where $f$ is **going downhill** (decreasing), $f'(x)$ is **negative**.
- Where $f$ has a **peak or a valley** (a turning point with a flat tangent line), $f'(x) = 0$ right there.

**An important one-way street:** if a function is differentiable at a point, it's guaranteed to also be continuous there — you can't have a well-defined tangent slope at a point where the graph is literally broken. But the reverse isn't true! A function can be perfectly continuous (no breaks) and *still* fail to be differentiable, if it has a sharp corner (like $|x|$ at $x=0$, from Unit 7). So: **differentiable $\Rightarrow$ continuous, but continuous does NOT $\Rightarrow$ differentiable.** This gives you a handy shortcut: if you can show a function *isn't even continuous* somewhere, you instantly know it can't be differentiable there either — no need to compute any derivative limit at all.

## 2. Toolbox

**The general definition** (same formula as Unit 7, but now $x$ stays a variable instead of being replaced by a fixed number):
$$f'(x) = \lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$$

**Notation — these all mean exactly the same thing:**
$$f'(x) \quad = \quad y' \quad = \quad \frac{dy}{dx} \quad = \quad \frac{df}{dx}$$

**The one-way theorem:**
$$\text{differentiable at } a \implies \text{continuous at } a$$
$$\text{(but continuous at } a \text{ does NOT guarantee differentiable at } a\text{)}$$

**Useful shortcut from the theorem (the contrapositive):** if $f$ is **not continuous** at $a$, then $f$ is automatically **not differentiable** at $a$ either — you can stop right there without any further computation.

**Reading a graph:** $f$ increasing $\Leftrightarrow$ $f'>0$; $f$ decreasing $\Leftrightarrow$ $f'<0$; $f$ has a horizontal tangent (peak, valley, or flat spot) $\Leftrightarrow$ $f'=0$.

## 3. Common mistakes

- **Doing the algebra as if $x$ were a specific fixed number.** Since $x$ is now a variable, terms like $x^2$, $2xh$, etc. must stay in the expansion — don't accidentally treat $x$ like a known constant and drop it.
- **Reading "high" as "steep."** A function's *height* on the graph (how big $f(x)$ is) has nothing to do with its *slope* (how big $f'(x)$ is). A function can be very high up but momentarily flat (small $f'$), or low down but very steep (large $f'$).
- **Assuming continuous automatically means differentiable.** Remember, this only goes one direction. Always check separately if you suspect a corner or a break in the tangent behavior.
- **Confusing $\dfrac{dy}{dx}$ with an actual fraction "dy divided by dx."** For now, treat it as a single symbol meaning "the derivative of $y$ with respect to $x$" — it behaves a bit like a fraction later on, but right now it's just notation.
- **Forgetting that once you have the general formula $f'(x)$, you can plug in any point instantly** — there's no need to redo the whole limit computation for every new point you want to evaluate.

## 4. Problem Set

### 🟢 Warm-up

1. Let $f(x)=x^2$. Use the definition to find the general formula for $f'(x)$.
2. Let $f(x)=3x+7$. Use the definition to find $f'(x)$.
3. Let $f(x)=x^2-4x$. Use the definition to find $f'(x)$.
4. Let $f(x)=5-2x^2$. Use the definition to find $f'(x)$.
5. Let $f(x)=x^2+3x-1$. Use the definition to find $f'(x)$, and also write your answer using $\dfrac{dy}{dx}$ notation.
6. Let $f(x)=7$ (a constant function). Use the definition to find $f'(x)$, and explain in plain words why a constant function's derivative is always $0$.

### 🟡 Standard

7. Let $f(x)=x^2-6x+5$. Find $f'(x)$ using the definition. Then evaluate $f'(0)$, $f'(3)$, and $f'(6)$, and describe in words what's happening to the slope of the graph as $x$ increases from $0$ to $6$.
8. Let $f(x)=-x^2+8x$. Find $f'(x)$ using the definition, then find the $x$-value where $f'(x)=0$ (the location of the horizontal tangent).
9. Let $f(x)=x^3$. Use the definition to find $f'(x)$. (You'll need to expand $(x+h)^3$.)
10. You're told that for $f(x)=x^2$, the general derivative formula is $f'(x)=2x$ (matching Problem 1). Without redoing the limit computation, quickly find $f'(5)$, $f'(-3)$, and the slope of the tangent line to $f$ at $x=5$.
11. Let $f(x)=2x^2+3x$. Find $f'(x)$ using the definition, then find all $x$-values where $f'(x)=7$.
12. A graph rises, then reaches a peak, then falls, then reaches a valley, then rises again. Describe, in words, where $f'(x)$ is positive, where it's negative, and where it equals $0$.

### 🔴 Challenge

13. Let $f(x)=\dfrac{1}{x}$. Use the definition to find the general formula for $f'(x)$.
14. Let $f(x)=\sqrt{x}$. Use the definition to find the general formula for $f'(x)$. (You'll need the conjugate trick.)
15. Let $f(x) = \begin{cases} x+1, & x<2 \\ x^2, & x\ge 2\end{cases}$. Using the continuity-differentiability theorem as a shortcut (rather than computing any derivative limit), determine whether $f$ could possibly be differentiable at $x=2$. Explain your reasoning.
16. Let $f(x) = \begin{cases} 3, & x\le 1 \\ 2x+1, & x>1\end{cases}$. First check whether $f$ is continuous at $x=1$. If it is, you'll need to go further and check differentiability directly — do so, and state your conclusion.
17. Let $f(x) = |x| + x^2$. Determine whether $f$ is differentiable at $x=0$ by computing the left-hand and right-hand difference-quotient limits.

### 🌍 Applied

18. A ball is thrown, and its height in meters after $t$ seconds is $h(t) = -5t^2+20t+2$. Find the general velocity function $v(t)=h'(t)$ using the definition. Then use your formula to find the velocity at $t=0$, $t=1$, and $t=2$ seconds, and describe what's physically happening to the ball at each of those moments.
19. A company's revenue (in dollars) from selling $x$ units is $R(x) = 100x-0.5x^2$. Find the general marginal revenue function $R'(x)$ using the definition. Then evaluate $R'(50)$, $R'(100)$, and $R'(150)$, and describe the trend.
20. The number of people who've heard a rumor by day $t$ is modeled by $N(t) = 200t-4t^2$. Find the general rate function $N'(t)$ using the definition. Then evaluate $N'(10)$ and $N'(25)$, and interpret what each number means, including what's special about day $25$.
21. An object's position in meters after $t$ seconds is $s(t) = t^3-3t$. Find the general velocity function $s'(t)$ using the definition. Then evaluate $s'(0)$, $s'(1)$, and $s'(2)$, and describe the object's motion at each moment.
