# Unit 27: The Fundamental Theorem of Calculus — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int_0^2 x^2\,dx$

Antiderivative: $F(x)=\dfrac{x^3}{3}$.

$$F(2)-F(0) = \frac{8}{3}-0 = \frac{8}{3}$$

**Answer: $\dfrac{8}{3}$.**

**2.** $\displaystyle\int_1^3 (2x+1)\,dx$

Antiderivative: $F(x)=x^2+x$.

$$F(3)-F(1) = (9+3)-(1+1) = 12-2=10$$

**Answer: $10$.**

**3.** $\displaystyle\int_0^4 x\,dx$

Antiderivative: $F(x)=\dfrac{x^2}{2}$.

$$F(4)-F(0) = 8-0=8$$

**Answer: $8$.**

**4.** $\displaystyle\int_{-1}^2 3x^2\,dx$

Antiderivative: $F(x)=x^3$.

$$F(2)-F(-1) = 8-(-1) = 9$$

**Answer: $9$.**

**5.** $\displaystyle\int_0^1 (x^3+x)\,dx$

Antiderivative: $F(x)=\dfrac{x^4}{4}+\dfrac{x^2}{2}$.

$$F(1)-F(0) = \left(\frac14+\frac12\right)-0 = \frac34$$

**Answer: $\dfrac34$.**

**6.** $\displaystyle\int_1^2 4\,dx$

Antiderivative: $F(x)=4x$.

$$F(2)-F(1) = 8-4=4$$

**Answer: $4$.**

**7.** $\displaystyle\int_0^\pi \sin x\,dx$

Antiderivative: $F(x)=-\cos x$.

$$F(\pi)-F(0) = (-\cos\pi)-(-\cos0) = -(-1) - (-(1)) = 1-(-1) = 2$$

**Answer: $2$.**

---

### 🟡 Standard

**8.** $\displaystyle\int_0^{\pi/2} \cos x\,dx$

Antiderivative: $F(x)=\sin x$.

$$F\left(\frac{\pi}{2}\right)-F(0) = 1-0=1$$

**Answer: $1$.**

**9.** $\displaystyle\int_1^4 \sqrt{x}\,dx$

Rewrite $\sqrt{x}=x^{1/2}$. Antiderivative: $F(x)=\dfrac23x^{3/2}$.

$$F(4)-F(1) = \frac23(8)-\frac23(1) = \frac{16}{3}-\frac23 = \frac{14}{3}$$

**Answer: $\dfrac{14}{3}$.**

**10.** $\displaystyle\int_1^2 \frac{1}{x^2}\,dx$

Rewrite $\dfrac{1}{x^2}=x^{-2}$. Antiderivative: $F(x)=-x^{-1}=-\dfrac1x$.

$$F(2)-F(1) = -\frac12-(-1) = -\frac12+1=\frac12$$

**Answer: $\dfrac12$.**

**11.** $\displaystyle\int_0^2 (x^2-2x+3)\,dx$

Antiderivative: $F(x)=\dfrac{x^3}{3}-x^2+3x$.

$$F(2)-F(0) = \left(\frac83-4+6\right)-0 = \frac83+2 = \frac83+\frac63 = \frac{14}{3}$$

**Answer: $\dfrac{14}{3}$.**

**12.** $\dfrac{d}{dx}\left[\displaystyle\int_2^x (t^2+1)\,dt\right]$

By FTC Part 1, this is simply the integrand evaluated at $x$:

$$\frac{d}{dx}\left[\int_2^x (t^2+1)\,dt\right] = x^2+1$$

**13.** $\dfrac{d}{dx}\left[\displaystyle\int_0^x \sin t\,dt\right]$

By FTC Part 1:

$$\frac{d}{dx}\left[\int_0^x \sin t\,dt\right] = \sin x$$

**14.** $\displaystyle\int_{-2}^2 x^3\,dx$

Antiderivative: $F(x)=\dfrac{x^4}{4}$.

$$F(2)-F(-2) = \frac{16}{4}-\frac{16}{4} = 4-4=0$$

**Answer: $0$** — this confirms exactly what we'd predict from Unit 26's odd-function symmetry shortcut, since $x^3$ is an odd function and $[-2,2]$ is symmetric about $0$.

---

### 🔴 Challenge

**15.** $\dfrac{d}{dx}\left[\displaystyle\int_1^{x^2} (t^3+1)\,dt\right]$

Using the chain rule version of FTC Part 1, with $g(x)=x^2$ (so $g'(x)=2x$):

$$\frac{d}{dx}\left[\int_1^{x^2} (t^3+1)\,dt\right] = \big[(x^2)^3+1\big]\cdot 2x = (x^6+1)(2x) = 2x^7+2x$$

**Answer: $2x^7+2x$.**

**16.** $\dfrac{d}{dx}\left[\displaystyle\int_0^{\sin x} \sqrt{1+t^2}\,dt\right]$

Using the chain rule version, with $g(x)=\sin x$ (so $g'(x)=\cos x$):

$$\frac{d}{dx}\left[\int_0^{\sin x} \sqrt{1+t^2}\,dt\right] = \sqrt{1+\sin^2x}\cdot\cos x$$

**Answer: $\sqrt{1+\sin^2x}\cdot\cos x$.**

**17.** $\displaystyle\int_1^2 \frac{x^4+x^2}{x^2}\,dx$

Simplify first by dividing each term by $x^2$:

$$\frac{x^4}{x^2}+\frac{x^2}{x^2} = x^2+1$$

Now integrate: antiderivative $F(x)=\dfrac{x^3}{3}+x$.

$$F(2)-F(1) = \left(\frac83+2\right)-\left(\frac13+1\right) = \left(\frac83+\frac63\right)-\left(\frac13+\frac33\right) = \frac{14}{3}-\frac43 = \frac{10}{3}$$

**Answer: $\dfrac{10}{3}$.**

**18.** $\displaystyle\int_0^3 |x-1|\,dx$

Split at $x=1$, where the absolute value changes behavior: for $x<1$, $|x-1|=1-x$; for $x\ge1$, $|x-1|=x-1$.

$$\int_0^3 |x-1|\,dx = \int_0^1 (1-x)\,dx + \int_1^3 (x-1)\,dx$$

**First piece:** antiderivative $x-\dfrac{x^2}{2}$.

$$\left[1-\frac12\right] - [0-0] = 0.5$$

**Second piece:** antiderivative $\dfrac{x^2}{2}-x$.

$$\left[\frac92-3\right]-\left[\frac12-1\right] = [1.5]-[-0.5] = 2$$

**Total:**

$$0.5+2 = 2.5$$

**Answer: $2.5$.**

**19.** $F(x)=\displaystyle\int_0^x (t^2-4)\,dt$

By FTC Part 1:

$$F'(x) = x^2-4$$

Set $F'(x)=0$: $x^2-4=0 \Rightarrow x=\pm2$.

Use the First Derivative Test on $F'(x)=(x-2)(x+2)$:

Test $x<-2$ (e.g., $-3$): $(−5)(−1)=5>0$ → $F$ increasing.

Test $-2<x<2$ (e.g., $0$): $(-2)(2)=-4<0$ → $F$ decreasing.

Test $x>2$ (e.g., $3$): $(1)(5)=5>0$ → $F$ increasing.

**Answer: $F$ has a local maximum at $x=-2$ (increasing then decreasing) and a local minimum at $x=2$ (decreasing then increasing).**

---

### 🌍 Applied

**20.** $v(t)=3t^2-6t$ on $[0,3]$.

Antiderivative: $F(t)=t^3-3t^2$.

$$F(3)-F(0) = (27-27)-0 = 0$$

**Answer: net displacement $=0$** — the particle ends up back where it started, even though it moved during the interval.

**21.** $r(t)=6t+2$ on $[0,5]$.

Antiderivative: $F(t)=3t^2+2t$.

$$F(5)-F(0) = (75+10)-0=85$$

**Answer: total water collected $=85$ gallons.**

**22.** $MC(x)=2x+10$, from $x=5$ to $x=10$.

Antiderivative: $F(x)=x^2+10x$.

$$F(10)-F(5) = (100+100)-(25+50) = 200-75=125$$

**Answer: total additional cost $=\$125$.**

**23.** $D(t)=\displaystyle\int_0^t v(s)\,ds$, where $v(s)=4s+1$.

By FTC Part 1:

$$D'(t) = v(t) = 4t+1$$

**Answer: $D'(t)=4t+1$, which represents the object's instantaneous velocity at time $t$** — the rate at which total distance is accumulating at that exact moment.
