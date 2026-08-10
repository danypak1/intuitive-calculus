# Unit 26: The Definite Integral

## 1. The idea, in plain words

You've now built, from scratch, the machinery for computing exact areas using limits of Riemann sums. This unit takes a step back from the raw computation and asks: **once we know $\displaystyle\int_a^b f(x)\,dx$ represents a signed area, what handy rules follow just from that idea — without needing to grind through a limit every time?**

**A crucial nuance: the definite integral gives *signed*, or *net*, area.** If the curve dips below the x-axis, that portion counts as *negative* area — it doesn't just vanish, and it doesn't add like ordinary area would. Picture a hiker's elevation change: walking uphill counts positive, walking downhill counts negative, and the "total" is the *net* change, not the total distance covered.

**This unit collects a toolkit of properties that let you combine, split, flip, and bound integrals — all without recomputing anything from the limit definition.** Two of these are especially powerful:

**The Max-Min Inequality (bounding an integral without evaluating it):** if you know the smallest value ($m$) and largest value ($M$) that $f$ takes on $[a,b]$, then the exact area has to be squeezed between two easy-to-compute rectangles — one using the shortest possible height, one using the tallest. Picture the true curve trapped between a short flat rectangle underneath it and a tall flat rectangle above it.

**The odd/even symmetry shortcut:** if a function is **odd** (its graph has $180°$ rotational symmetry through the origin) and you integrate it over an interval that's perfectly symmetric around $0$ (like $[-a,a]$), the positive area on one side exactly cancels the negative area on the other — the whole integral collapses to $0$, with zero computation required. If the function is **even** instead (mirror-symmetric across the y-axis), you can cut your work in half by just computing one side and doubling it.

## 2. Toolbox

**Definite integral as signed area:** $\displaystyle\int_a^b f(x)\,dx$ is positive where $f$ is above the x-axis, negative where $f$ is below it.

**Core properties:**
$$\int_a^a f(x)\,dx = 0$$
$$\int_a^b f(x)\,dx = -\int_b^a f(x)\,dx \quad \text{(reversing the limits flips the sign)}$$
$$\int_a^b c\cdot f(x)\,dx = c\int_a^b f(x)\,dx$$
$$\int_a^b \big[f(x)\pm g(x)\big]\,dx = \int_a^b f(x)\,dx \pm \int_a^b g(x)\,dx$$
$$\int_a^b f(x)\,dx + \int_b^c f(x)\,dx = \int_a^c f(x)\,dx \quad \text{(splitting/joining over adjacent intervals)}$$

**Max-Min Inequality:** if $m \le f(x) \le M$ for every $x$ in $[a,b]$, then
$$m(b-a) \le \int_a^b f(x)\,dx \le M(b-a)$$

**Odd/Even symmetry** (only valid on a symmetric interval $[-a,a]$):
$$f \text{ odd } (f(-x)=-f(x)) \implies \int_{-a}^{a} f(x)\,dx = 0$$
$$f \text{ even } (f(-x)=f(x)) \implies \int_{-a}^{a} f(x)\,dx = 2\int_0^a f(x)\,dx$$

**Classifying combinations of odd/even functions** (very useful for the symmetry shortcut):
$$\text{odd}\times\text{odd} = \text{even} \qquad \text{even}\times\text{even} = \text{even} \qquad \text{odd}\times\text{even} = \text{odd}$$
$$\text{odd}+\text{odd} = \text{odd} \qquad \text{even}+\text{even} = \text{even}$$
$$\text{Note: } x^n \text{ is even when } n \text{ is even, and odd when } n \text{ is odd.}$$

## 3. Common mistakes

- **Forgetting the sign flip when reversing the limits of integration.** $\displaystyle\int_b^a f(x)\,dx = -\int_a^b f(x)\,dx$, not the same value.
- **Treating the integral as ordinary (unsigned) area.** Remember: area below the x-axis subtracts from the total, it doesn't add.
- **Using the wrong $m$ and $M$ for the Max-Min Inequality** — these must be the actual minimum and maximum of $f$ *on the given interval*, which usually requires checking whether $f$ is increasing, decreasing, or has a peak/valley inside the interval — not just guessing from the endpoints blindly.
- **Misclassifying a function as odd or even**, especially for products or sums of several pieces. Test methodically: check each piece separately, then combine using the odd/even combination rules.
- **Applying the odd/even shortcut on a non-symmetric interval.** This trick only works when the interval is exactly $[-a,a]$, centered at $0$ — it does not apply to something like $[-1,3]$.

## 4. Problem Set

### 🟢 Warm-up

1. Given $\displaystyle\int_1^4 f(x)\,dx=10$, find $\displaystyle\int_4^1 f(x)\,dx$.
2. Given $\displaystyle\int_0^3 f(x)\,dx=7$, find $\displaystyle\int_0^3 5f(x)\,dx$.
3. Evaluate $\displaystyle\int_2^2 f(x)\,dx$.
4. Given $\displaystyle\int_0^2 f(x)\,dx=4$ and $\displaystyle\int_2^5 f(x)\,dx=9$, find $\displaystyle\int_0^5 f(x)\,dx$.
5. Given $\displaystyle\int_1^3 f(x)\,dx=6$ and $\displaystyle\int_1^3 g(x)\,dx=2$, find $\displaystyle\int_1^3 \big[f(x)-g(x)\big]\,dx$.
6. Given $\displaystyle\int_0^4 f(x)\,dx=8$ and $\displaystyle\int_0^4 g(x)\,dx=3$, find $\displaystyle\int_0^4 \big[2f(x)+3g(x)\big]\,dx$.

### 🟡 Standard

7. Given $\displaystyle\int_0^5 f(x)\,dx=12$ and $\displaystyle\int_3^5 f(x)\,dx=4$, find $\displaystyle\int_0^3 f(x)\,dx$.
8. Given $\displaystyle\int_1^6 f(x)\,dx=20$ and $\displaystyle\int_1^4 f(x)\,dx=9$, find $\displaystyle\int_4^6 f(x)\,dx$.
9. Given $\displaystyle\int_2^7 f(x)\,dx=15$, find $\displaystyle\int_7^2 f(x)\,dx$ and $\displaystyle\int_7^2 \big[-3f(x)\big]\,dx$.
10. If $g(x)=f(x)+2$, explain (using the properties) how $\displaystyle\int_1^5 g(x)\,dx$ compares to $\displaystyle\int_1^5 f(x)\,dx$, and find the exact difference between them.
11. Suppose $f$ is continuous, $f(x)\ge0$ for all $x$ in $[-3,3]$, and $\displaystyle\int_{-3}^3 f(x)\,dx=0$. What can you conclude about $f$ on this interval? Explain your reasoning.
12. Given that $m=2$ and $M=6$ are the minimum and maximum values of $f(x)$ on $[1,4]$, use the Max-Min Inequality to find the best bounds you can state for $\displaystyle\int_1^4 f(x)\,dx$.

### 🔴 Challenge

13. Show that $1 \le \displaystyle\int_0^1 \sqrt{x^2+1}\,dx \le \sqrt2$.
14. Use the Max-Min Inequality to find bounds for $\displaystyle\int_0^2 (x^2+3)\,dx$.
15. Determine, without evaluating the integral directly, whether $\displaystyle\int_{-2}^{2} (x^3-4x)\,dx = 0$. Justify your answer.
16. Determine whether $\displaystyle\int_{-\pi}^{\pi} x^2\cos x\,dx$ can be simplified using symmetry, and explain what the simplification tells you (note: this integral does **not** vanish to zero — explain why not, and what it simplifies to instead).
17. Explain why $\displaystyle\int_{-1}^{1} \left(x^{2024}\sin x + \frac{x^7}{1+x^2}\right)dx = 0$, using odd/even classification for each term — without attempting to actually evaluate any antiderivative.
18. Suppose $2\le f(x)\le 5$ for all $x$ in $[0,6]$, and you're told $\displaystyle\int_0^6 f(x)\,dx=20$. Is this consistent with the Max-Min Inequality? Show your reasoning.

### 🌍 Applied

19. A company's daily profit rate $p(t)$ satisfies $-50\le p(t)\le 200$ for all $t$ in a $30$-day month. Use the Max-Min Inequality to find bounds on the total monthly profit, $\displaystyle\int_0^{30} p(t)\,dt$.
20. A temperature deviation function $d(t)$ (measuring how far the temperature is from the daily average, with $t=0$ representing noon) is modeled as an odd function on $[-6,6]$ (representing 6 AM to 6 PM), based on the assumption that mornings run as far below average as evenings run above it. Find $\displaystyle\int_{-6}^{6} d(t)\,dt$ without further calculation, and interpret what this result means physically.
21. Pump A delivers water at a rate with $\displaystyle\int_0^{10} r(t)\,dt=150$ gallons over $10$ minutes, and Pump B delivers water with $\displaystyle\int_0^{10} s(t)\,dt=90$ gallons over the same period. Find the total combined output, $\displaystyle\int_0^{10} \big[r(t)+s(t)\big]\,dt$.
22. A vehicle's velocity satisfies $40 \le v(t) \le 65$ mph for all $t$ during a $3$-hour trip. Use the Max-Min Inequality to find bounds on the total distance traveled, $\displaystyle\int_0^3 v(t)\,dt$.
