# Cheat Sheet: Which Integration Technique Do I Use?

## How to use this sheet

Don't try to memorize this as a list — use it as a **decision path**. Start at Step 1 and work down. The moment one question fits your integral, stop and use that technique. If nothing seems to fit cleanly, it usually means you need to simplify algebraically first (expand, divide, factor, or use a trig identity) and then run through the steps again.

---

## Step 1: Is it a rational function (a polynomial divided by a polynomial)?

If yes, ask these in order:

**1a.** Does the numerator exactly match (or is a constant multiple of) the derivative of the denominator?

$$\text{Example: } \int \frac{2x-6}{x^2-6x+8}\,dx$$

$\rightarrow$ **Quick substitution.** The answer is just $\ln|\text{denominator}|+C$. No need for anything fancier.

**1b.** Is the numerator's degree *at least* as big as the denominator's degree?

$\rightarrow$ **Do polynomial long division first.** Then re-examine the leftover (smaller) fraction using the rest of this step.

**1c.** Does the denominator factor into linear (or repeated linear) pieces, and the numerator doesn't match 1a?

$$\text{Example: } \int \frac{x+1}{(x-1)(x-2)(x-3)}\,dx$$

$\rightarrow$ **Partial Fractions** (Unit 8.5).

---

## Step 2: Does it contain $\sqrt{a^2-x^2}$, $\sqrt{a^2+x^2}$, or $\sqrt{x^2-a^2}$?

**2a.** Can you complete the square (if it's not already in this exact form) to reveal one of these three shapes?

$$\text{Example: } \int \frac{dx}{\sqrt{-x^2+4x-3}} \rightarrow \int \frac{dx}{\sqrt{1-(x-2)^2}}$$

**2b.** Once in this form: is it a *simple* $\dfrac{1}{\sqrt{a^2-x^2}}$ or $\dfrac{1}{a^2+x^2}$ pattern (nothing else going on)?

$\rightarrow$ **Basic formula** (Unit 8.1) — direct $\arcsin$ or $\arctan$ answer.

**2c.** Is there more going on (a polynomial multiplying the root, or a power of the root itself)?

$$\text{Example: } \int x^2\sqrt{9-x^2}\,dx$$

$\rightarrow$ **Trig Substitution** (Unit 8.4): $x=a\sin\theta$, $x=a\tan\theta$, or $x=a\sec\theta$.

---

## Step 3: Is it a product of two clearly different *kinds* of functions?

(A polynomial times a trig function, a polynomial times $e^x$, a polynomial times $\ln x$ — or a lone $\ln x$, $\arctan x$, or $\arcsin x$ by itself.)

$$\text{Examples: } \int x\sin x\,dx \qquad \int x^5\ln x\,dx \qquad \int \arctan x\,dx$$

$\rightarrow$ **Integration by Parts** (Unit 8.2). Use LIATE to pick $u$: Logarithmic, Inverse trig, Algebraic, Trig, Exponential — whichever type appears earliest in that list becomes $u$.

**Special case:** if it's $e^x$ times $\sin x$ or $\cos x$, you'll need to apply parts *twice* and then solve algebraically for the original integral (a "cyclic" integral).

---

## Step 4: Is it built purely from powers of $\sin$, $\cos$, $\tan$, or $\sec$ of the *same* angle?

(No polynomial mixed in — just trig functions raised to powers.)

$$\text{Examples: } \int \sin^3x\,dx \qquad \int \sin^4x\cos^2x\,dx \qquad \int \sqrt{1+\cos(2x)}\,dx$$

$\rightarrow$ **Trigonometric Integrals** (Unit 8.3):

- If any power is **odd**, peel off one copy and use $\sin^2x+\cos^2x=1$, then substitute.
- If **all** powers are **even**, use the power-reducing identities $\sin^2x=\frac{1-\cos2x}{2}$, $\cos^2x=\frac{1+\cos2x}{2}$.

---

## Step 5: Does it have a "function inside a function," with the inside's derivative sitting right there as a factor?

$$\text{Examples: } \int 2x(x^2+1)^3\,dx \qquad \int \cos x\cdot e^{\sin x}\,dx$$

$\rightarrow$ **$u$-substitution** (Unit 5.5). This is usually the *first* thing to check for simpler integrals — if you spot this pattern early, you can skip straight here without working through Steps 1–4.

---

## If nothing above seems to fit

- Try expanding a product or power that's currently unexpanded.
- Try splitting a fraction into separate terms (dividing each part of the numerator by the denominator).
- Try a trig identity to rewrite the integrand in a friendlier form.
- Then run through the steps again — most integrals become recognizable after one round of simplification.
