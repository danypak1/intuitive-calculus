# Unit 40: Integration of Rational Functions by Partial Fractions

## 1. The idea, in plain words

You already know how to combine fractions like $\dfrac{1}{x-1}+\dfrac{1}{x+1}$ into a single fraction: $\dfrac{2x}{x^2-1}$. **Partial fractions is that exact process in reverse** — taking one complicated fraction and splitting it back apart into simple pieces that are each easy to integrate on their own.

**Why bother?** A fraction like $\dfrac{2x+6}{(x+1)(x-1)^2}$ has no obvious antiderivative as written. But if you can rewrite it as $\dfrac{A}{x+1}+\dfrac{B}{x-1}+\dfrac{C}{(x-1)^2}$ for the right constants $A$, $B$, $C$, then suddenly you're just integrating three separate, simple pieces — each one either a basic $\ln$ form or a basic power rule form.

**Before doing anything else, always check one thing first: is the numerator's degree *at least* as large as the denominator's?** If so, you can't do partial fractions directly — you have to do **polynomial long division first**, just like dividing $17\div5 = 3$ remainder $2$. This splits your fraction into a plain polynomial part (easy to integrate directly) plus a genuinely smaller "leftover" fraction — and it's only that leftover piece that needs partial fractions.

**A valuable shortcut worth watching for:** sometimes the numerator is *exactly* the derivative of the denominator (or a constant multiple of it). When that happens, you don't need partial fractions at all — a simple substitution gives you a clean $\ln$ answer immediately. Always glance for this pattern before diving into the full decomposition process.

**Setting up the decomposition:**

- **Distinct linear factors**, like $(x-a)(x-b)$: split into $\dfrac{A}{x-a}+\dfrac{B}{x-b}$.
- **A repeated linear factor**, like $(x-a)^2$: you need **both** $\dfrac{A}{x-a}$ **and** $\dfrac{B}{(x-a)^2}$ — not just one term.

**Finding the constants — the fast way:** multiply both sides of your decomposition equation by the full original denominator to clear all fractions. Then, **plug in the value of $x$ that makes each factor zero, one at a time** — this instantly kills off all the other terms and hands you each constant directly.

## 2. Toolbox

**Step 0 (always check first):** if $\deg(\text{numerator}) \ge \deg(\text{denominator})$, perform polynomial long division before anything else. Only the remainder fraction gets decomposed.

**Setting up partial fractions:**
$$\frac{P(x)}{(x-a)(x-b)} = \frac{A}{x-a}+\frac{B}{x-b} \qquad \frac{P(x)}{(x-a)^2(x-b)} = \frac{A}{x-a}+\frac{B}{(x-a)^2}+\frac{C}{x-b}$$

**Solving for constants:** clear the denominators, then plug in each root of the denominator one at a time (the "cover-up" trick) — or, if a constant can't be isolated that way (common with repeated factors), plug in one more convenient value (like $x=0$) and solve the small remaining system.

**Integrating each piece:**
$$\int \frac{A}{x-a}\,dx = A\ln|x-a|+C \qquad \int \frac{A}{(x-a)^2}\,dx = -\frac{A}{x-a}+C$$

**The shortcut to watch for:** if the numerator equals (or is a constant multiple of) the derivative of the denominator, skip decomposition entirely:
$$\int \frac{f'(x)}{f(x)}\,dx = \ln|f(x)|+C$$

## 3. Common mistakes

- **Forgetting to do polynomial long division first** when the numerator's degree is at least the denominator's degree — partial fractions only works correctly on a "proper" fraction (numerator degree strictly less than denominator degree).
- **Setting up a repeated factor incorrectly**, using only $\dfrac{B}{(x-a)^2}$ and forgetting the accompanying $\dfrac{A}{x-a}$ term.
- **Arithmetic slips solving for the constants.** Double-check each one by plugging back into the cleared-denominator equation.
- **Forgetting the absolute value** in $\ln|x-a|$.
- **Missing the derivative-matching shortcut**, and doing a full (unnecessary) partial fraction decomposition when a quick substitution would have worked.
- **Sign errors when clearing denominators or distributing**, especially with three or more factors — write out each step rather than trying to do it in your head.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int \frac{dx}{(x-1)(x+1)}$
2. $\displaystyle\int \frac{dx}{(x-2)(x+3)}$
3. $\displaystyle\int \frac{3x+5}{(x+1)(x+2)}\,dx$
4. $\displaystyle\int \frac{5x-1}{(x-1)(x-3)}\,dx$
5. $\displaystyle\int \frac{dx}{x^2-4}$
6. $\displaystyle\int \frac{x+7}{x^2+x-6}\,dx$ (factor the denominator first!)

### 🟡 Standard

7. $\displaystyle\int \frac{dx}{(x-1)^2(x+1)}$
8. $\displaystyle\int \frac{3x-1}{x^2(x+1)}\,dx$
9. $\displaystyle\int \frac{dx}{(x-1)(x-2)(x-3)}$
10. $\displaystyle\int \frac{2x+1}{(x-2)^2(x+1)}\,dx$
11. Use polynomial long division to rewrite $\dfrac{x^3+2x^2-5}{x+3}$ as a polynomial plus a remainder fraction.
12. $\displaystyle\int \frac{x^2+1}{x-1}\,dx$ (long division needed first!)

### 🔴 Challenge

13. $\displaystyle\int \frac{2x-6}{x^2-6x+8}\,dx$
14. $\displaystyle\int \frac{2x-7}{x^2-7x+12}\,dx$
15. $\displaystyle\int \frac{2x+6}{(x+1)(x-1)^2}\,dx$
16. $\displaystyle\int \frac{x+1}{(x-1)(x-2)(x-3)}\,dx$
17. $\displaystyle\int \frac{x^3+3x^2+2x-7}{x+2}\,dx$

### 🌍 Applied

18. Find $\displaystyle\int \frac{dx}{(x-2)(x-5)}$ (this type of integral arises when solving certain reaction-rate differential equations).
19. Find $\displaystyle\int \frac{dP}{P(100-P)}$ (this is a key building block for solving the logistic growth equation).
20. Find $\displaystyle\int_0^2 \frac{x+3}{(x+1)(x+2)}\,dx$.
21. Find $\displaystyle\int_4^5 \frac{dx}{(x-3)(x-6)}$.
