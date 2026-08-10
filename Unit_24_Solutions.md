# Unit 24: Area and Estimating with Finite Sums — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2$ on $[0,4]$, $n=4$, left sum.

$\Delta x = \dfrac{4-0}{4}=1$. Left endpoints: $x=0,1,2,3$. Function values: $f(0)=0$, $f(1)=1$, $f(2)=4$, $f(3)=9$.

$$L_4 = 1\times(0+1+4+9) = 14$$

**$L_4=14$.**

**2.** Same setup, right sum.

Right endpoints: $x=1,2,3,4$. Function values: $f(1)=1$, $f(2)=4$, $f(3)=9$, $f(4)=16$.

$$R_4 = 1\times(1+4+9+16) = 30$$

**$R_4=30$.**

**3.** $f(x)=x+1$ on $[0,4]$, $n=4$, left sum.

$\Delta x=1$. Left endpoints: $0,1,2,3$. Values: $1,2,3,4$.

$$L_4 = 1\times(1+2+3+4) = 10$$

**$L_4=10$.**

**4.** Same setup, right sum.

Right endpoints: $1,2,3,4$. Values: $2,3,4,5$.

$$R_4 = 1\times(2+3+4+5) = 14$$

**$R_4=14$.**

**5.** $f(x)=x^2$ on $[0,2]$, $n=4$, left sum.

$\Delta x=\dfrac{2-0}{4}=0.5$. Left endpoints: $0,0.5,1,1.5$. Values: $0,0.25,1,2.25$.

$$L_4 = 0.5\times(0+0.25+1+2.25) = 0.5\times3.5 = 1.75$$

**$L_4=1.75$.**

**6.** Same setup, right sum.

Right endpoints: $0.5,1,1.5,2$. Values: $0.25,1,2.25,4$.

$$R_4 = 0.5\times(0.25+1+2.25+4) = 0.5\times7.5=3.75$$

**$R_4=3.75$.**

---

### 🟡 Standard

**7.** $f(x)=x^2$ on $[0,4]$, $n=4$, midpoint sum.

$\Delta x=1$. Midpoints: $0.5,1.5,2.5,3.5$. Values: $0.25,2.25,6.25,12.25$.

$$M_4 = 1\times(0.25+2.25+6.25+12.25) = 21$$

**$M_4=21$.**

**8.** $f(x)=9-x^2$ on $[0,3]$, $n=3$.

$\Delta x=1$. Note $f$ is **decreasing** on $[0,3]$ (its derivative $-2x$ is negative for $x>0$).

**Left sum:** endpoints $0,1,2$; values $9,8,5$.

$$L_3 = 1\times(9+8+5) = 22$$

**Right sum:** endpoints $1,2,3$; values $8,5,0$.

$$R_3 = 1\times(8+5+0) = 13$$

**$L_3=22$, $R_3=13$.** Since $f$ is decreasing, the **left sum overestimates** and the **right sum underestimates** the true area — consistent with our rule.

**9.** $f(x)=\dfrac1x$ on $[1,5]$, $n=4$, left sum.

$\Delta x=1$. Left endpoints: $1,2,3,4$. Values: $1, 0.5, 0.3333, 0.25$.

$$L_4 = 1\times(1+0.5+0.3333+0.25) \approx 2.0833$$

**$L_4\approx2.0833$.**

**10.** $f(x)=\sqrt{x}$ on $[0,4]$, $n=4$, right sum.

$\Delta x=1$. Right endpoints: $1,2,3,4$. Values: $1, 1.4142, 1.7321, 2$.

$$R_4 = 1\times(1+1.4142+1.7321+2) \approx 6.1463$$

**$R_4\approx6.1463$.**

**11.** $f(x)=x^2+1$ on $[-1,1]$, $n=4$, midpoint sum.

$\Delta x=\dfrac{1-(-1)}{4}=0.5$. Subintervals: $[-1,-0.5],[-0.5,0],[0,0.5],[0.5,1]$. Midpoints: $-0.75,-0.25,0.25,0.75$.

Values: $f(-0.75)=0.5625+1=1.5625$; $f(-0.25)=0.0625+1=1.0625$; $f(0.25)=1.0625$; $f(0.75)=1.5625$.

$$M_4 = 0.5\times(1.5625+1.0625+1.0625+1.5625) = 0.5\times5.25 = 2.625$$

**$M_4=2.625$.**

**12.** $f(x)=4-x$ on $[0,4]$, $n=4$.

$\Delta x=1$. **Left sum:** endpoints $0,1,2,3$; values $4,3,2,1$.

$$L_4 = 1\times(4+3+2+1)=10$$

**Right sum:** endpoints $1,2,3,4$; values $3,2,1,0$.

$$R_4 = 1\times(3+2+1+0)=6$$

**Exact area:** this region is a triangle with base $4$ and height $4$: $\text{Area}=\dfrac12(4)(4)=8$.

**$L_4=10$ (overestimate, since $f$ is decreasing), $R_4=6$ (underestimate), and the true area $8$ falls right between them — exactly as expected.**

---

### 🔴 Challenge

**13.** $f(x)=x^2$ on $[1,3]$, $n=5$, left sum.

$\Delta x = \dfrac{3-1}{5}=0.4$. Left endpoints: $1, 1.4, 1.8, 2.2, 2.6$. Values: $1, 1.96, 3.24, 4.84, 6.76$.

$$L_5 = 0.4\times(1+1.96+3.24+4.84+6.76) = 0.4\times17.8 = 7.12$$

**$L_5=7.12$.**

**14.** $f(x)=x^3$ on $[0,2]$, $n=4$, right sum.

$\Delta x=0.5$. Right endpoints: $0.5,1,1.5,2$. Values: $0.125, 1, 3.375, 8$.

$$R_4 = 0.5\times(0.125+1+3.375+8) = 0.5\times12.5 = 6.25$$

**$R_4=6.25$.**

**15.** Why does the left sum underestimate and the right sum overestimate for an increasing function?

For an increasing function, on **any** subinterval, the function's **smallest** value occurs at the **left** edge of that piece (since the function is still climbing from there), and its **largest** value occurs at the **right** edge.

A **left-endpoint rectangle** uses that smallest height as its constant rectangle height. Since the actual curve is *always at least as tall* as that smallest value across the whole piece, the rectangle sits entirely *underneath* the curve — so the total left sum can never exceed the true area. **This makes the left sum an underestimate.**

A **right-endpoint rectangle** uses the largest height on that piece. Since the actual curve is *never taller* than that value anywhere in the piece, the rectangle sits entirely *at or above* the curve — so the total right sum can never fall short of the true area. **This makes the right sum an overestimate.**

**16.** $f(x)=\sin x$ on $[0,\pi]$, $n=4$, midpoint sum.

$\Delta x = \dfrac{\pi}{4}$. Subintervals: $\left[0,\frac{\pi}{4}\right],\left[\frac{\pi}{4},\frac{\pi}{2}\right],\left[\frac{\pi}{2},\frac{3\pi}{4}\right],\left[\frac{3\pi}{4},\pi\right]$. Midpoints: $\dfrac{\pi}{8},\dfrac{3\pi}{8},\dfrac{5\pi}{8},\dfrac{7\pi}{8}$.

Values (using known sine values, in degrees for intuition: $22.5°, 67.5°, 112.5°, 157.5°$):

$$\sin\left(\frac{\pi}{8}\right)\approx0.38268 \qquad \sin\left(\frac{3\pi}{8}\right)\approx0.92388$$

$$\sin\left(\frac{5\pi}{8}\right)\approx0.92388 \qquad \sin\left(\frac{7\pi}{8}\right)\approx0.38268$$

(The middle two match the outer two due to the symmetry of sine around $\frac{\pi}{2}$.)

$$\text{Sum} = 0.38268+0.92388+0.92388+0.38268 = 2.61312$$

$$M_4 = \frac{\pi}{4}\times2.61312 \approx 0.7854\times2.61312 \approx 2.0523$$

**$M_4\approx2.0523$** (the true value of this area is exactly $2$ — the midpoint rule gets remarkably close with just $4$ rectangles).

**17.** Left sum $=20$, right sum $=28$, increasing function.

Since the function is increasing, the left sum underestimates and the right sum overestimates the true area, so:

$$20 \le \text{true area} \le 28$$

**A better single estimate:** average the two sums:

$$\frac{20+28}{2} = 24$$

**Answer: the true area is somewhere between $20$ and $28$, and a better estimate using the average of the two sums is $24$.**

---

### 🌍 Applied

**18.** Velocity data, left sum, $\Delta t=1$.

Left endpoints use $v(0), v(1), v(2), v(3)$: $0, 10, 18, 24$.

$$L_4 = 1\times(0+10+18+24) = 52$$

**Answer: estimated distance $=52$ feet.**

**19.** Same data, right sum.

Right endpoints use $v(1), v(2), v(3), v(4)$: $10, 18, 24, 28$.

$$R_4 = 1\times(10+18+24+28) = 80$$

**Answer: estimated distance $=80$ feet.** Since velocity is increasing throughout, the left sum ($52$ ft) underestimates and the right sum ($80$ ft) overestimates — the true distance traveled lies somewhere between the two.

**20.** Flow rate data, left sum, $\Delta t=2$.

Left endpoints use $r(0), r(2), r(4), r(6)$: $5, 8, 12, 15$.

$$L_4 = 2\times(5+8+12+15) = 2\times40 = 80$$

**Answer: estimated total water collected $=80$ gallons.**

**21.** Marginal profit data, right sum.

Right endpoints (for $n=3$ subintervals over $[0,3]$, with $\Delta t=1$) use $P'(1), P'(2), P'(3)$: $120, 150, 180$.

$$R_3 = 1\times(120+150+180) = 450$$

**Answer: estimated total profit accumulated $=\$450$.**
