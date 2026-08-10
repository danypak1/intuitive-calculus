# Unit 25: Sigma Notation and Limits of Finite Sums

## 1. The idea, in plain words

Last unit, you approximated area using rectangles — and the more rectangles you used, the better the estimate got. This unit gives you two things: **a compact way to write "add up a bunch of terms"** (sigma notation), and **the tool to actually push the number of rectangles to infinity** and get an *exact* answer instead of just an estimate.

**Sigma notation is just shorthand for a sum.** Instead of writing out $1+2+3+4+5$, you can write $\displaystyle\sum_{i=1}^{5} i$ — read "the sum, as $i$ goes from $1$ to $5$, of $i$." The letter $i$ is called the **index**; it starts at the bottom number, increases by $1$ each step, and stops at the top number, plugging into whatever expression sits after the sigma each time.

**Why bother with this notation?** Because a handful of famous formulas let you evaluate huge sums — even sums of thousands of terms — instantly, without writing out a single term. These come in especially handy for one particular use: **writing a Riemann sum with $n$ rectangles using sigma notation, then taking the limit as $n\to\infty$.** When you do that, the jagged rectangle approximation smooths out into the *exact* area under the curve. This is genuinely the formal definition of the definite integral — you're about to compute a few exact areas using nothing but algebra and limits, the hard way, before the next unit hands you a dramatically faster shortcut.

## 2. Toolbox

**Sigma notation:**
$$\sum_{i=1}^{n} a_i = a_1+a_2+a_3+\cdots+a_n$$

**Properties of sums:**
$$\sum_{i=1}^n (a_i+b_i) = \sum_{i=1}^n a_i + \sum_{i=1}^n b_i \qquad \sum_{i=1}^n c\cdot a_i = c\sum_{i=1}^n a_i \qquad \sum_{i=1}^n c = nc \ \text{ (for a constant } c\text{)}$$

**The three key summation formulas** (memorize these — they do all the heavy lifting):
$$\sum_{i=1}^n i = \frac{n(n+1)}{2} \qquad \sum_{i=1}^n i^2 = \frac{n(n+1)(2n+1)}{6} \qquad \sum_{i=1}^n i^3 = \left[\frac{n(n+1)}{2}\right]^2$$

**Building a Riemann sum in sigma notation** (right endpoints), for $f$ on $[a,b]$ with $n$ rectangles:
$$\Delta x = \frac{b-a}{n} \qquad x_i = a+i\Delta x \qquad R_n = \sum_{i=1}^n f(x_i)\,\Delta x$$

**The definite integral, defined as a limit:**
$$\int_a^b f(x)\,dx = \lim_{n\to\infty} \sum_{i=1}^n f(x_i)\,\Delta x$$

**The general strategy for computing an exact area this way:**

1. Write $\Delta x$ and $x_i$ in terms of $n$ and $i$.
2. Build $f(x_i)\cdot\Delta x$ and simplify it into a clean expression involving $i$, $i^2$, and/or $i^3$.
3. Split the sum using the sum properties, and apply the summation formulas to each piece.
4. Simplify the resulting expression (it will be a formula in terms of $n$ alone).
5. Take the limit as $n\to\infty$ — any term with $n$ in the denominator will vanish, leaving the exact area.

## 3. Common mistakes

- **Miscounting the index bounds when expanding a sum.** Double check exactly which values of $i$ are included — from the bottom number all the way through the top number, inclusive.
- **Using the wrong summation formula** — mixing up the formulas for $\sum i$, $\sum i^2$, and $\sum i^3$. Take a moment to check which power of $i$ you actually have before reaching for a formula.
- **Losing track of $\Delta x$ and $x_i$'s dependence on $n$.** Both change as $n$ changes — make sure every $n$ is carried through the algebra correctly before you try to take the limit.
- **Algebra slips when simplifying the messy expression in $n$.** These expressions often have several terms with different powers of $n$ in the denominator — take your time expanding and combining them.
- **Forgetting that terms like $\dfrac{1}{n}$ or $\dfrac{1}{n^2}$ vanish as $n\to\infty$.** This is exactly what makes the final answer collapse down to a clean number — don't accidentally treat $n$ as if it stays finite.

## 4. Problem Set

### 🟢 Warm-up

Expand and evaluate each sum directly.

1. $\displaystyle\sum_{i=1}^{5} i$
2. $\displaystyle\sum_{i=1}^{4} i^2$
3. $\displaystyle\sum_{i=1}^{4} (2i+1)$
4. $\displaystyle\sum_{i=1}^{3} i^3$
5. $\displaystyle\sum_{i=1}^{6} 3$
6. $\displaystyle\sum_{i=1}^{5} (i-1)$

### 🟡 Standard

Use the summation formulas (rather than expanding term by term) to evaluate each sum.

7. $\displaystyle\sum_{i=1}^{10} i$
8. $\displaystyle\sum_{i=1}^{10} i^2$
9. $\displaystyle\sum_{i=1}^{6} i^3$
10. $\displaystyle\sum_{i=1}^{8} (3i-2)$
11. $\displaystyle\sum_{i=1}^{5} (i^2+2i)$
12. $\displaystyle\sum_{i=1}^{20} 5$

### 🔴 Challenge

Use the limit-of-Riemann-sums definition (with right endpoints) to find each exact area.

13. Find the exact area under $f(x)=x^2$ on $[0,3]$.
14. Find the exact area under $f(x)=x$ on $[0,4]$.
15. Find the exact area under $f(x)=2x+1$ on $[0,2]$.
16. Find the exact area under $f(x)=x^2$ on $[1,2]$.
17. Evaluate: $\displaystyle\lim_{n\to\infty} \frac1n\sum_{i=1}^{n} \left(\frac{i}{n}\right)^2$

### 🌍 Applied

18. An object's velocity is $v(t)=2t$ ft/s on $[0,5]$. Use the limit-of-Riemann-sums definition to find the exact total distance traveled.
19. Water flows into a tank at a rate of $r(t)=t^2$ gal/min on $[0,4]$. Use the limit definition to find the exact total gallons collected.
20. A company's marginal revenue is $MR(x)=6x$ dollars per unit on $[0,10]$. Use the limit definition to find the exact total revenue.
21. An object's velocity is $v(t)=3t^2$ ft/s on $[0,4]$. Use the limit definition to find the exact total distance traveled.
