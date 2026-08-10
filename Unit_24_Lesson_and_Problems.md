# Unit 24: Area and Estimating with Finite Sums

## 1. The idea, in plain words

Here's a question calculus is about to spend a lot of time answering: **how do you find the exact area under a curved graph?** For a straight-edged shape (a rectangle, a triangle), area is easy — you've known those formulas for years. But a curve doesn't have straight edges, so those old formulas don't directly apply.

**The clever fix: approximate the curved region using a bunch of thin rectangles, whose areas you *can* compute exactly, and add them all up.** The more rectangles you use, the thinner each one gets, and the better the jagged "staircase" of rectangle-tops hugs the actual curve. This unit is about building that approximation carefully — this chapter will eventually show how to make the number of rectangles grow without bound, turning the approximation into an exact answer, but for now we're just building the estimating tool itself.

**Picture it like this:** you're trying to measure the area of a oddly-shaped garden bed by laying down a row of rectangular tiles across it. Each tile's height matches the curve at *some* point within its width — but which point you pick (the left edge, the right edge, or the middle) changes your estimate slightly.

**Three common choices for "which point":**

- **Left sum:** use the function's value at the **left edge** of each rectangle's width.
- **Right sum:** use the function's value at the **right edge**.
- **Midpoint sum:** use the function's value at the exact **middle** of each rectangle's width — often the most accurate of the three for the same number of rectangles.

**A useful pattern worth knowing:** if the function is **increasing** across the whole interval, the left sum will always be a bit **too small** (an underestimate), and the right sum will always be a bit **too big** (an overestimate) — because the left edge of each piece is always the *lowest* point on that piece, and the right edge is the *highest*. For a **decreasing** function, this flips: left sum overestimates, right sum underestimates.

## 2. Toolbox

**Setting up the pieces:** to estimate the area under $f(x)$ on $[a,b]$ using $n$ rectangles of equal width:
$$\Delta x = \frac{b-a}{n}$$

This creates $n$ subintervals, with dividing points $x_0=a, x_1, x_2, \dots, x_n=b$ (that's $n+1$ total points, marking off $n$ pieces).

**Left Sum** (use the left endpoint of each subinterval):
$$L_n = \Delta x\big[f(x_0)+f(x_1)+\cdots+f(x_{n-1})\big]$$

**Right Sum** (use the right endpoint of each subinterval):
$$R_n = \Delta x\big[f(x_1)+f(x_2)+\cdots+f(x_n)\big]$$

**Midpoint Sum** (use the midpoint of each subinterval):
$$M_n = \Delta x\big[f(m_1)+f(m_2)+\cdots+f(m_n)\big] \qquad \text{where each } m_i \text{ is the midpoint of its subinterval}$$

**Over/underestimate rules:**

- Increasing function: left sum underestimates, right sum overestimates.
- Decreasing function: left sum overestimates, right sum underestimates.

## 3. Common mistakes

- **Mixing up left and right endpoints.** Always double check: for the left sum, you should never use the very last point $x_n$; for the right sum, you should never use the very first point $x_0$.
- **Forgetting to multiply by $\Delta x$.** Adding up the function values alone gives you the *sum of the heights* — you still need to multiply by the width of each rectangle to get an actual area.
- **Off-by-one errors in counting points.** $n$ subintervals always means $n+1$ total dividing points ($x_0$ through $x_n$) — it's easy to miscount by one.
- **Mixing up which sum over/underestimates.** The rule flips depending on whether the function is increasing or decreasing — always double check by picturing (or sketching) whether the curve is climbing or falling across the interval.
- **Using an endpoint instead of the true midpoint for the midpoint rule.** Take the extra step to actually compute the midpoint of each subinterval — $\dfrac{x_{i-1}+x_i}{2}$ — rather than reusing a left or right endpoint by mistake.

## 4. Problem Set

### 🟢 Warm-up

1. $f(x)=x^2$ on $[0,4]$, $n=4$. Find the **left** sum.
2. $f(x)=x^2$ on $[0,4]$, $n=4$. Find the **right** sum.
3. $f(x)=x+1$ on $[0,4]$, $n=4$. Find the **left** sum.
4. $f(x)=x+1$ on $[0,4]$, $n=4$. Find the **right** sum.
5. $f(x)=x^2$ on $[0,2]$, $n=4$. Find the **left** sum.
6. $f(x)=x^2$ on $[0,2]$, $n=4$. Find the **right** sum.

### 🟡 Standard

7. $f(x)=x^2$ on $[0,4]$, $n=4$. Find the **midpoint** sum.
8. $f(x)=9-x^2$ on $[0,3]$, $n=3$. Find both the left and right sums, and state which one overestimates and which underestimates (based on whether $f$ is increasing or decreasing on this interval).
9. $f(x)=\dfrac1x$ on $[1,5]$, $n=4$. Find the left sum.
10. $f(x)=\sqrt{x}$ on $[0,4]$, $n=4$. Find the right sum.
11. $f(x)=x^2+1$ on $[-1,1]$, $n=4$. Find the midpoint sum.
12. $f(x)=4-x$ on $[0,4]$, $n=4$. Find both the left and right sums, and compare them to the exact area (this region is a triangle, so you can compute its area directly with geometry).

### 🔴 Challenge

13. $f(x)=x^2$ on $[1,3]$, $n=5$. Find the left sum.
14. $f(x)=x^3$ on $[0,2]$, $n=4$. Find the right sum.
15. Explain, using the picture of rectangles under a curve, why the left sum always underestimates and the right sum always overestimates the true area for an **increasing** function on $[a,b]$.
16. $f(x)=\sin x$ on $[0,\pi]$, $n=4$. Find the midpoint sum.
17. For an increasing function on $[0,8]$, a left sum with $n=4$ gives $20$, and a right sum with $n=4$ gives $28$. What can you conclude about the true area? Use the average of the two sums to produce a better single estimate.

### 🌍 Applied

18. A car's velocity (ft/s) is recorded every second: $v(0)=0$, $v(1)=10$, $v(2)=18$, $v(3)=24$, $v(4)=28$. Use a **left** sum (with $\Delta t=1$) to estimate the total distance traveled over $[0,4]$ seconds.
19. Using the same velocity data as Problem 18, use a **right** sum to estimate the distance traveled, and compare it to your left-sum answer.
20. Water flows into a tank, with the flow rate (gal/min) measured every 2 minutes: $r(0)=5$, $r(2)=8$, $r(4)=12$, $r(6)=15$, $r(8)=20$. Use a left sum (with $\Delta t=2$) to estimate the total gallons collected over $[0,8]$ minutes.
21. A company's marginal profit rate (dollars/day) is measured at $t=0,1,2,3$: $P'(0)=100$, $P'(1)=120$, $P'(2)=150$, $P'(3)=180$. Use a right sum to estimate the total profit accumulated over $[0,3]$ days.
