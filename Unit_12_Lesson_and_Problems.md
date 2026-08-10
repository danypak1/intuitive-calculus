# Unit 12: Derivatives of Trig Functions

## 1. The idea, in plain words

Trig functions have their own special derivative formulas — six of them, one for each of the six trig functions. The good news: you don't need to derive these from the limit definition every time (though it can be done, and we'll actually walk through one derivation in this unit just to show it's not magic). You just need to **memorize the six formulas** and then combine them with everything you already know — the sum rule, the product rule, and the quotient rule.

**A helpful mental picture for sine and cosine:** imagine the graph of $\sin x$. Where it's climbing steepest (near $x=0$), $\cos x$ is at its tallest ($\cos 0 = 1$). Where $\sin x$ flattens out at its peak (near $x=\pi/2$), $\cos x$ has dropped to $0$ (flat tangent). The height of the cosine graph, at every point, matches the *steepness* of the sine graph at that same point. That's exactly what "the derivative of $\sin x$ is $\cos x$" means, pictured.

**A quick warning about the minus sign:** the derivative of $\cos x$ is $-\sin x$ — note the negative sign! This trips up almost everyone at some point, so it's worth committing to memory as its own fact, not just "cosine and sine swap."

**Where do the other four formulas come from?** You can actually get all four of them ($\tan x$, $\cot x$, $\sec x$, $\csc x$) using the quotient rule on $\sin x$ and $\cos x$, since $\tan x = \dfrac{\sin x}{\cos x}$, $\sec x = \dfrac{1}{\cos x}$, and so on. You'll walk through one of these derivations yourself in the problem set, just to see that these formulas aren't handed down from nowhere — they're built from tools you already have.

**Important reminder:** all six of these formulas assume $x$ is measured in **radians**, not degrees. Every trig derivative in this course (and in almost all of calculus) uses radians.

## 2. Toolbox

**The six trig derivatives:**
$$\frac{d}{dx}[\sin x] = \cos x \qquad \frac{d}{dx}[\cos x] = -\sin x$$
$$\frac{d}{dx}[\tan x] = \sec^2 x \qquad \frac{d}{dx}[\cot x] = -\csc^2 x$$
$$\frac{d}{dx}[\sec x] = \sec x \tan x \qquad \frac{d}{dx}[\csc x] = -\csc x \cot x$$

**Everything else still applies exactly as before:** the sum/difference rule, the constant multiple rule, the product rule, and the quotient rule all work on trig functions exactly the same way they worked on polynomials.

**Useful identity for simplifying before you differentiate:** $\dfrac{\sin x}{\cos x} = \tan x$. If you see a fraction like this hiding inside a problem, it's often worth converting it to $\tan x$ first — one function is much easier to work with than a fraction of two.

## 3. Common mistakes

- **Forgetting the negative sign on $\cos x$'s derivative.** $\dfrac{d}{dx}[\cos x] = -\sin x$, not $\sin x$. This single sign is the most common error in this whole unit.
- **Mixing up which trig function goes with which derivative.** A common mix-up: writing $\sec x \cdot \sec x$ instead of $\sec x \tan x$ for the derivative of $\sec x$, or forgetting the negative sign on $\cot x$'s and $\csc x$'s derivatives.
- **Forgetting to use the product or quotient rule when a trig function is multiplied by (or divided by) an algebraic expression.** Something like $x\sin x$ or $\dfrac{\sin x}{x}$ still needs the full product or quotient rule — you can't just differentiate the trig part alone.
- **Not simplifying a fraction of $\sin x$ and $\cos x$ before differentiating**, when it could be rewritten as $\tan x$, $\cot x$, $\sec x$, or $\csc x$ first.
- **Forgetting the trig formulas only apply in radians.** If you ever see degrees in a problem, that's a signal something unusual is happening — for this course, always assume radians.

## 4. Problem Set

### 🟢 Warm-up

1. $y = \sin x + \cos x$
2. $y = 3\sin x - 2\cos x$
3. $y = \tan x + 5$
4. $y = 4\cos x - x^2$
5. $y = \sec x + \cot x$
6. $y = 2\csc x - 3\tan x$
7. $y = x + \sin x$

### 🟡 Standard

8. $y = x\sin x$
9. $y = x^2 \cos x$
10. $y = \dfrac{\sin x}{x}$
11. $y = (x+1)\cos x$
12. $y = \dfrac{\tan x}{x}$
13. $y = \sin x \cos x$
14. $y = x\cos x - \sin x$

### 🔴 Challenge

15. $y=(\sin x + \cos x)(x^2+2x)$
16. $y = x^2\sin x + 2x\cos x - 2\sin x$
17. Starting from $\tan x = \dfrac{\sin x}{\cos x}$, use the quotient rule to derive the formula for $\dfrac{d}{dx}[\tan x]$, showing every step (you should end up with $\sec^2 x$, using the identity $\sin^2 x + \cos^2 x = 1$ along the way — remember $\sin^2 x$ just means $(\sin x)^2$, not $\sin(x^2)$).
18. $y = \sec x \tan x$
19. $y = \dfrac{x\sin x}{\cos x}$ (simplify first!)
20. $y = \csc x \cot x$

### 🌍 Applied

21. A pendulum's horizontal displacement (in cm) at time $t$ (seconds) is $x(t) = 5\sin t$. Find the velocity $v(t)=x'(t)$, then evaluate $v(0)$ and $v\left(\dfrac{\pi}{2}\right)$, and describe what's happening physically at each of those two moments.
22. The intensity of sunlight (in some unit) $t$ hours after a reference time is modeled by $I(t) = 100+20\cos t$. Find $I'(t)$, then evaluate $I'\left(\dfrac{\pi}{2}\right)$ and interpret what it means.
23. A Ferris wheel rider's height (in meters) at time $t$ (seconds) is $h(t) = 10+8\sin t$. Find $h'(t)$, then evaluate $h'(0)$ and describe whether the rider is rising or falling at that instant.
24. An electrical signal's voltage (in volts) is modeled by $V(t) = 5\cos t + 2\sin t$. Find $V'(t)$, then evaluate $V'(0)$ and interpret what it means about the voltage at that moment.
