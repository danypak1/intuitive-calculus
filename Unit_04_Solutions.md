# Unit 4: One-Sided Limits — Full Solutions

### 🟢 Warm-up

**1.** $f(x) = \begin{cases} x+1, & x<2 \\ 3x-1, & x\ge 2\end{cases}$

For the left-hand limit, use the piece valid for $x<2$, which is $x+1$:
$$\lim_{x\to 2^-}f(x) = 2+1 = 3$$

For the right-hand limit, use the piece valid for $x\ge 2$, which is $3x-1$:
$$\lim_{x\to 2^+}f(x) = 3(2)-1 = 5$$

Since $3 \ne 5$, the two sides disagree.

**Answer: left limit $=3$, right limit $=5$. The two-sided limit does NOT exist.**

**2.** $f(x) = \begin{cases} x^2, & x<1 \\ 2x-1, & x\ge 1\end{cases}$

Left-hand limit (use $x^2$): $1^2 = 1$.

Right-hand limit (use $2x-1$): $2(1)-1 = 1$.

Both sides give $1$.

**Answer: left limit $=1$, right limit $=1$. The two-sided limit exists and equals $1$.**

**3.** $f(x) = \begin{cases} 3, & x<0 \\ x+3, & x\ge 0\end{cases}$

Left-hand limit (use the constant $3$): $3$.

Right-hand limit (use $x+3$): $0+3=3$.

Both sides give $3$.

**Answer: left limit $=3$, right limit $=3$. The two-sided limit exists and equals $3$.**

**4.** $f(x)=|x|$

For $x<0$: $|x| = -x$, so $\displaystyle\lim_{x\to 0^-} f(x) = -0 = 0$.

For $x\ge 0$: $|x|=x$, so $\displaystyle\lim_{x\to 0^+} f(x) = 0$.

Both sides give $0$.

**Answer: left limit $=0$, right limit $=0$. The two-sided limit exists and equals $0$.**

**5.** $f(x) = \begin{cases} 5-x, & x\le 3 \\ x-1, & x>3\end{cases}$

Left-hand limit (use $5-x$): $5-3 = 2$.

Right-hand limit (use $x-1$): $3-1 = 2$.

Both sides give $2$.

**Answer: left limit $=2$, right limit $=2$. The two-sided limit exists and equals $2$.**

**6.** $f(x) = \begin{cases} 2x, & x<-1 \\ x^2, & x\ge -1\end{cases}$

Left-hand limit (use $2x$): $2(-1) = -2$.

Right-hand limit (use $x^2$): $(-1)^2 = 1$.

Since $-2 \ne 1$, the two sides disagree.

**Answer: left limit $=-2$, right limit $=1$. The two-sided limit does NOT exist.**

---

### 🟡 Standard

**7.** $f(x) = \begin{cases} 1-x^2, & x\ne 1 \\ 2, & x=1\end{cases}$

The piece $1-x^2$ applies for every $x$ near $1$ except exactly at $1$ itself — so it's the correct formula to use approaching from *both* sides.

$$\lim_{x\to 1^-}f(x) = 1-1^2 = 0, \qquad \lim_{x\to 1^+}f(x) = 1-1^2 = 0$$

Both sides give $0$.

**Answer: left limit $=0$, right limit $=0$. The two-sided limit exists and equals $0$.** Notice this is different from $f(1)=2$ — but that's fine, since the limit never cares what the function's actual value is at the point itself.

**8.** $f(x) = \begin{cases} x^2-4, & x\ne 2 \\ 5, & x=2\end{cases}$

The piece $x^2-4$ governs both sides near $x=2$:

$$\lim_{x\to 2^-}f(x) = 2^2-4 = 0, \qquad \lim_{x\to 2^+}f(x) = 2^2-4=0$$

**Answer: left limit $=0$, right limit $=0$. The two-sided limit exists and equals $0$** (again different from $f(2)=5$, which doesn't affect the limit).

**9.** $f(x) = \begin{cases} \dfrac{x^2-9}{x-3}, & x\ne 3 \\ 10, & x=3\end{cases}$

Near $x=3$ (from either side), we use $\dfrac{x^2-9}{x-3}$. Factor the top: $x^2-9=(x-3)(x+3)$, so:

$$\frac{(x-3)(x+3)}{x-3} = x+3 \quad (\text{for } x\ne 3)$$

So both one-sided limits are:

$$\lim_{x\to 3}(x+3) = 3+3 = 6$$

**Answer: $\displaystyle\lim_{x\to 3}f(x) = 6$.** This is different from $f(3)=10$ — the limit describes what the function approaches, not what it's actually defined to equal at that one point.

**10.** $f(x) = \begin{cases} x+2, & x<0 \\ x^2+2, & x\ge 0\end{cases}$

Left-hand limit (use $x+2$): $0+2 = 2$.

Right-hand limit (use $x^2+2$): $0^2+2 = 2$.

**Answer: left limit $=2$, right limit $=2$. The two-sided limit exists and equals $2$.**

**11.** $f(x) = \begin{cases} 3x+2, & x\le -2 \\ -x, & x>-2\end{cases}$

Left-hand limit (use $3x+2$): $3(-2)+2 = -6+2 = -4$.

Right-hand limit (use $-x$): $-(-2) = 2$.

Since $-4 \ne 2$, the sides disagree.

**Answer: left limit $=-4$, right limit $=2$. The two-sided limit does NOT exist.**

**12.** $f(x) = \dfrac{|x-3|}{x-3}$

For $x>3$: $x-3>0$, so $|x-3| = x-3$, giving $f(x) = \dfrac{x-3}{x-3} = 1$.

$$\lim_{x\to 3^+}f(x) = 1$$

For $x<3$: $x-3<0$, so $|x-3| = -(x-3)$, giving $f(x) = \dfrac{-(x-3)}{x-3} = -1$.

$$\lim_{x\to 3^-}f(x) = -1$$

Since $-1 \ne 1$, the sides disagree.

**Answer: left limit $=-1$, right limit $=1$. The two-sided limit does NOT exist.**

---

### 🔴 Challenge

**13.** $f(x) = \begin{cases} x+3, & x<-1 \\ x^2-1, & -1\le x<2 \\ 2x-1, & x\ge 2\end{cases}$

**At $x=-1$:**

Left-hand limit (use $x+3$, valid for $x<-1$): $-1+3 = 2$.

Right-hand limit (use $x^2-1$, valid starting at $-1$): $(-1)^2-1 = 1-1 = 0$.

Since $2 \ne 0$, the limit does **not** exist at $x=-1$.

**At $x=2$:**

Left-hand limit (use $x^2-1$, valid up to but not including $2$): $2^2-1 = 3$.

Right-hand limit (use $2x-1$, valid starting at $2$): $2(2)-1 = 3$.

Since both sides give $3$, the limit **exists** at $x=2$ and equals $3$.

**Answer: at $x=-1$ — left limit $=2$, right limit $=0$, limit DOES NOT exist. At $x=2$ — left limit $=3$, right limit $=3$, limit exists and equals $3$.**

**14.** $f(x) = \begin{cases} \dfrac{x^2-1}{x-1}, & x<1 \\ 3, & x=1 \\ 2x, & x>1\end{cases}$

Left-hand limit: for $x<1$, simplify $\dfrac{x^2-1}{x-1} = \dfrac{(x-1)(x+1)}{x-1} = x+1$ (for $x\ne 1$).

$$\lim_{x\to 1^-}f(x) = 1+1 = 2$$

Right-hand limit (use $2x$): $2(1) = 2$.

Both sides give $2$.

**Answer: left limit $=2$, right limit $=2$. The two-sided limit exists and equals $2$.** This is different from $f(1)=3$ — again, a totally normal and expected mismatch, since the limit doesn't depend on the function's defined value at the point.

**15.** $f(x) = \dfrac{x^2-4}{|x-2|}$

Factor the top for later use: $x^2-4 = (x-2)(x+2)$.

**For $x>2$:** $|x-2| = x-2$, so

$$f(x) = \frac{(x-2)(x+2)}{x-2} = x+2$$

$$\lim_{x\to 2^+}f(x) = 2+2 = 4$$

**For $x<2$:** $|x-2| = -(x-2)$, so

$$f(x) = \frac{(x-2)(x+2)}{-(x-2)} = -(x+2)$$

$$\lim_{x\to 2^-}f(x) = -(2+2) = -4$$

Since $-4 \ne 4$, the sides disagree.

**Answer: left limit $=-4$, right limit $=4$. The two-sided limit does NOT exist.**

**16.** $f(x) = \begin{cases} kx+1, & x<3 \\ x^2-2, & x\ge 3\end{cases}$, find $k$ so the limit exists at $x=3$.

Left-hand limit (use $kx+1$): $k(3)+1 = 3k+1$.

Right-hand limit (use $x^2-2$): $3^2-2 = 7$.

For the limit to exist, the two sides must match:

$$3k+1 = 7$$

$$3k = 6$$

$$k = 2$$

**Answer: $k=2$.**

**17.** $f(x) = \begin{cases} x^2+c, & x\le 2 \\ 3x-4, & x>2\end{cases}$, find $c$ so the limit exists at $x=2$.

Left-hand limit (use $x^2+c$): $2^2+c = 4+c$.

Right-hand limit (use $3x-4$): $3(2)-4 = 2$.

Set them equal:

$$4+c = 2$$

$$c = -2$$

**Answer: $c=-2$.**

---

### 🌍 Applied

**18.** $T(x) = \begin{cases} 0.10x, & x\le 50 \\ 0.12x-1, & x>50\end{cases}$

Left-hand limit (use $0.10x$): $0.10(50) = 5$.

Right-hand limit (use $0.12x-1$): $0.12(50)-1 = 6-1 = 5$.

Both sides give $5$.

**Answer: left limit $=5$, right limit $=5$. The limit exists and equals $5$ — meaning there's no sudden jump in tax owed right at the $x=50$ bracket boundary in this model; the tax owed transitions smoothly across the boundary.**

**19.** $C(w) = \begin{cases} 5, & w\le 2 \\ 5+2(w-2), & w>2\end{cases}$

Left-hand limit (use the constant $5$): $5$.

Right-hand limit (use $5+2(w-2)$): $5+2(2-2) = 5+0 = 5$.

Both sides give $5$.

**Answer: left limit $=5$, right limit $=5$. The limit exists and equals $5$ — there's no price jump right at the $2$-pound mark.**

**20.** $P(h) = \begin{cases} 5, & 0<h\le 1 \\ 8, & 1<h\le 2 \\ 11, & 2<h\le 3\end{cases}$

Left-hand limit at $h=1$ (use the piece valid for $h\le 1$, the constant $5$): $5$.

Right-hand limit at $h=1$ (use the piece valid just above $1$, the constant $8$): $8$.

Since $5 \ne 8$, the sides disagree.

**Answer: left limit $=5$, right limit $=8$. The limit does NOT exist at $h=1$.** This tells you that the moment you cross from $1$ hour into just over $1$ hour, the price suddenly jumps from \$5 to \$8 — a real, sudden jump, unlike the smooth tax and shipping examples above.

**21.** $D(x) = \begin{cases} 30, & x\le 2 \\ 30+10(x-2), & x>2\end{cases}$

Left-hand limit (use the constant $30$): $30$.

Right-hand limit (use $30+10(x-2)$): $30+10(2-2) = 30+0 = 30$.

Both sides give $30$.

**Answer: left limit $=30$, right limit $=30$. The limit exists and equals $30$ — there's no sudden jump in cost right at the $2$ GB mark; the overage charge phases in smoothly from that point.**
