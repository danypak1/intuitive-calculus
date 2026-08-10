# Unit 1: Rates of Change and Tangent Lines to Curves

## 1. The idea, in plain words

Imagine you drive from home to a friend's house, 60 miles away, and it takes you 2 hours. Your **average speed** is 30 miles per hour. But you didn't drive at exactly 30 mph the whole time — maybe you were stuck at a red light (0 mph) and later flew down the highway (70 mph). Average speed just tells you the overall "big picture" rate, using only the start and the end.

Now imagine glancing at your speedometer at one exact instant. That's your **instantaneous speed** — your speed *right now*, not averaged over the whole trip.

That's the whole idea of this unit:

- **Average rate of change** = comparing two points and asking "how much did y change, divided by how much x changed?" On a graph, this is the slope of the straight line connecting the two points — called a **secant line**.
- **Instantaneous rate of change** = the rate at one single point. On a graph, this is the slope of the line that just barely grazes the curve at that one point — called a **tangent line**.

**Picture it:** Draw a curve. Pick two points on it and connect them with a straight ruler — that's the secant line, and its slope is the average rate of change. Now slide the second point closer and closer to the first point. The ruler keeps tilting until, in the limit, it settles into a line that just kisses the curve at a single point without crossing through it. That final line is the tangent line, and its slope is the instantaneous rate of change.

**How do we actually compute the tangent slope?** We use a trick: pretend the second point is a *tiny* step away from the first, a distance we call $h$. We compute the secant slope using that tiny step, simplify the algebra, and then imagine $h$ shrinking all the way down to $0$. Whatever number the slope settles on is the tangent slope. This is called taking a **limit**, and we'll get more comfortable with limits formally in the next unit — for now, just think of it as "let $h$ shrink to nothing and see what number the slope approaches."

**Quick notation refresher before we dive in:** you're about to see a lot of $f(x)$-style notation, so here's the one-sentence version if it's been a while. $f(x)$ is just a named formula — "$f$ of $x$" — and $f(\text{anything})$ means "take the formula and plug that anything in everywhere you see $x$." So if $f(x)=x^2$, then $f(3)$ means plug in $3$: $f(3)=3^2=9$. And $f(a+h)$ means plug in the whole expression $a+h$ wherever $x$ was: $f(a+h)=(a+h)^2$. Same move every time, no matter how complicated the thing inside the parentheses looks.

## 2. Toolbox

**Average rate of change** of $f$ from $x=a$ to $x=b$ (slope of the secant line):
$$\text{avg rate of change} = \frac{f(b)-f(a)}{b-a}$$

**Difference quotient** (secant slope using a tiny step $h$ away from $x=a$):
$$\frac{f(a+h)-f(a)}{h}$$

**Slope of the tangent line at $x=a$** (let $h$ shrink to $0$):
$$m = \lim_{h\to 0}\frac{f(a+h)-f(a)}{h}$$

**Equation of the tangent line** at the point $(a, f(a))$, once you know the slope $m$:
$$y - f(a) = m(x-a)$$

**Equation of the normal line** (the line perpendicular to the tangent, at the same point): if the tangent slope is $m$, the normal slope is $-\dfrac{1}{m}$:
$$y - f(a) = -\frac{1}{m}(x-a)$$

## 3. Common mistakes

- **Mixing up average and instantaneous rate.** Average rate uses two separate points; instantaneous rate uses a limit at one single point. Read the problem carefully to see which one is being asked for.
- **Plugging in $h=0$ too early.** If you plug $h=0$ into the *original* difference quotient before simplifying, you get $\frac{0}{0}$, which tells you nothing. You must expand and simplify the algebra *first*, cancel the $h$ in the denominator, and only *then* let $h\to 0$.
- **Algebra slips when expanding $f(a+h)$.** This is the #1 source of errors. Take your time expanding things like $(a+h)^2$ or $(2+h)^2$ — write out every term instead of rushing.
- **Forgetting the normal line uses the negative reciprocal.** If the tangent slope is $m$, the normal slope is $-1/m$, not $-m$ and not $1/m$.
- **Losing track of which point you're evaluating at.** Always write down $f(a)$ and $f(a+h)$ clearly before subtracting — don't try to do it all in your head.

## 4. Problem Set

### 🟢 Warm-up

1. Let $f(x) = x^2$. Find the average rate of change of $f$ from $x=1$ to $x=4$.
2. Let $f(x) = 3x + 2$. Find the average rate of change of $f$ from $x=-2$ to $x=5$. (Notice anything about the answer, given that $f$ is a straight line?)
3. Let $f(x) = x^2 - 2x$. Find the average rate of change of $f$ on the interval $[0,3]$.
4. Let $f(x) = \sqrt{x}$. Find the average rate of change of $f$ from $x=1$ to $x=9$.
5. Two points on a curve are $(2,5)$ and $(6,13)$. Find the slope of the secant line through them.
6. Let $f(x) = x^3$. Find the slope of the secant line from $x=1$ to $x=2$.
7. Let $f(x) = \dfrac{1}{x}$. Find the average rate of change of $f$ on $[1,2]$.

### 🟡 Standard

8. Let $f(x) = x^2$. Use the difference quotient $\dfrac{f(a+h)-f(a)}{h}$, simplify, and let $h \to 0$ to find the slope of the tangent line at $x=3$.
9. Let $f(x) = x^2 + 1$. Find the slope of the tangent line at the point $(1,2)$ using the limit definition.
10. Let $f(x) = 2x^2 - 3x$. Find the slope of the tangent line at $x=2$.
11. Let $f(x) = x^2$. Find the equation of the tangent line at $x=-1$.
12. Let $f(x) = -2x^2$. Using the definition, find the slope of the tangent line at $x=1$, then write the equation of the tangent line.
13. Let $f(x) = x^3$. Find the slope of the tangent line at $x=1$.

### 🔴 Challenge

14. Let $f(x) = x^2+1$. Find **both** the tangent line **and** the normal line at the point $(1,2)$.
15. Let $f(x) = x^2 - 4x + 3$. Find the point (or points) where the tangent line is **horizontal**. (Hint: find a general formula for the slope at $x=a$, then set it equal to $0$.)
16. Let $f(x) = x^2$. Find the point where the tangent line has slope $6$.
17. Let $f(x) = \dfrac{1}{x}$. Find the slope of the tangent line at $x=2$ using the difference quotient. (You'll need to combine fractions before you can cancel the $h$.)
18. Let $f(x) = \sqrt{x}$. Find the slope of the tangent line at $x=4$ using the difference quotient. (You'll need to multiply by a conjugate before you can cancel the $h$.)

### 🌍 Applied

19. A ball is thrown, and its height in meters after $t$ seconds is $h(t) = 20t - 5t^2$. Find the **average velocity** from $t=1$ to $t=3$.
20. Using the same height function $h(t) = 20t - 5t^2$, find the **instantaneous velocity** at $t=1$, using the limit definition.
21. A car's position in miles after $t$ hours is $s(t) = t^2 + 2t$. Find the average speed over $[0,2]$, and then find the instantaneous speed at $t=2$.
22. The temperature (in °F) $x$ hours after 6 AM is modeled by $T(x) = -0.1x^2 + 2x + 50$. Find the average rate of change of temperature between hour $2$ and hour $8$. Then find the instantaneous rate of change of temperature at hour $5$.
