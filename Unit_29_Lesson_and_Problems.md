# Unit 29: Definite Integral Substitutions and the Area Between Curves

## 1. The idea, in plain words

You now have every tool needed to tackle one of the most natural geometric questions in all of calculus: **what's the area of the region trapped between two curves?**

**Picture it like this:** if one curve sits above another over some stretch of $x$-values, the region between them is like a "ribbon" of varying width. At each $x$-value, the ribbon's height is exactly (top curve) minus (bottom curve). Adding up all those tiny heights across the whole stretch — which is exactly what a definite integral does — gives you the ribbon's total area.

**The game plan:**

1. **Find where the two curves intersect.** Set the two functions equal to each other and solve — these intersection points become your limits of integration (unless the problem already gives you specific bounds).
2. **Figure out which curve is on top** in each region between consecutive intersection points. The easiest way: plug in one test value from that region into both functions and see which one comes out bigger.
3. **Set up the integral** as $\displaystyle\int (\text{top}-\text{bottom})\,dx$ over that region.
4. **Watch out for curves that cross in the middle of your interval.** If the curves swap which one's on top partway through, you can't just integrate straight through — you need to **split the integral at each crossing point**, using the correct (top $-$ bottom) setup in each separate piece, and then add all the pieces together.
5. **Evaluate each piece** using antiderivatives — sometimes needing substitution, exactly like Unit 28.

**A useful sanity check:** area is always positive. If you ever compute a piece and get a negative number, that's a signal you had top and bottom backward for that particular piece — go back and swap them.

## 2. Toolbox

**Area between two curves** (where $f(x)\ge g(x)$ on $[a,b]$):
$$A = \int_a^b \big[f(x)-g(x)\big]\,dx$$

**Finding the bounds when they're not given:** solve $f(x)=g(x)$ for $x$ — the solutions are your intersection points.

**When curves cross inside the interval:** split into separate pieces at each crossing point, using the correct top-minus-bottom setup in each piece, then add the (positive) areas together:
$$A = \int_a^c \big[f(x)-g(x)\big]\,dx + \int_c^b \big[g(x)-f(x)\big]\,dx \quad \text{(if the curves swap order at } x=c\text{)}$$

**Substitution still applies exactly as in Unit 28** whenever the (top $-$ bottom) expression you're integrating has a chain-rule pattern hiding inside it.

## 3. Common mistakes

- **Using the wrong bounds.** Always double-check whether the problem gives you specific bounds, or whether you're meant to find them yourself from the intersection points — these are not always the same thing.
- **Guessing which curve is on top instead of actually testing a point.** Always plug a test value from each sub-region into both functions to be sure.
- **Forgetting to split the integral when the curves cross in the middle of the region.** If you integrate straight through without splitting, positive and negative contributions can partially cancel out, giving you a wrong (usually too-small) answer instead of the true total area.
- **Sign errors in the (top $-$ bottom) subtraction**, especially when one or both functions already have negative terms.
- **Getting a negative "area" and not catching it as a red flag.** A negative result always means the top and bottom were swapped somewhere — go back and fix that piece.

## 4. Problem Set

### 🟢 Warm-up

1. Find the area between $y=x$ and $y=x^2$ on $[0,1]$.
2. Find the area between $y=8-x^2$ and $y=x^2$.
3. Find the area between $y=x^2$ and $y=2x$.
4. Find the area between $y=x+6$ and $y=x^2$.
5. Find the area between $y=4-x^2$ and the x-axis.
6. Find the area between $y=x$ and $y=x^3$ on $[0,1]$.

### 🟡 Standard

7. Find the area between $y=x^2-4$ and $y=4-x^2$.
8. Find the area between $y=x^3$ and $y=4x$. (Watch for a crossing in the middle of the region!)
9. Find the area between $y=\sqrt{x}$ and $y=\dfrac{x}{2}$ on $[0,4]$.
10. Find the area bounded by $y=6x(x^2+1)^2$, the x-axis, $x=0$, and $x=1$.
11. Find the area between $y=x^2+2$ and $y=-x+4$.
12. Find the area between $y=x^3-x$ and the x-axis on $[-1,1]$. (This region needs to be split.)

### 🔴 Challenge

13. Find the area of the region bounded by $y=-x^2+3x$ and $y=2x^3-x^2-5x$.
14. Find the area between $y=x^4-4x^2$ and the x-axis.
15. Find the area between $y=x^3-3x$ and $y=x$. (Watch for a crossing in the middle!)
16. Find the area under $y=x\sqrt{9-x^2}$ from $x=0$ to $x=3$ (using the x-axis as the bottom boundary).
17. Find the area under $y=3x^2(x^3+1)$ from $x=-1$ to $x=1$ (using the x-axis as the bottom boundary).

### 🌍 Applied

18. Company A's revenue rate is $R_A(t)=100+20t$ dollars/week, and Company B's is $R_B(t)=80+15t$ dollars/week, for $t$ in $[0,10]$ weeks. Find the total extra cumulative revenue Company A earns over Company B during this period.
19. Tank 1 fills at a rate of $r_1(t)=5+2t$ gal/min, and Tank 2 fills at a rate of $r_2(t)=3+t$ gal/min, for $t$ in $[0,6]$ minutes. Find how much more water Tank 1 has collected than Tank 2 after $6$ minutes.
20. Runner A's velocity is $v_A(t)=8+0.5t$ mph, and Runner B's velocity is $v_B(t)=7+0.3t$ mph, for $t$ in $[0,4]$ hours. Find the lead (in miles) that Runner A gains over Runner B during this time.
21. Business Strategy A generates profit at a rate of $p_A(x)=50+3x$ dollars/week, and Strategy B generates profit at a rate of $p_B(x)=40+2x$ dollars/week, for $x$ in $[0,20]$ weeks. Find the total additional profit Strategy A generates over Strategy B.
