# Unit 35: Inverse Trigonometric Functions

## 1. The idea, in plain words

You already know how to find $\sin(30°)$ — but what about the reverse question: "what angle has a sine of $\dfrac12$?" **That's exactly what inverse trig functions answer.** $\arcsin x$ (also written $\sin^{-1}x$) asks "what angle has this sine value?" and hands back an angle.

**The one tricky wrinkle: since sine, cosine, and tangent repeat their values over and over (infinitely many angles share the same sine), each inverse trig function has to agree on picking just *one* specific angle as "the" answer, out of all the possibilities.** Each one restricts its output to a narrow window, called its **range**:

- $\arcsin x$ always gives an angle in $\left[-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right]$.
- $\arccos x$ always gives an angle in $[0,\pi]$.
- $\arctan x$ always gives an angle in $\left(-\dfrac{\pi}{2}, \dfrac{\pi}{2}\right)$.

**A powerful visual trick for evaluating compositions like $\sin(\arccos x)$:** picture $\theta=\arccos x$ as an actual angle in a right triangle. Since $\cos\theta = \dfrac{\text{adjacent}}{\text{hypotenuse}}$, if $\cos\theta = x$, you can draw a triangle with adjacent side $x$ and hypotenuse $1$ — then the Pythagorean theorem hands you the missing side, and you can read off whatever other trig ratio you need (like $\sin\theta$) directly from the triangle.

**Derivatives of the inverse trig functions** follow their own distinctive patterns — different enough from anything before that they're worth memorizing as a fresh set of formulas, but once memorized, they combine with the chain rule exactly like everything else you've learned.

## 2. Toolbox

**Standard values worth memorizing** (from the familiar $30°$-$45°$-$60°$ angles):
$$\arcsin\left(\frac12\right)=\frac{\pi}{6} \qquad \arcsin\left(\frac{\sqrt2}{2}\right)=\frac{\pi}{4} \qquad \arcsin\left(\frac{\sqrt3}{2}\right)=\frac{\pi}{3}$$
$$\arccos(0)=\frac{\pi}{2} \qquad \arccos\left(\frac12\right)=\frac{\pi}{3} \qquad \arctan(1)=\frac{\pi}{4}$$

**The right-triangle technique for compositions:** to evaluate something like $\sin(\arccos x)$ or $\tan(\arcsin x)$, draw a right triangle where the given ratio matches the inverse function's definition, use the Pythagorean theorem to find the missing side, then read off the requested ratio.

**Derivatives:**
$$\frac{d}{dx}[\arcsin x] = \frac{1}{\sqrt{1-x^2}} \qquad \frac{d}{dx}[\arccos x] = \frac{-1}{\sqrt{1-x^2}} \qquad \frac{d}{dx}[\arctan x] = \frac{1}{1+x^2}$$

**Chain rule versions** (for $u$ instead of plain $x$):
$$\frac{d}{dx}[\arcsin u] = \frac{u'}{\sqrt{1-u^2}} \qquad \frac{d}{dx}[\arccos u] = \frac{-u'}{\sqrt{1-u^2}} \qquad \frac{d}{dx}[\arctan u] = \frac{u'}{1+u^2}$$

## 3. Common mistakes

- **Forgetting the restricted range.** $\arcsin x$ never returns an angle outside $\left[-\frac{\pi}{2},\frac{\pi}{2}\right]$, even though sine itself repeats — always double-check your answer actually falls in the correct window.
- **Sign errors when reading a triangle for a negative input.** If $\arcsin x$ has a negative input, the angle is negative (in the fourth-quadrant-like part of its range) — track carefully which sides of the triangle should be positive or negative based on the specific inverse function's range.
- **Mixing up the three derivative formulas**, especially the sign difference between $\arcsin$ and $\arccos$, and the "$1+x^2$" pattern unique to $\arctan$ (no square root involved there, unlike the other two).
- **Forgetting the chain rule multiplier $u'$** when the input isn't plain $x$.
- **Forgetting the domain restriction on $\arcsin$ and $\arccos$** — their inputs must stay within $[-1,1]$.

## 4. Problem Set

### 🟢 Warm-up

1. Find $\arcsin\left(\dfrac12\right)$.
2. Find $\arccos(0)$.
3. Find $\arctan(1)$.
4. Find $\arcsin\left(-\dfrac{\sqrt2}{2}\right)$.
5. Find $\arccos(1)$.
6. State the formula for $\dfrac{d}{dx}[\arcsin x]$.
7. State the formula for $\dfrac{d}{dx}[\arctan x]$.

### 🟡 Standard

8. Find $\sin\big(\arccos\left(\tfrac35\right)\big)$.
9. Find $\cos\big(\arcsin\left(\tfrac{5}{13}\right)\big)$.
10. Find $\tan\big(\arcsin\left(\tfrac13\right)\big)$.
11. Find $\dfrac{d}{dx}\big[\arcsin(2x)\big]$.
12. Find $\dfrac{d}{dx}\big[\arctan(x^2)\big]$.
13. Find $\dfrac{d}{dx}\big[\arccos(3x)\big]$.
14. Find $\sec\big(\arctan(2)\big)$.

### 🔴 Challenge

15. $y=\arctan(\sin x)$. Find $\dfrac{dy}{dx}$.
16. Find $\sin\left(\arccos\left(\dfrac{\sqrt2}{2}\right)\right)$.
17. Find $\tan\left(\arcsin\left(-\dfrac12\right)\right)$.
18. Find $\dfrac{d}{dx}\Big[x\arcsin(x) + \sqrt{1-x^2}\Big]$.
19. Find $\cos\big(\arctan\left(\tfrac34\right)\big)$.

### 🌍 Applied

20. A ladder leans against a wall, reaching $15$ ft up with its base $8$ ft from the wall. Find the angle of elevation $\theta = \arctan\left(\dfrac{15}{8}\right)$, in degrees.
21. A camera tracks an object's horizontal distance $x(t)$ (in feet) from a fixed point, with the tracking angle given by $\theta(t)=\arctan\left(\dfrac{x(t)}{50}\right)$. At the moment $x=30$ ft and $\dfrac{dx}{dt}=10$ ft/s, find $\dfrac{d\theta}{dt}$.
22. A viewing angle is modeled by $\theta = \arcsin\left(\dfrac{x}{10}\right)$. Find $\dfrac{d\theta}{dx}$, then evaluate it at $x=6$.
23. A ship has traveled $3$ miles east and is currently $5$ miles from its starting point. Its bearing angle from the starting direction is $\theta = \arccos\left(\dfrac{3}{5}\right)$. Find $\theta$ in degrees.
