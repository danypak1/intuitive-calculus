# Unit 29: Area Between Curves — Full Solutions

### 🟢 Warm-up

**1.** $y=x$ and $y=x^2$ on $[0,1]$.

Check which is on top: at $x=0.5$, $x=0.5$ and $x^2=0.25$, so $y=x$ is on top.

$$A = \int_0^1 (x-x^2)\,dx = \left[\frac{x^2}{2}-\frac{x^3}{3}\right]_0^1 = \left(\frac12-\frac13\right)-0 = \frac16$$

**Answer: $\dfrac16$.**

**2.** $y=8-x^2$ and $y=x^2$.

Intersections: $8-x^2=x^2 \Rightarrow 8=2x^2 \Rightarrow x=\pm2$.

At $x=0$: $8-x^2=8$, $x^2=0$, so $8-x^2$ is on top.

$$A = \int_{-2}^2 \big[(8-x^2)-x^2\big]\,dx = \int_{-2}^2 (8-2x^2)\,dx = \left[8x-\frac{2x^3}{3}\right]_{-2}^2$$

$$= \left(16-\frac{16}{3}\right)-\left(-16+\frac{16}{3}\right) = 16-\frac{16}{3}+16-\frac{16}{3} = 32-\frac{32}{3} = \frac{64}{3}$$

**Answer: $\dfrac{64}{3}$.**

**3.** $y=x^2$ and $y=2x$.

Intersections: $x^2=2x \Rightarrow x^2-2x=0 \Rightarrow x(x-2)=0 \Rightarrow x=0,2$.

At $x=1$: $x^2=1$, $2x=2$, so $2x$ is on top.

$$A = \int_0^2 (2x-x^2)\,dx = \left[x^2-\frac{x^3}{3}\right]_0^2 = \left(4-\frac83\right)-0 = \frac43$$

**Answer: $\dfrac43$.**

**4.** $y=x+6$ and $y=x^2$.

Intersections: $x^2=x+6 \Rightarrow x^2-x-6=0 \Rightarrow (x-3)(x+2)=0 \Rightarrow x=-2,3$.

At $x=0$: $x+6=6$, $x^2=0$, so $x+6$ is on top.

$$A = \int_{-2}^3 \big[(x+6)-x^2\big]\,dx = \left[\frac{x^2}{2}+6x-\frac{x^3}{3}\right]_{-2}^3$$

At $x=3$: $\dfrac92+18-9 = \dfrac{27}{2}$.

At $x=-2$: $2-12+\dfrac83 = -10+\dfrac83 = -\dfrac{22}{3}$.

$$A = \frac{27}{2}-\left(-\frac{22}{3}\right) = \frac{27}{2}+\frac{22}{3} = \frac{81}{6}+\frac{44}{6} = \frac{125}{6}$$

**Answer: $\dfrac{125}{6}\approx20.83$.**

**5.** $y=4-x^2$ and the x-axis.

Intersections: $4-x^2=0 \Rightarrow x=\pm2$.

$$A = \int_{-2}^2 (4-x^2)\,dx = \left[4x-\frac{x^3}{3}\right]_{-2}^2 = \left(8-\frac83\right)-\left(-8+\frac83\right) = 16-\frac{16}{3} = \frac{32}{3}$$

**Answer: $\dfrac{32}{3}$.**

**6.** $y=x$ and $y=x^3$ on $[0,1]$.

At $x=0.5$: $x=0.5$, $x^3=0.125$, so $y=x$ is on top.

$$A = \int_0^1 (x-x^3)\,dx = \left[\frac{x^2}{2}-\frac{x^4}{4}\right]_0^1 = \left(\frac12-\frac14\right)-0 = \frac14$$

**Answer: $\dfrac14$.**

---

### 🟡 Standard

**7.** $y=x^2-4$ and $y=4-x^2$.

Intersections: $x^2-4=4-x^2 \Rightarrow 2x^2=8 \Rightarrow x=\pm2$.

At $x=0$: $x^2-4=-4$, $4-x^2=4$, so $4-x^2$ is on top — same setup as Problem 2.

$$A = \int_{-2}^2 (8-2x^2)\,dx = \frac{64}{3}$$

**Answer: $\dfrac{64}{3}$.**

**8.** $y=x^3$ and $y=4x$.

Intersections: $x^3=4x \Rightarrow x^3-4x=0 \Rightarrow x(x^2-4)=0 \Rightarrow x=0,\pm2$.

Check each region: at $x=-1$: $x^3=-1$, $4x=-4$; since $-1>-4$, $x^3$ is on top on $(-2,0)$.

At $x=1$: $x^3=1$, $4x=4$; since $4>1$, $4x$ is on top on $(0,2)$.

$$A = \int_{-2}^0 (x^3-4x)\,dx + \int_0^2 (4x-x^3)\,dx$$

First piece: $\left[\dfrac{x^4}{4}-2x^2\right]_{-2}^0 = 0-(4-8) = 4$.

Second piece: $\left[2x^2-\dfrac{x^4}{4}\right]_0^2 = (8-4)-0 = 4$.

$$A = 4+4=8$$

**Answer: $8$.**

**9.** $y=\sqrt{x}$ and $y=\dfrac{x}{2}$ on $[0,4]$.

Intersections: $\sqrt{x}=\dfrac{x}{2} \Rightarrow x=\dfrac{x^2}{4} \Rightarrow 4x=x^2 \Rightarrow x(x-4)=0 \Rightarrow x=0,4$.

At $x=1$: $\sqrt{x}=1$, $\dfrac{x}{2}=0.5$, so $\sqrt{x}$ is on top.

$$A = \int_0^4 \left(\sqrt{x}-\frac{x}{2}\right)dx = \left[\frac23x^{3/2}-\frac{x^2}{4}\right]_0^4 = \left(\frac23(8)-4\right)-0 = \frac{16}{3}-4 = \frac43$$

**Answer: $\dfrac43$.**

**10.** $y=6x(x^2+1)^2$, x-axis, $x=0$, $x=1$.

Since $x\ge0$ and $(x^2+1)^2>0$ throughout $[0,1]$, the function stays at or above the x-axis — no splitting needed.

Let $u=x^2+1$, $du=2x\,dx$. When $x=0$, $u=1$; when $x=1$, $u=2$.

$$\int_0^1 6x(x^2+1)^2\,dx = 6\int_1^2 u^2\cdot\frac{du}{2} = 3\int_1^2 u^2\,du = 3\left[\frac{u^3}{3}\right]_1^2 = \Big[u^3\Big]_1^2 = 8-1=7$$

**Answer: $7$.**

**11.** $y=x^2+2$ and $y=-x+4$.

Intersections: $x^2+2=-x+4 \Rightarrow x^2+x-2=0 \Rightarrow (x+2)(x-1)=0 \Rightarrow x=-2,1$.

At $x=0$: $x^2+2=2$, $-x+4=4$, so $-x+4$ is on top.

$$A = \int_{-2}^1 \big[(-x+4)-(x^2+2)\big]\,dx = \int_{-2}^1 (-x^2-x+2)\,dx = \left[-\frac{x^3}{3}-\frac{x^2}{2}+2x\right]_{-2}^1$$

At $x=1$: $-\dfrac13-\dfrac12+2 = \dfrac76$.

At $x=-2$: $\dfrac83-2-4 = -\dfrac{10}{3}$.

$$A = \frac76-\left(-\frac{10}{3}\right) = \frac76+\frac{20}{6} = \frac{27}{6} = \frac92$$

**Answer: $\dfrac92=4.5$.**

**12.** $y=x^3-x$ and the x-axis on $[-1,1]$.

The curve crosses the axis at $x=-1,0,1$. On $(-1,0)$: test $x=-0.5$: $(-0.125)-(-0.5)=0.375>0$, above axis. On $(0,1)$: test $x=0.5$: $0.125-0.5=-0.375<0$, below axis.

$$A = \int_{-1}^0 (x^3-x)\,dx + \int_0^1 \big[-(x^3-x)\big]\,dx = \int_{-1}^0 (x^3-x)\,dx + \int_0^1 (x-x^3)\,dx$$

First piece: $\left[\dfrac{x^4}{4}-\dfrac{x^2}{2}\right]_{-1}^0 = 0-\left(\dfrac14-\dfrac12\right) = 0-\left(-\dfrac14\right) = \dfrac14$.

Second piece: $\left[\dfrac{x^2}{2}-\dfrac{x^4}{4}\right]_0^1 = \left(\dfrac12-\dfrac14\right)-0 = \dfrac14$.

$$A = \frac14+\frac14 = \frac12$$

**Answer: $\dfrac12$.**

---

### 🔴 Challenge

**13.** $y=-x^2+3x$ and $y=2x^3-x^2-5x$.

Set equal: $-x^2+3x = 2x^3-x^2-5x \Rightarrow 3x = 2x^3-5x \Rightarrow 8x-2x^3=0 \Rightarrow 2x(4-x^2)=0 \Rightarrow x=0,\pm2$.

Let $d(x) = (-x^2+3x)-(2x^3-x^2-5x) = -2x^3+8x = 2x(4-x^2)$.

On $(-2,0)$, test $x=-1$: $2(-1)(3)=-6<0$, so $y=2x^3-x^2-5x$ is on top there.

On $(0,2)$, test $x=1$: $2(1)(3)=6>0$, so $y=-x^2+3x$ is on top there.

$$A = \int_{-2}^0 \big[-d(x)\big]\,dx + \int_0^2 d(x)\,dx = \int_{-2}^0 (2x^3-8x)\,dx + \int_0^2 (-2x^3+8x)\,dx$$

First piece: $\left[\dfrac{x^4}{2}-4x^2\right]_{-2}^0 = 0-(8-16) = 8$.

Second piece: $\left[-\dfrac{x^4}{2}+4x^2\right]_0^2 = (-8+16)-0 = 8$.

$$A = 8+8=16$$

**Answer: $16$.**

**14.** $y=x^4-4x^2$ and the x-axis.

Roots: $x^2(x^2-4)=0 \Rightarrow x=0,\pm2$.

Check the sign: at $x=1$, $1-4=-3<0$; at $x=-1$, $1-4=-3<0$. The curve stays at or below the axis throughout $[-2,2]$ (touching $0$ only at the three roots, never crossing back above), so **no splitting is needed**.

$$A = \int_{-2}^2 \big[0-(x^4-4x^2)\big]\,dx = \int_{-2}^2 (4x^2-x^4)\,dx = \left[\frac{4x^3}{3}-\frac{x^5}{5}\right]_{-2}^2$$

At $x=2$: $\dfrac{32}{3}-\dfrac{32}{5} = \dfrac{160}{15}-\dfrac{96}{15}=\dfrac{64}{15}$.

At $x=-2$: $-\dfrac{32}{3}+\dfrac{32}{5} = -\dfrac{64}{15}$.

$$A = \frac{64}{15}-\left(-\frac{64}{15}\right) = \frac{128}{15}$$

**Answer: $\dfrac{128}{15}$.**

**15.** $y=x^3-3x$ and $y=x$.

Intersections: $x^3-3x=x \Rightarrow x^3-4x=0 \Rightarrow x(x^2-4)=0 \Rightarrow x=0,\pm2$.

Let $d(x)=(x^3-3x)-x=x^3-4x$.

On $(-2,0)$, test $x=-1$: $-1+4=3>0$, so $y=x^3-3x$ is on top there.

On $(0,2)$, test $x=1$: $1-4=-3<0$, so $y=x$ is on top there.

$$A = \int_{-2}^0 (x^3-4x)\,dx + \int_0^2 (4x-x^3)\,dx$$

First piece: $\left[\dfrac{x^4}{4}-2x^2\right]_{-2}^0 = 0-(4-8)=4$.

Second piece: $\left[2x^2-\dfrac{x^4}{4}\right]_0^2 = (8-4)-0=4$.

$$A = 4+4=8$$

**Answer: $8$.**

**16.** $y=x\sqrt{9-x^2}$ from $x=0$ to $x=3$.

Since $x\ge0$ and $\sqrt{9-x^2}\ge0$ throughout $[0,3]$, the curve stays at or above the axis — no splitting needed.

Let $u=9-x^2$, $du=-2x\,dx \Rightarrow x\,dx=-\dfrac{du}{2}$. When $x=0$, $u=9$; when $x=3$, $u=0$.

$$\int_0^3 x\sqrt{9-x^2}\,dx = \int_9^0 \sqrt{u}\cdot\left(-\frac{du}{2}\right) = \frac12\int_0^9 \sqrt{u}\,du = \frac12\left[\frac23u^{3/2}\right]_0^9$$

$$= \frac13\Big[u^{3/2}\Big]_0^9 = \frac13(27-0) = 9$$

**Answer: $9$.**

**17.** $y=3x^2(x^3+1)$ from $x=-1$ to $x=1$.

Since $x^2\ge0$ always, and $x^3+1\ge0$ for all $x\ge-1$ (because $x^3\ge-1$ throughout this range), the whole product stays at or above the x-axis on $[-1,1]$ — no splitting needed.

Let $u=x^3+1$, $du=3x^2\,dx$. When $x=-1$, $u=0$; when $x=1$, $u=2$.

$$\int_{-1}^1 3x^2(x^3+1)\,dx = \int_0^2 u\,du = \left[\frac{u^2}{2}\right]_0^2 = 2-0=2$$

**Answer: $2$.**

---

### 🌍 Applied

**18.** $R_A(t)=100+20t$, $R_B(t)=80+15t$, on $[0,10]$.

Since $R_A>R_B$ throughout (both the starting value and the growth rate favor A), the extra cumulative revenue is:

$$\int_0^{10} \big[R_A(t)-R_B(t)\big]\,dt = \int_0^{10} (20+5t)\,dt = \left[20t+\frac{5t^2}{2}\right]_0^{10} = (200+250)-0=450$$

**Answer: Company A earns $\$450$ more than Company B over the $10$ weeks.**

**19.** $r_1(t)=5+2t$, $r_2(t)=3+t$, on $[0,6]$.

$$\int_0^6 \big[r_1(t)-r_2(t)\big]\,dt = \int_0^6 (2+t)\,dt = \left[2t+\frac{t^2}{2}\right]_0^6 = (12+18)-0=30$$

**Answer: Tank 1 has collected $30$ more gallons than Tank 2 after $6$ minutes.**

**20.** $v_A(t)=8+0.5t$, $v_B(t)=7+0.3t$, on $[0,4]$.

$$\int_0^4 \big[v_A(t)-v_B(t)\big]\,dt = \int_0^4 (1+0.2t)\,dt = \left[t+0.1t^2\right]_0^4 = (4+1.6)-0=5.6$$

**Answer: Runner A gains a lead of $5.6$ miles over Runner B.**

**21.** $p_A(x)=50+3x$, $p_B(x)=40+2x$, on $[0,20]$.

$$\int_0^{20} \big[p_A(x)-p_B(x)\big]\,dx = \int_0^{20} (10+x)\,dx = \left[10x+\frac{x^2}{2}\right]_0^{20} = (200+200)-0=400$$

**Answer: Strategy A generates $\$400$ more total profit than Strategy B over the $20$ weeks.**
