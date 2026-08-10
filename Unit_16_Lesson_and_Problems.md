# Unit 16: Linearization and Differentials

## 1. The idea, in plain words

Here's a neat trick: if you zoom in close enough on any smooth curve, it starts to look just like a straight line — specifically, its tangent line. **This unit is about using that tangent line as a stand-in for the actual curve, to make quick, easy estimates of a function's value near a point you already know well.**

**Picture it like this:** you know $\sqrt{9}=3$ exactly, no calculator needed. But what about $\sqrt{9.3}$? You could reach for a calculator — or you could notice that $9.3$ is *very close* to $9$, and use the tangent line to the curve $y=\sqrt{x}$ at the point $x=9$ as a quick stand-in for the curve itself, right in that neighborhood. Since the tangent line is straight (and easy to compute), it gives you a fast, pretty accurate estimate without any heavy lifting.

**This "stand-in tangent line" has a name: the linearization**, $L(x)$. It's built from information you already know how to find: the function's value at some nearby "nice" point $a$, and the slope there ($f'(a)$).

**A closely related idea: differentials.** Instead of asking "what is $f$ at this new point?", differentials ask a slightly different but related question: "if $x$ changes by a *tiny* amount, roughly how much does $y$ change?" The answer, $dy$, is just the tangent line's *rise* for a given tiny *run*, $dx$. It's the same core idea as linearization, just phrased in terms of a small change rather than a specific new point.

## 2. Toolbox

**Linearization** (the tangent line at $x=a$, used as an approximation for $f(x)$ near $a$):
$$L(x) = f(a) + f'(a)(x-a)$$

**Using it to estimate:** for $x$ close to $a$,
$$f(x) \approx L(x) = f(a)+f'(a)(x-a)$$

**Differentials:** if $dx$ represents a small change in $x$, the corresponding estimated change in $y$ is
$$dy = f'(x)\cdot dx$$

**The key distinction:** $\Delta y$ is the actual, exact change in $y$ (which you'd get by plugging both $x$-values into $f$ and subtracting). $dy$ is the tangent line's *estimate* of that change. When $dx$ is small, $dy \approx \Delta y$ — close, but not usually exactly equal.

**Picking a good point $a$:** always choose a nearby value where $f(a)$ and $f'(a)$ are both easy to compute by hand (a perfect square, a nice round number, an angle you know the trig values for, etc.).

## 3. Common mistakes

- **Evaluating $f'$ at the wrong point.** Always evaluate the derivative at $a$ (the known, nearby point) — not at the target value you're trying to estimate.
- **Getting the sign of $dx$ backward.** If the target value is *smaller* than $a$, then $dx$ is negative — don't forget the negative sign.
- **Forgetting that $L(x)$ is only an estimate, not the exact answer.** It'll be close to the true value for small $dx$, but it isn't meant to be perfectly exact — a bit of difference between the estimate and the true value is expected and normal.
- **Choosing a bad reference point $a$.** If $f(a)$ and $f'(a)$ are hard to compute, the whole point of the technique is lost — always pick the closest "nice" value.
- **Forgetting the units when doing an error/estimation problem** (like estimating volume error from a measurement error) — the differential $dy$ carries the same units as $y$ itself.

## 4. Problem Set

### 🟢 Warm-up

1. Let $f(x)=x^2$. Find the linearization $L(x)$ at $a=3$, then use it to estimate $f(3.1)$.
2. Let $f(x)=x^3$. Find $L(x)$ at $a=2$, then estimate $f(2.05)$.
3. Let $f(x)=\dfrac{1}{x}$. Find $L(x)$ at $a=4$, then estimate $f(4.2)$.
4. Let $f(x)=\sqrt{x}$. Find $L(x)$ at $a=9$, then estimate $f(9.3)$ (i.e., estimate $\sqrt{9.3}$).
5. Let $f(x)=x^2+3x$. Find $L(x)$ at $a=1$, then estimate $f(1.1)$.
6. Let $f(x)=\sqrt{x}$. Find $L(x)$ at $a=25$, then estimate $f(24.7)$ (i.e., estimate $\sqrt{24.7}$).

### 🟡 Standard

7. Let $y=x^3$. Find the differential $dy$ when $x=2$ and $dx=0.1$.
8. Let $y=\sqrt{x}$. Find $dy$ when $x=16$ and $dx=-0.2$.
9. Estimate $\sqrt{50}$ using linearization at $a=49$.
10. Estimate $\sqrt[3]{26}$ using linearization at $a=27$ (i.e., $f(x)=x^{1/3}$).
11. Let $y=\dfrac{1}{x^2}$. Find $dy$ when $x=5$ and $dx=0.05$.
12. Estimate $(3.98)^2$ using linearization at $a=4$.

### 🔴 Challenge

13. A sphere's radius is measured as $10$ cm, with a possible measurement error of $\pm0.1$ cm. Using differentials, estimate the resulting possible error in the computed volume, $V=\dfrac43\pi r^3$.
14. A circle's radius is measured as $5$ cm, with a possible error of $\pm0.05$ cm. Using differentials, estimate the resulting error in the computed area, $A=\pi r^2$, and express it as an approximate percentage error.
15. Let $f(x)=\tan x$. Find $L(x)$ at $a=\dfrac{\pi}{4}$, then use it to estimate $f\left(\dfrac{\pi}{4}+0.01\right)$.
16. Let $f(x)=\sin x$. Find $L(x)$ at $a=0$, then use it to estimate $\sin(0.05)$.
17. A cube's side length is measured as $6$ cm, with a possible error of $\pm0.05$ cm. Using differentials, estimate the resulting error in the computed volume, $V=s^3$, and express it as an approximate percentage error.

### 🌍 Applied

18. A company's cost (in dollars) to produce $x$ units is $C(x)=0.01x^2+5x+200$. Use a differential to estimate the change in cost when production increases from $100$ to $101$ units. Then compute the exact change, $C(101)-C(100)$, and compare.
19. A bacteria population is modeled by $P(t)=500+20t+t^2$. Use a differential to estimate the change in population from $t=10$ to $t=10.2$.
20. A rocket's height (in feet) is modeled by $h(t)=-16t^2+200t+10$. Use a differential to estimate the change in height from $t=3$ to $t=3.1$.
21. A company's revenue (in dollars) is $R(x)=100x-0.5x^2$. Use a differential to estimate the change in revenue when sales increase from $x=50$ to $x=51$. Then compute the exact change, $R(51)-R(50)$, and compare.
