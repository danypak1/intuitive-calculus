# Unit 39: Trigonometric Substitution

## 1. The idea, in plain words

Some integrals hide an expression like $\sqrt{a^2-x^2}$, $\sqrt{a^2+x^2}$, or $\sqrt{x^2-a^2}$ — and no amount of ordinary substitution or algebra will tame that square root. **The fix is a clever trick: replace $x$ with a trig function of a new variable $\theta$, chosen specifically so the square root collapses using the Pythagorean identity.**

**Picture why this works, using the $\sqrt{a^2-x^2}$ case as an example.** If you let $x=a\sin\theta$, then:
$$a^2-x^2 = a^2-a^2\sin^2\theta = a^2(1-\sin^2\theta) = a^2\cos^2\theta$$
Suddenly, the square root of that is just $a\cos\theta$ — clean, no root left at all! The three standard substitutions each target one specific "shape" of expression, chosen so the Pythagorean identity ($\sin^2\theta+\cos^2\theta=1$, or its rearranged cousins) knocks out the square root every time.

**After substituting, you're left with an integral purely in terms of $\theta$** — often one you can handle with the trig integral techniques from Unit 38, or with the classic formula $\displaystyle\int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$ (a standard result worth just remembering, similar to how you memorized the basic trig antiderivatives).

**The last step is always the same: convert your answer back from $\theta$ to $x$.** Since $\theta$ was defined by an equation like $x=a\sin\theta$, you can picture $\theta$ as an angle in a right triangle, and read off whatever other trig ratios you need (like $\cos\theta$ or $\tan\theta$) directly from that triangle — the exact same technique from Unit 35.

## 2. Toolbox

**The three substitution patterns:**

| If you see... | Substitute... | It becomes... |
|---|---|---|
| $\sqrt{a^2-x^2}$ | $x=a\sin\theta$ | $a\cos\theta$ |
| $\sqrt{a^2+x^2}$ | $x=a\tan\theta$ | $a\sec\theta$ |
| $\sqrt{x^2-a^2}$ | $x=a\sec\theta$ | $a\tan\theta$ |

**Don't forget to substitute $dx$ too:**
$$x=a\sin\theta \Rightarrow dx=a\cos\theta\,d\theta \qquad x=a\tan\theta \Rightarrow dx=a\sec^2\theta\,d\theta \qquad x=a\sec\theta \Rightarrow dx=a\sec\theta\tan\theta\,d\theta$$

**A key formula you'll need for the $\tan\theta$ and $\sec\theta$ cases:**
$$\int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

**Converting back from $\theta$ to $x$ — the reference triangle:** draw a right triangle matching the substitution equation (e.g., for $x=a\sin\theta$, since $\sin\theta=\frac{x}{a}$, label opposite $=x$, hypotenuse $=a$; find the missing side with the Pythagorean theorem), then read off whatever ratio you need directly from the triangle.

**The full procedure:**

1. Identify which of the three patterns matches your integral.
2. Substitute for $x$ and $dx$; simplify the square root using the identity.
3. Integrate the resulting expression in $\theta$.
4. Convert the answer back to $x$, using a reference triangle for any leftover trig ratios.

## 3. Common mistakes

- **Choosing the wrong substitution pattern.** Double-check whether you have $a^2-x^2$ (sine), $a^2+x^2$ (tangent), or $x^2-a^2$ (secant) — these are genuinely different shapes and need different substitutions.
- **Forgetting to substitute $dx$ as well as the square root expression.** Both pieces of the integral need to be rewritten in terms of $\theta$.
- **Forgetting to convert the final answer back to $x$.** An answer left in terms of $\theta$ isn't finished — always draw the reference triangle and substitute back.
- **Mislabeling the reference triangle.** Match the sides to the *specific* substitution equation you used (e.g., for $x=a\sec\theta$, secant is hypotenuse-over-adjacent, so hypotenuse $=x$, adjacent $=a$) — mixing this up gives you the wrong ratios.
- **Forgetting the formula for $\int\sec\theta\,d\theta$** and trying to reinvent it from scratch — it's a standard result worth memorizing directly.

## 4. Problem Set

### 🟢 Warm-up

1. Which trig substitution would you use for $\displaystyle\int \frac{dx}{\sqrt{9-x^2}}$?
2. Which trig substitution would you use for $\displaystyle\int \frac{dx}{\sqrt{x^2+16}}$?
3. Which trig substitution would you use for $\displaystyle\int \frac{dx}{\sqrt{x^2-25}}$?
4. $\displaystyle\int \frac{dx}{\sqrt{4-x^2}}$ using $x=2\sin\theta$
5. $\displaystyle\int \frac{dx}{\sqrt{9-x^2}}$ using $x=3\sin\theta$
6. $\displaystyle\int \sqrt{1-x^2}\,dx$ using $x=\sin\theta$

### 🟡 Standard

7. $\displaystyle\int \frac{x^2}{\sqrt{4-x^2}}\,dx$ using $x=2\sin\theta$
8. $\displaystyle\int \frac{dx}{\sqrt{x^2+4}}$ using $x=2\tan\theta$
9. $\displaystyle\int \frac{dx}{\sqrt{x^2+9}}$ using $x=3\tan\theta$
10. $\displaystyle\int \frac{dx}{(x^2+4)^{3/2}}$ using $x=2\tan\theta$
11. $\displaystyle\int \frac{dx}{\sqrt{x^2-4}}$ using $x=2\sec\theta$
12. $\displaystyle\int \frac{dx}{x^2\sqrt{x^2-9}}$ using $x=3\sec\theta$

### 🔴 Challenge

13. $\displaystyle\int \sqrt{9-x^2}\,dx$ using $x=3\sin\theta$
14. $\displaystyle\int x^2\sqrt{9-x^2}\,dx$ using $x=3\sin\theta$
15. $\displaystyle\int \frac{dx}{\sqrt{x^2+16}}$ using $x=4\tan\theta$
16. $\displaystyle\int \frac{dx}{(x^2+9)^{3/2}}$ using $x=3\tan\theta$
17. $\displaystyle\int \frac{dx}{x^2\sqrt{x^2-4}}$ using $x=2\sec\theta$

### 🌍 Applied

18. Find $\displaystyle\int_{-2}^{2} \sqrt{4-x^2}\,dx$, and check your answer against the known area formula for a semicircle.
19. Find $\displaystyle\int_0^3 x^2\sqrt{9-x^2}\,dx$.
20. Find $\displaystyle\int_0^4 \frac{dx}{\sqrt{x^2+16}}$.
21. Find $\displaystyle\int_3^{3\sqrt2} \frac{dx}{x^2\sqrt{x^2-9}}$.
