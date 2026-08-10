# Unit 38: Trigonometric Integrals

## 1. The idea, in plain words

Integrals like $\displaystyle\int\sin^3x\,dx$ or $\displaystyle\int\sin^4x\cos^2x\,dx$ look intimidating, but they all fall to one of just **two clean strategies**, depending on whether the powers involved are odd or even.

**Strategy 1 — when at least one power is odd:** "peel off" a single copy of that odd-power function to pair with $dx$ (since it's exactly what you need for a substitution), and convert everything else using the Pythagorean identity $\sin^2x+\cos^2x=1$. Picture it like setting aside one puzzle piece to be your "$du$" and reshaping the rest of the picture using the identity so it's written entirely in terms of the *other* function — which you can then substitute for cleanly.

**Strategy 2 — when both powers are even (so neither can be "peeled off"):** there's no derivative-pair trick available, so instead you use the **power-reducing (half-angle) identities** to trade a squared trig function for a plain cosine of double the angle:
$$\sin^2x = \frac{1-\cos(2x)}{2} \qquad \cos^2x = \frac{1+\cos(2x)}{2}$$
This turns a stubborn power into a simple sum that you can expand and integrate term by term (sometimes needing to apply the identity a second time if a $\cos^2(2x)$ term shows up along the way).

**A related, very satisfying trick: eliminating a square root using a double-angle identity.** Since $1+\cos(2x) = 2\cos^2x$ and $1-\cos(2x)=2\sin^2x$, an integral like $\displaystyle\int\sqrt{1+\cos(2x)}\,dx$ instantly simplifies — the square root and the double angle cancel each other out, leaving just $\sqrt2\,|\cos x|$. **The absolute value matters:** always check the sign of the trig function over your specific interval before dropping it (and if the sign changes partway through, you'll need to split the integral at that point).

## 2. Toolbox

**Pythagorean identity:**
$$\sin^2x+\cos^2x = 1$$

**Power-reducing (half-angle) identities:**
$$\sin^2x = \frac{1-\cos(2x)}{2} \qquad \cos^2x = \frac{1+\cos(2x)}{2}$$

**Strategy for $\displaystyle\int \sin^mx\cos^nx\,dx$:**

- If $m$ (the power on sine) is **odd**: peel off one $\sin x$, convert the remaining even power of sine using $\sin^2x=1-\cos^2x$, then substitute $u=\cos x$.
- If $n$ (the power on cosine) is **odd**: peel off one $\cos x$, convert the remaining even power of cosine using $\cos^2x=1-\sin^2x$, then substitute $u=\sin x$.
- If **both** $m$ and $n$ are even: use the power-reducing identities to rewrite everything in terms of $\cos(2x)$ (and possibly $\cos(4x)$ after a second application), then expand and integrate term by term.

**Eliminating a square root via double angle:**
$$\sqrt{1+\cos(2x)} = \sqrt2\,|\cos x| \qquad \sqrt{1-\cos(2x)} = \sqrt2\,|\sin x|$$

## 3. Common mistakes

- **Reaching for the power-reducing formula when an odd-power shortcut would be much faster.** Always check first: is any power odd? If so, use the peel-off-and-substitute method — it's usually much quicker than expanding with half-angle identities.
- **Sign errors when peeling off an odd power.** For example, $\sin^3x = (1-\cos^2x)\sin x$ — it's easy to drop the parentheses or mishandle the minus sign inside.
- **Mixing up which power-reducing formula goes with which function.** $\sin^2x$ pairs with $\dfrac{1-\cos(2x)}{2}$ (minus sign); $\cos^2x$ pairs with $\dfrac{1+\cos(2x)}{2}$ (plus sign).
- **Forgetting to reduce a leftover $\cos^2(2x)$ term** if it shows up after a first application of the half-angle identity — you may need to apply the identity a second time (this time with $4x$ appearing).
- **Dropping the absolute value carelessly when eliminating a square root**, or forgetting to split the integral at a point where the sign of $\sin x$ or $\cos x$ changes within the interval.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int \sin^3x\,dx$
2. $\displaystyle\int \cos^3x\,dx$
3. $\displaystyle\int \sin x\cos^2x\,dx$
4. $\displaystyle\int \sin^2x\cos x\,dx$
5. $\displaystyle\int \cos^3x\sin x\,dx$
6. $\displaystyle\int \sin^2x\,dx$

### 🟡 Standard

7. $\displaystyle\int \cos^2x\,dx$
8. $\displaystyle\int \sin^3x\cos^2x\,dx$
9. $\displaystyle\int \cos^3x\sin^4x\,dx$
10. $\displaystyle\int \sin^4x\cos x\,dx$
11. $\displaystyle\int \cos^5x\,dx$
12. $\displaystyle\int \sin^4x\,dx$

### 🔴 Challenge

13. $\displaystyle\int \sin^5x\,dx$
14. $\displaystyle\int \sin^6x\cos^3x\,dx$
15. $\displaystyle\int \cos^2x\sin^2x\,dx$
16. $\displaystyle\int_0^{\pi/2} \sqrt{1+\cos(2x)}\,dx$
17. $\displaystyle\int_{-\pi/4}^{\pi/4} \sqrt{1-\cos(2x)}\,dx$ (watch for a sign change within the interval!)

### 🌍 Applied

18. Find $\displaystyle\int_0^{2\pi} \sin^2x\,dx$ (this type of integral shows up when computing average AC power over a full cycle).
19. Find $\displaystyle\int_0^{\pi} \cos^2x\sin x\,dx$.
20. Find $\displaystyle\int_0^{\pi} \sin^3x\,dx$.
21. Find the average value $\dfrac1\pi\displaystyle\int_0^{\pi} \sin^2x\cos^2x\,dx$.
