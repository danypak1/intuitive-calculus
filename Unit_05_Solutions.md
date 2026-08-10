# Unit 5: Continuity — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2+3$ at $x=2$.

**Check 1 — is $f(2)$ defined?** $f(2) = 4+3 = 7$. Yes, defined.

**Check 2 — does the limit exist?** Polynomials are smooth everywhere, so $\displaystyle\lim_{x\to 2}f(x) = 2^2+3 = 7$. Yes, exists.

**Check 3 — does the limit equal $f(2)$?** $7 = 7$. Yes.

**Answer: $f$ is continuous at $x=2$.** (This will always be true for polynomials — they're continuous everywhere.)

**2.** $f(x) = \dfrac{x+1}{x-2}$ at $x=0$ and $x=2$.

**At $x=0$:** $f(0) = \dfrac{1}{-2} = -\dfrac12$, defined. Since this is a rational function and the denominator isn't zero at $x=0$, the limit equals $f(0)$ automatically.

**Answer: continuous at $x=0$.**

**At $x=2$:** the denominator becomes $2-2=0$, so $f(2)$ is **undefined**. Condition 1 already fails.

**Answer: discontinuous at $x=2$.** Since the numerator at $x=2$ is $2+1=3 \ne 0$, the function blows up toward $\pm\infty$ near $x=2$ — this is an infinite discontinuity (a vertical asymptote).

**3.** $f(x) = \begin{cases} x+2, & x<1 \\ 4, & x\ge 1\end{cases}$ at $x=1$.

$f(1) = 4$ (defined, using the second piece).

Left-hand limit: $1+2=3$. Right-hand limit: $4$.

Since $3 \ne 4$, the limit does not exist.

**Answer: discontinuous at $x=1$** (condition 2 fails — this is a jump discontinuity).

**4.** $f(x) = \begin{cases} x^2, & x\le 2 \\ 2x, & x>2\end{cases}$ at $x=2$.

$f(2) = 2^2 = 4$ (defined, using the first piece since $x\le 2$ includes $2$).

Left-hand limit: $2^2=4$. Right-hand limit: $2(2)=4$. Both match, so the limit exists and equals $4$.

Compare to $f(2)=4$: they match.

**Answer: $f$ is continuous at $x=2$.** All three conditions check out.

**5.** $f(x) = \begin{cases} 7, & x=0 \\ x^2+3, & x\ne 0\end{cases}$ at $x=0$.

$f(0) = 7$, defined.

The limit uses the "$x\ne 0$" piece (valid on both sides near $0$): $\displaystyle\lim_{x\to 0}(x^2+3) = 0+3=3$. So the limit exists and equals $3$.

Compare to $f(0)=7$: **they do not match** ($3\ne7$).

**Answer: discontinuous at $x=0$.** This is a **removable discontinuity** — the limit exists just fine (it's heading toward $3$), but the function has been deliberately defined to the "wrong" value ($7$) right at that point. Redefining $f(0)=3$ would patch the hole completely.

**6.** $f(x) = \dfrac{1}{x-3}$ at $x=3$.

$f(3)$ would require dividing by $0$, so $f(3)$ is **undefined**.

**Answer: discontinuous at $x=3$.** Since the numerator ($1$) never becomes zero, the function shoots off toward $\pm\infty$ as $x\to 3$ — this is an **infinite discontinuity** (a vertical asymptote at $x=3$).

---

### 🟡 Standard

**7.** $f(x) = \begin{cases} x^2-2x+3, & x<3 \\ 2ax, & x\ge 3\end{cases}$, find $a$ for continuity at $x=3$.

Left-hand limit (use $x^2-2x+3$): $3^2-2(3)+3 = 9-6+3 = 6$.

Right-hand value/limit (use $2ax$): $2a(3) = 6a$.

Set them equal for continuity:

$$6a = 6$$

$$a = 1$$

**Answer: $a=1$.**

**8.** $f(x) = \begin{cases} kx+1, & x<2 \\ x^2-1, & x\ge 2\end{cases}$, find $k$ for continuity at $x=2$.

Left-hand limit: $k(2)+1 = 2k+1$.

Right-hand value: $2^2-1 = 3$.

Set equal:

$$2k+1 = 3$$

$$2k = 2$$

$$k = 1$$

**Answer: $k=1$.**

**9.** $f(x) = \begin{cases} 3x+b, & x\le 1 \\ x^2+2, & x>1\end{cases}$, find $b$ for continuity at $x=1$.

Left-hand value (using the piece that includes $x=1$): $3(1)+b = 3+b$.

Right-hand limit: $1^2+2 = 3$.

Set equal:

$$3+b = 3$$

$$b = 0$$

**Answer: $b=0$.**

**10.** $f(x) = \begin{cases} x^2+4, & x<-1 \\ mx-3, & x\ge -1\end{cases}$, find $m$ for continuity at $x=-1$.

Left-hand limit: $(-1)^2+4 = 1+4 = 5$.

Right-hand value: $m(-1)-3 = -m-3$.

Set equal:

$$-m-3 = 5$$

$$-m = 8$$

$$m = -8$$

**Answer: $m=-8$.**

**11.** $f(x) = \begin{cases} ax^2, & x\le 2 \\ 4x-4, & x>2\end{cases}$, find $a$ for continuity at $x=2$.

Left-hand value: $a(2)^2 = 4a$.

Right-hand limit: $4(2)-4 = 8-4 = 4$.

Set equal:

$$4a = 4$$

$$a = 1$$

**Answer: $a=1$.**

**12.** $f(x) = \begin{cases} x^3, & x<1 \\ c-x, & x\ge 1\end{cases}$, find $c$ for continuity at $x=1$.

Left-hand limit: $1^3 = 1$.

Right-hand value: $c-1$.

Set equal:

$$c-1 = 1$$

$$c = 2$$

**Answer: $c=2$.**

---

### 🔴 Challenge

**13.** $f(x) = \begin{cases} ax+b, & x<0 \\ x^2+1, & 0\le x\le 2 \\ 3x-1, & x>2\end{cases}$, with $f(-2)=7$. Find $a$ and $b$.

**Step 1 — continuity at $x=0$:**

Left-hand limit (use $ax+b$): $a(0)+b = b$.

Value at $x=0$ (use the middle piece, since $0\le x\le 2$ includes $0$): $0^2+1 = 1$.

Set equal: $b = 1$.

**Step 2 — use the extra condition $f(-2)=7$:**

Since $-2<0$, we use the first piece: $f(-2) = a(-2)+b = -2a+b$.

Plug in $b=1$:

$$-2a+1 = 7$$

$$-2a = 6$$

$$a = -3$$

**Bonus check at $x=2$:** middle piece value: $2^2+1=5$. Right-hand limit (use $3x-1$): $3(2)-1=5$. They already match — this breakpoint takes care of itself no matter what $a$ and $b$ are, since neither piece there involves $a$ or $b$.

**Answer: $a=-3$, $b=1$.**

**14.** $f(x) = \begin{cases} \dfrac{x^2-9}{x-3}, & x\ne 3 \\ k, & x=3\end{cases}$, find $k$ for continuity at $x=3$.

The limit (approaching from either side, using the "$x\ne3$" piece) requires factoring first, since plugging in $x=3$ gives $\frac{0}{0}$:

$$\frac{x^2-9}{x-3} = \frac{(x-3)(x+3)}{x-3} = x+3$$

$$\lim_{x\to 3}(x+3) = 6$$

For continuity, we need $f(3)=k$ to match this limit:

$$k = 6$$

**Answer: $k=6$.** This patches the hole that was sitting at $x=3$.

**15.** $f(x) = \begin{cases} \sqrt{x+4}, & x\le 0 \\ 2x+a, & x>0\end{cases}$, find $a$ for continuity at $x=0$.

Left-hand value (use $\sqrt{x+4}$, since $x\le 0$ includes $0$): $\sqrt{0+4} = \sqrt{4} = 2$.

Right-hand limit (use $2x+a$): $2(0)+a = a$.

Set equal:

$$a = 2$$

**Answer: $a=2$.**

**16.** $f(x) = \begin{cases} x+1, & x<2 \\ 5, & x=2 \\ x+3, & x>2\end{cases}$, continuity at $x=2$?

$f(2) = 5$, defined.

Left-hand limit: $2+1 = 3$.

Right-hand limit: $2+3 = 5$.

Since $3 \ne 5$, the two one-sided limits disagree, so the overall limit **does not exist**.

**Answer: $f$ is discontinuous at $x=2$.** This is a **jump discontinuity** — even though $f(2)=5$ happens to match the right-hand side, the left and right limits themselves don't agree with each other, so there's no way to patch this by simply redefining the single point $f(2)$. The two sides are genuinely heading toward different heights.

**17.** $f(x) = \dfrac{1}{(x-4)^2}$, continuity at $x=4$?

$f(4)$ would require dividing by $0$, so it's **undefined** — condition 1 already fails.

**Answer: $f$ is discontinuous at $x=4$.** Since $(x-4)^2$ is always positive and shrinks toward $0$ from both sides as $x\to 4$, the fraction $\frac{1}{(x-4)^2}$ grows without bound toward $+\infty$ on both sides. This is an **infinite discontinuity** (a vertical asymptote at $x=4$).

---

### 🌍 Applied

**18.** $T(x) = \begin{cases} 0.10x, & x\le 50 \\ 0.12x-k, & x>50\end{cases}$, find $k$ for continuity at $x=50$.

Left-hand value: $0.10(50) = 5$.

Right-hand limit: $0.12(50)-k = 6-k$.

Set equal:

$$6-k = 5$$

$$k = 1$$

**Answer: $k=1$.** With this value, the tax owed transitions smoothly across the $x=50$ bracket boundary with no sudden jump.

**19.** $C(w) = \begin{cases} 5+2w, & w\le 3 \\ b+3w, & w>3\end{cases}$, find $b$ for continuity at $w=3$.

Left-hand value: $5+2(3) = 5+6=11$.

Right-hand limit: $b+3(3) = b+9$.

Set equal:

$$b+9 = 11$$

$$b = 2$$

**Answer: $b=2$.** With this value, the shipping price transitions smoothly at $w=3$ pounds.

**20.** $D(x) = \begin{cases} 20, & x\le 1 \\ 20+m(x-1), & x>1\end{cases}$, with $D(5)=52$, find $m$.

Plug $x=5$ into the second piece (since $5>1$):

$$20+m(5-1) = 52$$

$$20+4m = 52$$

$$4m = 32$$

$$m = 8$$

**Answer: $m=8$.**

**Bonus explanation:** continuity at $x=1$ holds automatically for *any* value of $m$, because plugging $x=1$ into the right-hand piece gives $20+m(1-1) = 20+m(0) = 20$ — the $m$ term always vanishes at exactly $x=1$, so the right side always matches the left side's value of $20$ no matter what $m$ turns out to be. That's why we needed a separate piece of information (the cost at $5$ GB) to pin down $m$.

**21.** $T(t) = \begin{cases} 2t+50, & t\le 4 \\ -3t+c, & t>4\end{cases}$, find $c$ for continuity at $t=4$.

Left-hand value: $2(4)+50 = 8+50 = 58$.

Right-hand limit: $-3(4)+c = -12+c$.

Set equal:

$$-12+c = 58$$

$$c = 70$$

**Answer: $c=70$.** With this value, the temperature model transitions smoothly at $t=4$ hours with no sudden jump.
