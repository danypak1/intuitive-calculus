# Unit 6: Limits Involving Infinity; Asymptotes of Graphs

## 1. The idea, in plain words

This unit asks two closely related questions:

1. **"What happens to $f(x)$ as $x$ grows forever, in either direction?"** — this is a **limit at infinity**, and it tells us about **horizontal asymptotes**: flat lines the graph flattens out toward (but doesn't necessarily touch) way out on the left or right.
2. **"What happens to $f(x)$ as $x$ approaches some specific number where the function blows up?"** — this connects straight back to the infinite discontinuities from Unit 5, and tells us about **vertical asymptotes**: vertical lines the graph shoots up or down alongside, without ever crossing.

**Picture it:** imagine a graph that, way off to the right, gets flatter and flatter, hugging a horizontal line more and more closely — that flat line is the horizontal asymptote. Now imagine a totally different spot on the same graph where, as you approach one particular $x$-value, the curve rockets straight up (or down) like a rocket ship — that's a vertical asymptote.

**The key trick for limits at infinity with fractions of polynomials:** you can't just "plug in infinity" — infinity isn't a number. Instead, we divide every single term (top and bottom) by the *highest power of $x$ found in the denominator*. Every term that ends up with an $x$ in the bottom (like $\frac{1}{x}$ or $\frac{5}{x^2}$) shrinks to $0$ as $x\to\infty$, since dividing by a bigger and bigger number gives you less and less. What's left tells you the answer instantly.

## 2. Toolbox

**Limits of simple power terms:**
$$\lim_{x\to\infty}\frac{c}{x^n} = 0 \quad \text{for any constant } c \text{ and any } n>0$$

**The three-case rule for rational functions** (fraction of polynomial over polynomial) as $x\to\infty$ or $x\to-\infty$ — compare the **degree** (highest power of $x$) on top versus bottom:

- **Top degree $<$ bottom degree:** the limit is $0$. Horizontal asymptote: $y=0$.
- **Top degree $=$ bottom degree:** the limit is the ratio of the **leading coefficients** (the numbers in front of the highest powers). Horizontal asymptote: $y = \dfrac{\text{leading coeff. of top}}{\text{leading coeff. of bottom}}$.
- **Top degree $>$ bottom degree:** the limit is $+\infty$ or $-\infty$ (the fraction grows without bound). There is no horizontal asymptote in this case.

**How to actually compute it:** divide every term in the numerator and denominator by $x^n$, where $n$ is the highest power appearing in the *denominator*. Then apply $\lim_{x\to\infty}\frac{c}{x^k}=0$ to every leftover fraction term.

**Vertical asymptotes:** for a rational function $\dfrac{P(x)}{Q(x)}$, a vertical asymptote occurs at any $x=a$ where $Q(a)=0$ **and** $P(a)\ne 0$ (the factor causing the zero does *not* cancel out). This is exactly the infinite-discontinuity idea from Unit 5.

**The cancellation trap (important!):** always factor the top and bottom fully *before* deciding on vertical asymptotes. If a factor cancels between the numerator and denominator, that $x$-value is only a **removable hole**, not a vertical asymptote — the graph doesn't blow up there at all.

## 3. Common mistakes

- **Trying to "plug in infinity."** Infinity is not a number you can substitute — always divide by the highest power in the denominator instead.
- **Forgetting to factor before finding vertical asymptotes.** If you skip factoring, you might mistakenly call a removable hole a vertical asymptote (or vice versa).
- **Mixing up which direction the graph shoots — $+\infty$ or $-\infty$.** Check the sign of the expression just barely to the left and just barely to the right of the asymptote separately; they can be different.
- **Assuming top degree $=$ bottom degree always gives a "nice" horizontal asymptote of $1$.** It's the *ratio of leading coefficients*, not automatically $1$ — don't forget to actually read off the coefficients.
- **Forgetting that a graph *can* cross its horizontal asymptote** (just not near $\pm\infty$) — unlike a vertical asymptote, which the graph never touches at all.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\lim_{x\to\infty}\frac{3x+5}{2x-1}$
2. $\displaystyle\lim_{x\to\infty}\frac{2x+1}{x^2+3}$
3. $\displaystyle\lim_{x\to\infty}\frac{x^3+2}{5x^2-1}$
4. $\displaystyle\lim_{x\to-\infty}\frac{4x^2-3}{2x^2+7}$
5. $\displaystyle\lim_{x\to\infty}\frac{5}{x^3}$
6. $\displaystyle\lim_{x\to\infty}\frac{7x^2-2x+1}{3x^2+4x-5}$

### 🟡 Standard

7. $\displaystyle\lim_{x\to\infty}\frac{5x^2+8x-3}{3x^2+2}$
8. Find the horizontal asymptote of $y=\dfrac{2x-7}{x+4}$.
9. Find the horizontal asymptote of $y=\dfrac{3x^2+1}{x^2-5x+6}$.
10. Find the horizontal asymptote of $y=\dfrac{x+2}{x^2-9}$.
11. Find the vertical asymptote(s) of $y=\dfrac{x+1}{x^2-4}$.
12. Find the vertical asymptote(s) of $y=\dfrac{2x}{x^2+x-6}$.

### 🔴 Challenge

13. Find the horizontal **and** vertical asymptotes of $y = \dfrac{(x+3)(x+1)}{(x+2)(x-1)}$.
14. Find the horizontal and vertical asymptotes of $y = \dfrac{(x-2)(x+5)}{(x-2)(x+3)}$. (Watch carefully for a factor that cancels!)
15. Find the horizontal and vertical asymptotes of $y = \dfrac{x^2-1}{x^2-4x+3}$. (Factor everything first.)
16. Find the horizontal and vertical asymptotes of $y = \dfrac{3x^2-12}{x^2-x-2}$.
17. For $y = \dfrac{1}{x-2}$: find the horizontal asymptote, and separately determine whether the graph shoots toward $+\infty$ or $-\infty$ as $x\to 2^-$ and as $x\to 2^+$.

### 🌍 Applied

18. A company's average cost per unit (in dollars) when producing $x$ units is $C(x) = \dfrac{500+3x}{x}$. Find the horizontal asymptote as $x\to\infty$, and explain what it means about the long-run average cost per unit as production grows very large.
19. A drug's concentration in the bloodstream (mg/L) $t$ hours after being administered is modeled by $C(t) = \dfrac{50t}{t^2+25}$. Find the horizontal asymptote as $t\to\infty$, and explain what it means about the drug concentration over a very long time.
20. A city's population (in thousands) $t$ years from now is modeled by $P(t) = \dfrac{200t+500}{t+2}$. Find the horizontal asymptote as $t\to\infty$, and explain what it suggests about the population in the very long run.
21. A factory's production rate (units per hour) as a function of available resources $x$ is modeled by $R(x) = \dfrac{10x}{x+5}$. Find the horizontal asymptote as $x\to\infty$, and explain what it means about the maximum achievable production rate.
